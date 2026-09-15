# Agente de Estudos

Assistente pessoal para gerenciamento de tarefas acadêmicas, acessível tanto por uma API REST quanto por um agente de linguagem natural via **MCP (Model Context Protocol)**.

## Objetivo

Este projeto foi criado para aplicar, na prática, conceitos de desenvolvimento backend, APIs, autenticação e agentes de IA — em especial o Model Context Protocol, permitindo que um modelo de linguagem (como o Claude) consulte e gerencie minhas tarefas de faculdade através de linguagem natural, em vez de uma interface tradicional.

## Como funciona

O sistema mantém um banco de dados MySQL com as tarefas (título, matéria, prazo, status). Essas informações podem ser acessadas de duas formas:

- **Via API REST** — endpoints tradicionais para criar, listar, editar e excluir tarefas.
- **Via servidor MCP** — as mesmas operações expostas como "ferramentas" que um cliente MCP (ex: Claude Desktop) pode chamar, permitindo perguntas como *"quais tarefas de Banco de Dados eu tenho essa semana?"*.

## Tecnologias

- **Python**
- **FastAPI** — API REST
- **MySQL** — banco de dados relacional (persistência das tarefas)
- **JWT** — autenticação de usuários
- **MCP SDK (Anthropic)** — servidor MCP com ferramentas para o agente
- **Docker** — containerização do ambiente

## Status atual

- [ ] API REST com CRUD de tarefas
- [ ] Modelagem do banco de dados (tarefas, matérias, prazos)
- [ ] Autenticação de usuários via JWT
- [ ] Servidor MCP expondo as operações como ferramentas
- [ ] Containerização com Docker

*(Esta seção será atualizada conforme o desenvolvimento avança.)*

## Motivação

Projeto pessoal desenvolvido para aprofundar conhecimentos em desenvolvimento backend, integração de APIs e agentes de IA, com foco em Model Context Protocol.
