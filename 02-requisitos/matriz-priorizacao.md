**Matriz de Priorização e Rastreabilidade**

**Classificação MoSCoW**

- **Must Have (Essencial):** Autenticação, CRUD de Postagens e CRUD de Temas.
- **Should Have (Importante):** Filtro de busca por título de postagem e por nome do tema.
- **Could Have (Desejável):** Paginação customizada de postagens na interface e modo escuro no frontend.
- **Won't Have (Fora do escopo atual):** Integração com redes sociais para publicação automática.

| ID Requisito | Descrição               | Regra de Negócio (RN) | Categoria MoSCoW | Componente Backend (Spring)                              | Componente Frontend (React)      |
| :----------- | :---------------------- | :-------------------- | :--------------- | :------------------------------------------------------- | :------------------------------- |
| **RF001**    | Autenticação de Usuário | RN001                 | Must Have        | `UsuarioController`, `UsuarioService`                    | `Login.tsx`, `AuthContext.tsx`   |
| **RF006**    | Gerenciamento de Temas  | RN002, RN003, RN004   | Must Have        | `TemaController`, `TemaRepository`                       | `FormTema.tsx`, `ListaTemas.tsx` |
| **RF007**    | Filtro por Título       | N/A                   | Should Have      | `PostagemRepository.findAllByTituloContainingIgnoreCase` | `BuscaPostagem.tsx`              |
