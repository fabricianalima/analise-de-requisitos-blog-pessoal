**Mapeamento de Stakeholders e Regras de Negócio**

**Partes Interessadas (Stakeholders)**

- **Visitante:** Usuário não autenticado que pode visualizar listagens e detalhes das postagens públicas.
- **Autor/Usuário Autenticado:** Usuário logado responsável por criar, atualizar e remover o seu próprio conteúdo de postagens.
- **Administrador:** Responsável pela moderação global das postagens e gestão dos temas cadastrados na plataforma.
- **Time de Desenvolvimento/Manutenção:** Responsável pelo suporte técnico, implementação de novas features e evolução da infraestrutura.

**Regras de Negócio (RN)**

- **[RN001] Unicidade de Usuário:** Não é permitido o cadastro de dois usuários com o mesmo endereço de e-mail na base de dados.
- **[RN002] Validação de Título e Texto:** O título da postagem deve ter no mínimo 5 caracteres e o texto da postagem no mínimo 10 caracteres.
- **[RN003] Vínculo Obrigatório com Tema:** Toda postagem deve obrigatoriamente estar associada a pelo menos um Tema previamente cadastrado no sistema.
- **[RN004] Autorização de Alteração:** Um usuário só possui permissão para editar ou deletar postagens das quais seja o autor original, exceto perfis com papel de Administrador.
