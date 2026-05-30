# Sistema PayAll

> **Plataforma de Pagamentos Inteligentes para o Futuro**

---

## Descrição do Sistema

O **PayAll** é uma plataforma de pagamentos digitais desenvolvida para facilitar transações financeiras entre pessoas físicas e jurídicas de forma rápida, segura e acessível.

O sistema permite que empresas e desenvolvedores integrem soluções de pagamento em seus produtos por meio de uma API robusta e bem documentada. Com o PayAll, é possível processar cobranças via Pix, cartão de crédito, boleto bancário e carteiras digitais em um único lugar.

O PayAll resolve o problema da fragmentação de meios de pagamento, eliminando a necessidade de contratar múltiplos gateways. Ele é utilizado por e-commerces, fintechs, startups e pequenos negócios que precisam de uma solução confiável e escalável.

---

## Tecnologias Utilizadas

| Categoria         | Tecnologia         |
|-------------------|--------------------|
| Linguagem         | TypeScript (Node.js) |
| Framework         | NestJS             |
| Banco de Dados    | PostgreSQL          |
| Cache             | Redis              |
| Autenticação      | JWT + OAuth 2.0    |
| Ferramenta CI/CD  | GitHub Actions     |
| Containerização   | Docker / Docker Compose |

---

## Como Executar o Projeto

### Pré-requisitos

- Node.js >= 18.x
- Docker e Docker Compose
- Git

### Instalação

```bash
# Clone o repositório
git clone https://github.com/payall/payall-core.git

# Acesse a pasta do projeto
cd payall-core

# Instale as dependências
npm install

# Configure as variáveis de ambiente
cp .env.example .env
```

### Rodando com Docker

```bash
# Suba os containers (banco, cache e aplicação)
docker-compose up -d

# Acesse a aplicação em:
# http://localhost:3000
```

### Rodando localmente (sem Docker)

```bash
# Inicie o banco de dados PostgreSQL e Redis manualmente, depois:
npm run start:dev
```

### Rodando os testes

```bash
# Testes unitários
npm run test

# Testes de integração
npm run test:e2e

# Cobertura de testes
npm run test:cov
```

---

## Estrutura de Pastas

```
payall-core/
├── src/           # Código-fonte principal da aplicação
├── docs/          # Documentação técnica e contratos de API (Swagger)
├── tests/         # Testes unitários e de integração (e2e)
├── docker/        # Arquivos de configuração Docker
├── scripts/       # Scripts utilitários de automação
└── .github/       # Configurações de CI/CD com GitHub Actions
```

- **`src/`** — Contém os módulos, controladores, serviços e entidades da aplicação.
- **`docs/`** — Documentação da API no formato OpenAPI/Swagger e guias de integração.
- **`tests/`** — Suítes de testes automatizados para garantir qualidade e cobertura de código.

---

## Links

- Site oficial: [https://www.payall.com.br](https://www.payall.com.br)
- Repositório: [https://github.com/SamuelRMagro/sistema-payall](https://github.com/SamuelRMagro/sistema-payall)
- Documentação da API: [https://docs.payall.com.br](https://docs.payall.com.br)

---

## Funcionalidades Principais

- Processamento de pagamentos via **Pix**, **cartão de crédito** e **boleto**
- **Dashboard** com relatórios financeiros em tempo real
- **API RESTful** com documentação Swagger integrada
- Sistema de **split de pagamentos** entre múltiplos recebedores
- **Webhooks** para notificações automáticas de transações
- Suporte a **múltiplas moedas** e conversão automática

---

## Equipe

| Nome | RGM |
|------|-----|
| Samuel Rodrigues Magro | 114.021 |

---

*PayAll © 2025 — Todos os direitos reservados.*
