# Scripts de Banco de Dados


# 🗄️ Scripts de Banco de Dados — DevNova Solutions

Esta página reúne scripts padrões utilizados para configurar bancos de dados em clientes.

---

## 🏗️ Criação de Banco (PostgreSQL)

```sql
CREATE DATABASE devnova_client;
CREATE USER client_user WITH ENCRYPTED PASSWORD '12345';
GRANT ALL PRIVILEGES ON DATABASE devnova_client TO client_user;
```

Criação de Tabelas Básicas

```sql
CREATE TABLE usuarios (
  id SERIAL PRIMARY KEY,
  nome VARCHAR(100) NOT NULL,
  email VARCHAR(150) UNIQUE NOT NULL,
  criado_em TIMESTAMP DEFAULT NOW()
);
```

Script de Seed Inicial

```sql
INSERT INTO usuarios (nome, email)
VALUES 
('Administrador', 'admin@cliente.com'),
('Suporte', 'suporte@cliente.com');
```

Script de Alteração (Migration)

```sql
ALTER TABLE usuarios
ADD COLUMN ativo BOOLEAN DEFAULT TRUE;
```

Script de Limpeza de Tabelas

```sql
TRUNCATE TABLE usuarios RESTART IDENTITY CASCADE;
```