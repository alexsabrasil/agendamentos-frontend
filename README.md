# Sistema de Agendamentos | Front-end

Aplicação web para gerenciamento de agendamentos, desenvolvida com React, TypeScript e Vite, conteinerizada com Docker e publicada no Render.

## Aplicação em produção

[Acessar o sistema](https://agendamentos-frontend-fkxd.onrender.com)

## Tecnologias

- React 19, TypeScript e Vite 8
- Tailwind CSS
- Nginx e Docker
- Git, GitHub e Docker Hub
- Render

## Funcionalidades

- Cadastro e visualização de agendamentos
- Alteração de status, cancelamento e conclusão
- Filtros por status e período
- Indicadores de agendamentos
- Integração com API REST e PostgreSQL

## Arquitetura

**React + TypeScript → API REST (Node.js/Express) → PostgreSQL**

O front-end é compilado com Vite e disponibilizado por Nginx em um contêiner Docker.

## Execução local

Instale as dependências com `npm ci` e inicie o servidor com `npm run dev`.

Configure a variável `VITE_API_URL` em um arquivo `.env` para apontar para a API local.

## Docker

Construa a imagem com `docker build -t agendamentos-frontend:v1 .`.

Execute com `docker run -d --name agendamentos-frontend -p 8080:80 agendamentos-frontend:v1`.

Acesse `http://localhost:8080`.

## Testes realizados

Foram validados o build de produção, a inicialização do Nginx, o health check e a integração com a API. Também foram realizados testes manuais de cadastro, alteração de status, cancelamento, conclusão e persistência dos registros após atualização da página.

## Links

- [Aplicação publicada](https://agendamentos-frontend-fkxd.onrender.com)
- [API no GitHub](https://github.com/alexsabrasil/api-agendamentos)
- [Imagem Docker](https://hub.docker.com/r/alexsasec/agendamentos-frontend)
- [Documentação Swagger](https://api-agendamentos-flpb.onrender.com/api-docs)

## Melhorias futuras

Automatização do pipeline CI/CD, testes de interface, autenticação, monitoramento e verificações de segurança.

## Contexto acadêmico

Projeto desenvolvido e adaptado durante atividades práticas de DevOps, com foco em conteinerização, hospedagem e integração entre serviços.