<div align="center">
 
```
 ██████╗████████╗    ██████╗ ███████╗██╗   ██╗███████╗
██╔════╝╚══██╔══╝    ██╔══██╗██╔════╝██║   ██║██╔════╝
██║        ██║       ██║  ██║█████╗  ██║   ██║███████╗
██║        ██║       ██║  ██║██╔══╝  ╚██╗ ██╔╝╚════██║
╚██████╗   ██║       ██████╔╝███████╗ ╚████╔╝ ███████║
 ╚═════╝   ╚═╝       ╚═════╝ ╚══════╝  ╚═══╝  ╚══════╝
```
 
# 🍃 Dashboard Cannloli — CT Devs
 
> **Transformando dados em decisões. Um dashboard à altura da Cannloli.**
 
![Status](https://img.shields.io/badge/status-em%20desenvolvimento-yellow?style=for-the-badge&logo=github)
![Time](https://img.shields.io/badge/time-CT%20Devs-green?style=for-the-badge)
![Cliente](https://img.shields.io/badge/cliente-Cannloli-brightgreen?style=for-the-badge)
![Python](https://img.shields.io/badge/Python-3.11+-blue?style=for-the-badge&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-0.111+-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![React](https://img.shields.io/badge/React-18+-61DAFB?style=for-the-badge&logo=react&logoColor=black)
 
</div>
 
---
 
## 📋 Índice
 
- [Sobre o Projeto](#-sobre-o-projeto)
- [Sobre o Time](#-sobre-o-time)
- [Tecnologias](#-tecnologias)
- [Estrutura do Projeto](#-estrutura-do-projeto)
- [Pré-requisitos](#-pré-requisitos)
- [Instalação e Configuração](#-instalação-e-configuração)
- [Como Rodar](#-como-rodar)
- [Variáveis de Ambiente](#-variáveis-de-ambiente)
- [Padrões e Convenções](#-padrões-e-convenções)
- [Fluxo de Trabalho com Git](#-fluxo-de-trabalho-com-git)
- [Contato](#-contato)
 
---
 
## 🍃 Sobre o Projeto
 
O **Dashboard Cannloli** é uma solução de business intelligence desenvolvida pelo time **CT Devs** para centralizar, visualizar e analisar os dados estratégicos da empresa **Cannloli**.
 
O sistema combina uma API de alta performance construída com **FastAPI**, pipelines de dados em **Python** e uma interface moderna em **React** — entregando uma experiência fluida do dado bruto até a tomada de decisão.
 
### 🎯 Objetivos
 
- **Centralização de dados** — integração com as fontes de dados da Cannloli em um único painel
- **Análise inteligente** — processamento e transformação de dados com bibliotecas Python especializadas
- **Visualizações claras** — gráficos interativos, indicadores de performance e relatórios exportáveis
- **Tomada de decisão ágil** — informações atualizadas em tempo real para gestores e líderes
- **Experiência de uso** — interface limpa, responsiva e acessível em qualquer dispositivo
 
---
 
## 👥 Sobre o Time
 
> **CT Devs** — Um time movido por código limpo, colaboração e entrega de valor.
 
| Integrante | GitHub | Função |
|---|---|---|
| 🧑‍💻 **Breno Costa** | [@brenocosta](https://github.com/brenocosta) | Dev / Tech Lead |
| 🧑‍💻 **Felipe Yamaschita** | [@felipeyamaschita](https://github.com/felipeyamaschita) | Dev / Frontend |
| 🧑‍💻 **Vinicius Nishimura** | [@viniciusnishimura](https://github.com/viniciusnishimura) | Dev / Backend & Dados |
| 🧑‍💻 **Bruno Souza** | [@brunosouza](https://github.com/brunosouza) | Dev / UI & UX |
 
> ⚠️ *Atualize os links de GitHub acima com os usuários reais de cada integrante.*
 
---
 
## 🛠 Tecnologias
 
### 🐍 Backend — Python + FastAPI
 
| Tecnologia | Descrição |
|---|---|
| **Python 3.11+** | Linguagem principal do backend |
| **FastAPI** | Framework web assíncrono e de alta performance para a API REST |
| **Uvicorn** | Servidor ASGI para rodar a aplicação FastAPI |
| **Pydantic v2** | Validação e serialização de dados |
| **SQLAlchemy** | ORM para modelagem e acesso ao banco de dados |
| **Alembic** | Gerenciamento de migrations do banco |
| **PostgreSQL** | Banco de dados relacional |
 
### 📊 Dados & Análise — Python
 
| Tecnologia | Descrição |
|---|---|
| **Pandas** | Manipulação e transformação de dados tabulares |
| **NumPy** | Computação numérica e operações vetorizadas |
| **Matplotlib / Seaborn** | Geração de gráficos e visualizações no backend |
| **Plotly** | Gráficos interativos exportáveis para o frontend |
| **Scikit-learn** | Modelos estatísticos e análise preditiva (se aplicável) |
 
### ⚛️ Frontend — React
 
| Tecnologia | Descrição |
|---|---|
| **React 18** | Biblioteca para construção da interface |
| **TypeScript** | Tipagem estática para um código mais seguro |
| **Vite** | Build tool e dev server ultra-rápido |
| **Tailwind CSS** | Estilização utilitária e responsiva |
| **Recharts** | Gráficos e visualizações interativas |
| **React Router** | Navegação entre páginas do dashboard |
| **Axios** | Requisições HTTP para a API FastAPI |
| **React Query** | Gerenciamento de estado assíncrono e cache |
 
### ⚙️ Ferramentas & Infraestrutura
 
| Tecnologia | Descrição |
|---|---|
| **Docker + Docker Compose** | Containerização do ambiente completo |
| **Poetry** | Gerenciamento de dependências Python |
| **ESLint + Prettier** | Padronização e formatação do código frontend |
| **Ruff / Black** | Linting e formatação do código Python |
| **Git + GitHub** | Versionamento e colaboração |
| **GitHub Actions** | CI/CD automatizado |
 
---
 
## 📁 Estrutura do Projeto
 
```
cannloli-dashboard/
│
├── 📁 backend/                        # API FastAPI + pipeline de dados
│   ├── 📁 app/
│   │   ├── 📁 api/                    # Rotas e endpoints
│   │   │   └── 📁 v1/
│   │   │       ├── 📁 endpoints/      # Handlers por domínio
│   │   │       └── router.py
│   │   ├── 📁 core/                   # Configurações gerais
│   │   │   ├── config.py
│   │   │   └── security.py
│   │   ├── 📁 data/                   # Camada de dados e análise
│   │   │   ├── 📁 pipelines/          # Scripts de ETL e transformação
│   │   │   ├── 📁 analysis/           # Lógica analítica com Pandas/NumPy
│   │   │   └── 📁 charts/             # Geração de gráficos com Plotly
│   │   ├── 📁 db/                     # Banco de dados
│   │   │   ├── 📁 models/             # Modelos SQLAlchemy
│   │   │   ├── 📁 migrations/         # Alembic migrations
│   │   │   └── session.py
│   │   ├── 📁 schemas/                # Schemas Pydantic (request/response)
│   │   ├── 📁 services/               # Regras de negócio
│   │   └── main.py                    # Entrypoint da aplicação
│   ├── 📁 tests/
│   ├── pyproject.toml                 # Dependências (Poetry)
│   ├── alembic.ini
│   └── .env.example
│
├── 📁 frontend/                       # Interface React
│   ├── 📁 public/
│   ├── 📁 src/
│   │   ├── 📁 assets/                 # Imagens, ícones e fontes
│   │   ├── 📁 components/             # Componentes reutilizáveis
│   │   │   ├── 📁 charts/             # Gráficos e visualizações
│   │   │   ├── 📁 layout/             # Header, Sidebar, Footer
│   │   │   └── 📁 ui/                 # Botões, Cards, Modais etc.
│   │   ├── 📁 pages/                  # Páginas do dashboard
│   │   ├── 📁 hooks/                  # Custom hooks React
│   │   ├── 📁 services/               # Integração com a API
│   │   ├── 📁 types/                  # Tipagens TypeScript
│   │   ├── 📁 utils/                  # Funções utilitárias
│   │   ├── App.tsx
│   │   └── main.tsx
│   ├── package.json
│   ├── vite.config.ts
│   └── .env.example
│
├── 📁 docs/                           # Documentação e diagramas
├── docker-compose.yml
└── README.md
```
 
---
 
## ✅ Pré-requisitos
 
Antes de começar, certifique-se de ter instalado:
 
- [Python](https://www.python.org/) `>= 3.11`
- [Poetry](https://python-poetry.org/) `>= 1.8`
- [Node.js](https://nodejs.org/) `>= 18.x`
- [npm](https://www.npmjs.com/) `>= 9.x`
- [Docker](https://www.docker.com/) e [Docker Compose](https://docs.docker.com/compose/) *(recomendado)*
- [Git](https://git-scm.com/)
 
---
 
## ⚙️ Instalação e Configuração
 
### 1. Clone o repositório
 
```bash
git clone https://github.com/ct-devs/cannloli-dashboard.git
cd cannloli-dashboard
```
 
### 2. Configure o Backend
 
```bash
cd backend
 
# Instale as dependências com Poetry
poetry install
 
# Ative o ambiente virtual
poetry shell
 
# Configure as variáveis de ambiente
cp .env.example .env
```
 
### 3. Configure o Frontend
 
```bash
cd ../frontend
 
npm install
cp .env.example .env
```
 
### 4. Suba o banco de dados
 
```bash
# Na raiz do projeto
docker-compose up db -d
```
 
### 5. Execute as migrations
 
```bash
cd backend
alembic upgrade head
```
 
---
 
## ▶️ Como Rodar
 
### Opção 1 — Com Docker (Recomendado)
 
```bash
docker-compose up --build
```
 
### Opção 2 — Sem Docker
 
**Backend (FastAPI):**
```bash
cd backend
poetry shell
uvicorn app.main:app --reload --port 8000
```
 
**Frontend (React):** *(em outro terminal)*
```bash
cd frontend
npm run dev
```
 
### Acessos
 
| Serviço | URL |
|---|---|
| 🌐 Frontend | `http://localhost:5173` |
| 🔌 API FastAPI | `http://localhost:8000` |
| 📄 Swagger UI | `http://localhost:8000/docs` |
| 📄 ReDoc | `http://localhost:8000/redoc` |
| 🗄️ Banco de Dados | `localhost:5432` |
 
> O FastAPI gera automaticamente documentação interativa da API em `/docs` e `/redoc`.
 
---
 
## 🔐 Variáveis de Ambiente
 
### Frontend — `frontend/.env`
 
```env
VITE_API_URL=http://localhost:8000
VITE_APP_NAME=Cannloli Dashboard
```
 
### Backend — `backend/.env`
 
```env
# Servidor
APP_ENV=development
APP_PORT=8000
 
# Banco de Dados
DATABASE_URL=postgresql+asyncpg://usuario:senha@localhost:5432/cannloli_db
 
# Autenticação
SECRET_KEY=sua_chave_secreta_aqui
ALGORITHM=HS256
ACCESS_TOKEN_EXPIRE_MINUTES=60
```
 
> ⚠️ **Nunca** commite o arquivo `.env` com dados reais. Use sempre o `.env.example`.
 
---
 
## 📐 Padrões e Convenções
 
### Código
 
- **Idioma do código:** Inglês (variáveis, funções, comentários técnicos)
- **Idioma da UI:** Português (textos visíveis ao usuário)
- **Python:** formatação com `Black`, linting com `Ruff`
- **Frontend:** formatação e linting com `ESLint + Prettier`
 
### Commits
 
Seguimos o padrão [Conventional Commits](https://www.conventionalcommits.org/):
 
```
<tipo>(escopo): descrição curta
 
Exemplos:
feat(dashboard): adiciona gráfico de vendas mensais
fix(auth): corrige expiração do token JWT
refactor(pipeline): otimiza transformação com pandas
docs(readme): atualiza instruções de instalação
test(api): adiciona testes para endpoint de métricas
```
 
| Tipo | Quando usar |
|---|---|
| `feat` | Nova funcionalidade |
| `fix` | Correção de bug |
| `refactor` | Refatoração de código |
| `style` | Ajustes de estilo/formatação |
| `docs` | Alterações na documentação |
| `test` | Criação ou ajuste de testes |
| `chore` | Tarefas de manutenção |
 
---
 
## 🌿 Fluxo de Trabalho com Git
 
```
main         ← código em produção (protegida)
  └─ develop ← branch de integração
        └─ feature/nome-da-feature
        └─ fix/nome-do-bug
        └─ hotfix/nome-do-hotfix
```
 
### Passo a passo para contribuir
 
```bash
# 1. Atualize sua branch develop local
git checkout develop
git pull origin develop
 
# 2. Crie sua branch de feature
git checkout -b feature/nome-da-sua-feature
 
# 3. Faça suas alterações e commits
git add .
git commit -m "feat(módulo): descrição do que foi feito"
 
# 4. Suba para o repositório remoto
git push origin feature/nome-da-sua-feature
 
# 5. Abra um Pull Request para a branch develop no GitHub
```
 
### Regras para Pull Request
 
- [ ] Código segue os padrões do projeto (Black/Ruff no Python, ESLint/Prettier no Frontend)
- [ ] Funcionalidade testada localmente
- [ ] Branch atualizada com a `develop`
- [ ] PR possui descrição clara do que foi feito
- [ ] Pelo menos **1 aprovação** de outro membro do time para o merge
 
---
 
## 📬 Contato
 
Para dúvidas, sugestões ou reportar problemas, abra uma [Issue](https://github.com/ct-devs/cannloli-dashboard/issues) no repositório ou entre em contato com algum integrante do time CT Devs.
 
---
 
<div align="center">
 
**CT Devs** — Desenvolvido com 💚 para a Cannloli
 
*"Transformando dados em decisões. Um dashboard à altura da Cannloli."*
 
</div>
