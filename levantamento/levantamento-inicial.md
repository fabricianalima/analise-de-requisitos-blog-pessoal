# Registro de Elicitação de Requisitos (Levantamento)

## 1. Informações da Sessão

- **Data:** 10/09/2026
- **Técnica Utilizada:** Entrevista Semiestruturada / Workshop de Alinhamento
- **Participantes:** Analista de Sistemas, Product Owner (PO), Especialista de Negócio

## 2. Necessidades Identificadas (Notas Brutas)

- O cliente precisa de um painel web rápido para gerenciar os artigos do blog sem depender do time de TI.
- É necessário garantir que usuários não autorizados não consigam deletar ou editar artigos de terceiros.
- O sistema deve suportar acesso via navegadores modernos (Chrome, Firefox, Edge) e dispositivos móveis (design responsivo).
- Para o backend, há preferência pelo uso de Java com Spring Boot devido à infraestrutura existente na empresa.

## 3. Insumos para Análise

- **Candidato a RF:** Sistema de autenticação com permissões por perfil (Autor vs. Administrador).
- **Candidato a RNF:** Interface React adaptável a diferentes tamanhos de tela (Responsividade).
- **Candidato a RN:** Validação de propriedade do post antes de permitir ações de atualização ou exclusão.
