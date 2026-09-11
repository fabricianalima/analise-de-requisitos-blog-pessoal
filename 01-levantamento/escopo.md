# Especificação de Escopo — Aplicação Blog Pessoal

## 1. Visão Geral do Produto

O Blog Pessoal é uma plataforma web para publicação e gerenciamento
de conteúdos organizados por temas.

A solução é composta por uma API REST desenvolvida em Java/Spring Boot
e uma interface web responsiva desenvolvida em React com TypeScript.

---

## 2. Objetivo do Sistema

Disponibilizar uma plataforma que permita aos usuários cadastrados
gerenciar conteúdos publicados no blog, enquanto visitantes podem
consultar os conteúdos disponibilizados publicamente.

---

## 3. Partes Interessadas

### Visitante / Leitor

Acessa os conteúdos públicos sem necessidade de autenticação.

### Autor / Usuário

Realiza autenticação e gerencia seus próprios conteúdos.

### Administrador

Possui permissões adicionais para gerenciamento do sistema.

### Time de Desenvolvimento

Responsável pela implementação, manutenção e evolução da solução.

> O detalhamento dos stakeholders está disponível em
> [stakeholders.md](../01-levantamento/stakeholders.md).

---

## 4. Escopo do Sistema

### 4.1 Dentro do Escopo

- Cadastro e autenticação de usuários
- Gerenciamento de postagens
- Gerenciamento de temas
- Associação entre postagens e temas
- Consulta de postagens
- Filtro de postagens por título
- Filtro de postagens por tema
- Controle de acesso conforme perfil do usuário

### 4.2 Fora do Escopo

- Integração com redes sociais para publicação automática
- Sistema de comentários
- Monetização do conteúdo
- Sistema de notificações
- Analytics avançado

---

## 5. Principais Entidades

O sistema possui como principais entidades:

- Usuário
- Postagem
- Tema

O modelo de dados detalhado será apresentado na documentação
de modelagem do sistema.

---

## 6. Premissas e Restrições

### Premissas

- Usuários devem estar cadastrados para realizar operações de
  gerenciamento.
- Cada postagem deve estar associada a um tema.
- O acesso às funcionalidades deve respeitar as permissões
  definidas para cada perfil.

### Restrições

- Backend desenvolvido em Java e Spring Boot.
- Frontend desenvolvido em React e TypeScript.
- Comunicação realizada por meio de API REST.
