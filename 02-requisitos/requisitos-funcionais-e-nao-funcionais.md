# Requisitos do Sistema

## Requisitos Funcionais (RF)

### RF001 — Autenticação de Usuário

O sistema deve permitir o login de usuários cadastrados
utilizando e-mail e senha.

### RF002 — Criar Postagem

O sistema deve permitir que usuários autorizados criem
postagens vinculadas a um tema.

### RF003 — Editar Postagem

O sistema deve permitir que usuários autorizados editem
suas próprias postagens.

### RF004 — Listar Postagens

O sistema deve permitir a consulta das postagens cadastradas.

### RF005 — Excluir Postagem

O sistema deve permitir a exclusão de postagens conforme
as permissões do usuário.

### RF006 — Gerenciamento de Temas

O sistema deve permitir a criação, listagem, alteração
e exclusão de temas.

### RF007 — Filtro por Título

O sistema deve permitir a busca de postagens por palavras-chave
contidas no título.

### RF008 — Filtro por Tema

O sistema deve permitir a filtragem de postagens por tema.

## Requisitos Não Funcionais (RNF)

### RNF001 — Segurança

A comunicação entre cliente e servidor deve utilizar HTTPS.
Os endpoints que exigem autenticação devem possuir controle
de acesso baseado nas permissões do usuário.

### RNF002 — Tempo de Resposta

As chamadas de leitura da API devem apresentar tempo de
resposta inferior a 300 ms em condições normais de uso.

## Restrições Técnicas (RT)

### RT001 — Backend

A API REST deve ser implementada utilizando Java 17+
e Spring Boot.

### RT002 — Frontend

A interface deve ser desenvolvida utilizando React,
TypeScript e React Router.
