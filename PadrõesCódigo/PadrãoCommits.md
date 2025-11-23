# Boas Práticas e Padrões de Código

## Padrão de Commits (Conventional Commits)

Exemplos:

```bash
feat(api): adiciona criação de usuário
fix(auth): corrige refresh token
docs(wiki): atualiza documentação
```

---

## Padrões de Branch

- `main` → Produção  
- `develop` → Preparação  
- `feature/*` → Novas features  
- `bugfix/*` → Correções  
- `hotfix/*` → Corretivos urgentes  

---

## Cobertura de Testes

- Mínimo de **80%** obrigatório  
- Testes exigidos em:  
  - Controllers  
  - Services  
  - Helpers/Utils  

---

## Regras Gerais de Código Limpo

- Funções com até **20 linhas**  
- Evitar nomes genéricos (`data`, `obj`)  
- Priorizar composição sobre herança  
- Documentar endpoints com comentários claros  

---

## Regras de Pull Request

- Mínimo **2 revisores**  
- PRs com até **300 linhas modificadas**  
- Checklist obrigatório no PR  