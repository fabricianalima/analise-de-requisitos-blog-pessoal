**Matriz de Priorização e Rastreabilidade**

**Classificação MoSCoW**

- **Must Have (Essencial):** Autenticação JWT, CRUD de Postagens e CRUD de Temas.
- **Should Have (Importante):** Filtro de busca por título de postagem e por nome do tema.
- **Could Have (Desejável):** Paginação customizada de postagens na interface e modo escuro no frontend.
- **Won't Have (Fora do escopo atual):** Integração com redes sociais para publicação automática.

| ID Requisito | Descrição                  | Regra de Negócio (RN) | Categoria MoSCoW | Componente Backend (Spring)                              | Componente Frontend (React)              |
| :----------- | :------------------------- | :-------------------- | :--------------- | :------------------------------------------------------- | :--------------------------------------- |
| **RF001**    | Autenticação de Usuário    | RN001                 | Must Have        | `UsuarioController`, `UsuarioService`                    | `Login.tsx`, `AuthContext.tsx`           |
| **RF002**    | Gerenciamento de Postagens | RN002, RN003, RN004   | Must Have        | `PostagemController`, `PostagemRepository`               | `FormPostagem.tsx`, `ListaPostagens.tsx` |
| **RF003**    | Filtro por Título          | N/A                   | Should Have      | `PostagemRepository.findAllByTituloContainingIgnoreCase` | `BuscaPostagem.tsx`                      |
