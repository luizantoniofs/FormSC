# Fala Cidadão - Plataforma de Engajamento Cívico de Balneário Camboriú

![Logo da Prefeitura de Balneário Camboriú](./client/src/assets/prefeitura-logo.png)

Uma plataforma web para cidadãos de Balneário Camboriú reportarem problemas urbanos e acompanharem o status de suas solicitações.

## Sobre o Projeto

O **Fala Cidadão** é uma plataforma desenvolvida para melhorar a comunicação entre os moradores e a prefeitura de Balneário Camboriú. Através dela, os cidadãos podem:

- Reportar problemas urbanos como buracos em vias, iluminação deficiente, coleta de lixo, etc.
- Receber um número de protocolo para acompanhamento
- Verificar o status de suas solicitações usando o número de protocolo
- Receber atualizações sobre o andamento do atendimento

## Tecnologias Utilizadas

### Frontend
- React
- TailwindCSS
- Shadcn/UI Components
- Wouter (Roteamento)
- React Query
- React Hook Form + Zod

### Backend
- Node.js
- Express
- Drizzle ORM
- PostgreSQL

## Como Executar o Projeto

### Pré-requisitos
- Node.js 16+
- PostgreSQL

### Passos para Instalação

1. Clone este repositório
```bash
git clone https://github.com/seu-usuario/fala-cidadao-bc.git
cd fala-cidadao-bc
```

2. Instale as dependências
```bash
npm install
```

3. Configure as variáveis de ambiente
Crie um arquivo `.env` na raiz do projeto com as seguintes variáveis:
```
DATABASE_URL=postgres://user:password@localhost:5432/fala_cidadao
PGPORT=5432
PGUSER=seu_usuario
PGPASSWORD=sua_senha
PGDATABASE=fala_cidadao
PGHOST=localhost
```

4. Crie as tabelas no banco de dados
```bash
npm run db:push
```

5. Inicie o servidor de desenvolvimento
```bash
npm run dev
```

6. Acesse a aplicação em `http://localhost:5000`

## Estrutura do Projeto

```
├── client/           # Frontend React
│   ├── src/
│   │   ├── assets/   # Imagens e outros arquivos estáticos
│   │   ├── components/ # Componentes React reutilizáveis
│   │   ├── pages/    # Páginas da aplicação
│   │   ├── lib/      # Utilitários e configurações
│   │   ├── hooks/    # Custom React hooks
│   │   └── ...
├── server/           # Backend Express
│   ├── db.ts         # Configuração do banco de dados
│   ├── dbStorage.ts  # Implementação da camada de armazenamento
│   ├── routes.ts     # Rotas da API
│   └── ...
├── shared/           # Código compartilhado entre frontend e backend
│   └── schema.ts     # Esquema de dados e validação
└── ...
```

## Licença

Este projeto é de código aberto.

## Contato

Para mais informações, entre em contato com a equipe responsável na Prefeitura Municipal de Balneário Camboriú.