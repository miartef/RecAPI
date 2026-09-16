# StreamFit - API

Guia completo para instalação, configuração e teste das rotas da API StreamFit.

---

## 🚀 Configuração Inicial do Projeto

Execute os comandos abaixo na raiz do projeto para criar a estrutura, instalar dependências e configurar o banco de dados.

### 1. Inicializar o projeto e instalar dependências
```bash
npm init -y
npm i express nodemon dotenv cors
npx create-db
criar o .env: DATABASE_URL="postgresql://postgres:senai@localhost:5432/streamfit?schema=public"
npx prisma generate
npx prisma migrate dev --name init
npm run dev