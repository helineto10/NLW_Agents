# NLW Agents

Projeto desenvolvido durante o evento **NLW (Next Level Week)** da Rocketseat, focado em criar uma aplicação de agentes inteligentes.

## 🚀 Tecnologias Utilizadas

### Backend
- **Fastify** - Framework web rápido para Node.js
- **Drizzle ORM** - ORM TypeScript-first para PostgreSQL
- **PostgreSQL** - Banco de dados com extensão pgvector
- **Zod** - Validação de schemas TypeScript
- **TypeScript** - Linguagem de programação

### Frontend
- **React 19** - Biblioteca para interfaces de usuário
- **Vite** - Build tool e dev server
- **React Router DOM** - Roteamento para React
- **TanStack Query** - Gerenciamento de estado e cache
- **Tailwind CSS** - Framework CSS utilitário
- **Radix UI** - Componentes acessíveis
- **Lucide React** - Ícones

### Ferramentas
- **Biome** - Linter e formatter
- **Docker** - Containerização do banco de dados

## 📁 Estrutura do Projeto

```
agents/
├── server/          # Backend Fastify + Drizzle
├── web/            # Frontend React + Vite
└── README.md
```

## ⚙️ Setup e Configuração

### Pré-requisitos
- Node.js 18+
- Docker e Docker Compose
- npm

### Backend

1. **Instalar dependências:**
```bash
cd server
npm install
```

2. **Configurar banco de dados:**
```bash
docker-compose up -d
```

3. **Executar migrações:**
```bash
npx drizzle-kit migrate
```

4. **Executar seed do banco:**
```bash
npm run db:seed
```

5. **Iniciar servidor de desenvolvimento:**
```bash
npm run dev
```

### Frontend

1. **Instalar dependências:**
```bash
cd web
npm install
```

2. **Iniciar servidor de desenvolvimento:**
```bash
npm run dev
```

## 🔧 Scripts Disponíveis

### Backend
- `npm run dev` - Servidor de desenvolvimento com hot reload
- `npm start` - Servidor de produção
- `npx drizzle-kit migrate` - Executar migrações do banco de dados
- `npm run db:seed` - Executar seed do banco de dados

### Frontend
- `npm run dev` - Servidor de desenvolvimento
- `npm run build` - Build de produção
- `npm run preview` - Preview do build

## 🌐 Acesso

- **Frontend:** http://localhost:5173
- **Backend:** http://localhost:3333
- **Banco de dados:** PostgreSQL na porta 5432

## 📝 Padrões de Projeto

- **Arquitetura:** Monorepo com backend e frontend separados
- **API:** REST com Fastify e validação Zod
- **Banco:** PostgreSQL com Drizzle ORM
- **Frontend:** React com roteamento e gerenciamento de estado
- **Estilização:** Tailwind CSS com componentes Radix UI
- **Code Quality:** Biome para linting e formatação 
