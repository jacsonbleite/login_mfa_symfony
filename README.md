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
   git clone https://github.com/jacsonbleite/login_mfa_symfony.git
   cd login_mfa_symfony
   ```

2. **Copie o arquivo .env.example para .env e preencha-o:**
   
   ```bash
   cp ./symfony/.env.example ./symfony/.env
   ```

3. **Inicie o projeto:**
   
   1. **Primeira execução**
   
   ```bash
   docker-compose up --build
   ```
   
   2. **Nas próximas**
   
   ```bash
   docker-compose up -d
   ```

4. **Acesse a aplicação**
   
   * Symfony: http://localhost:8080
   * pgAdmin: http://localhost:5050

## Estrutura do projeto

```
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
```
