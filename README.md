# Symfony API com MFA e JWT (Projeto em Desenvolvimento)

Este projeto é uma API construída com Symfony 6 que fornece funcionalidades de registro de usuário e autenticação com MFA (Multi-Factor Authentication) e JWT (JSON Web Token). A aplicação é containerizada usando Docker e Docker Compose.

## Tecnologias Utilizadas

- **PHP 8.3**
- **Symfony 7**
- **PostgreSQL**
- **pgAdmin**
- **Docker**
- **Docker Compose**

## Pré-requisitos

Certifique-se de ter o Docker e o Docker Compose instalados na sua máquina.

- [Docker](https://docs.docker.com/get-docker/)
- [Docker Compose](https://docs.docker.com/compose/install/)


## Configuração do Ambiente

1. **Clone o repositório:**

   ```bash
   git clone https://github.com/seu-usuario/seu-repositorio.git
   cd seu-repositorio
   ```


2. **Copie o arquivo .env.example para .env:**

   ```bash
   cp ./symfony/.env.example ./symfony/.env
   ```


3. **Inicie os containers Docker:**

   ```bash
   docker-compose up --build
   ```

4. **Acesse a aplicação**

   * Symfony: http://localhost:8080
   * pgAdmin: http://localhost:5050


## Estrutura do projeto

project-root/
├── docker-compose.yml
├── apache/
│   ├── Dockerfile
│   └── 000-default.conf
├── symfony/
│   ├── Dockerfile
│   ├── .env
│   ├── .env.example
│   └── ... (outros arquivos do Symfony)
└── pgadmin/
    └── Dockerfile

