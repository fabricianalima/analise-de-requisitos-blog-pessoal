# Especificação de Escopo: Aplicação Blog Pessoal

## 1. Visão Geral do Produto

O **Blog Pessoal** é uma plataforma web para publicação de artigos e gerenciamento de conteúdos organizados por temas[cite: 2, 3]. A solução é dividida em um backend em API REST Java/Spring Boot e uma interface SPA responsiva construída em React com TypeScript.

---

## 2. Partes Interessadas (Stakeholders)

- **Visitante / Leitor:** Acessa conteúdos públicos sem necessidade de autenticação.
- **Autor / Usuário Cadastrado:** Realiza autenticação no sistema para criar e gerenciar seus próprios textos e temas.
- **Time de Engenharia de Software:** Responsável pelo desenvolvimento, manutenção da API REST[cite: 3] e versionamento dos artefatos técnicos no GitHub.

---

## 3. Modelo de Dados / Entidades (DER)

A aplicação baseia-se em três entidades fundamentais: **USUARIO**, **POSTAGEM** e **TEMA**.

```mermaid
erDiagram
    USUARIO ||--o{ POSTAGEM : escreve
    TEMA ||--o{ POSTAGEM : classifica

    USUARIO {
        bigint id PK
        varchar(255) nome
        varchar(255) usuario
        varchar(255) senha
        varchar(5000) foto
    }

    POSTAGEM {
        bigint id PK
        varchar(100) titulo
        varchar(1000) texto
        datetime data
        bigint tema_id FK
        bigint usuario_id FK
    }

    TEMA {
        bigint id PK
        varchar(255) descricao
    }
```
