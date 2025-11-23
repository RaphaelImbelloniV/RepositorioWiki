# Procedimentos Operacionais — DevNova Solutions

Runbooks para suporte, deploy e resolução de incidentes.

---

## 🐳 Reiniciar Serviços Docker

```bash
docker compose down
docker compose pull
docker compose up -d
```

🚀 Checklist de Deploy

1. Rodar todos os testes

1. Executar análise no SonarQube

1. Criar tag de versão

1. Iniciar pipeline no CI/CD

1. Validar logs

1. Testar serviços no ambiente


Rollback de Versão

```bash
docker compose down
git checkout tags/v1.2.0
docker compose up -d
```

📡 Monitoramento Básico

Verificar CPU/RAM
```bash
docker stats
```

Ver logs do container
```bash
docker logs api --tail 100
```

Resolução de Incidentes
Erro: Banco "Connection Refused"

- Validar se o container está ativo

- Testar porta:
```bash
nc -zv localhost 5432
```

API não responde após deploy

- Reiniciar:
```bash
docker compose restart api
```

- Verificar .env duplicadas

