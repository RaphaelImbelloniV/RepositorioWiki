# 🛠️ Configurações Padrão de IDE — DevNova Solutions

Esta página define padrões e extensões obrigatórias para garantir consistência no desenvolvimento.

---

## 🧩 VS Code

### 📦 Extensões Obrigatórias
- ESLint  
- Prettier  
- GitLens  
- Docker  
- EditorConfig  

### ⚙️ Configurações (`settings.json`)

```json
{
  "editor.formatOnSave": true,
  "editor.minimap.enabled": false,
  "editor.tabSize": 2,
  "eslint.enable": true,
  "files.autoSave": "afterDelay"
}
```

🧩 IntelliJ IDEA
🔌 Plugins Recomendados

- SonarLint
- 
- Key Promoter X
- 
- Database Tools
- 
- Lombok


📏 Code Style

O padrão utilizado é uma variação do Google Style.

Arquivo oficial:

```bash
/infrastructure/config/intellij/code-style.xml
```

🧪 Linters e Formatadores

- JavaScript/TypeScript: ESLint + Prettier
- 
- Java: CheckStyle
- 
- PHP: PHPStan

