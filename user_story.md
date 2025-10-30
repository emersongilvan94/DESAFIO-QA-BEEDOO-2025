# User Story — Módulo de Cursos (Beedoo QA Challenge)

**Como** administrador/gestor de conteúdo  
**Quero** cadastrar, listar e excluir cursos (presencial e online)  
**Para** manter o catálogo atualizado e acessível aos alunos.

## Contexto e Decisões
- A tela possui ações **LISTAR CURSOS** e **CADASTRAR CURSO**. O formulário inclui **Nome do curso**, **Descrição**, **Datas (início/fim)**, **Tipo do curso (Presencial/Online)**, **Endereço** (para Presencial), **Link de inscrição** (para Online) e **URL da imagem de capa**.
- Decidimos tratar **validações mínimas obrigatórias**: campos essenciais não devem ficar vazios; datas devem ser consistentes (*início ≤ fim*); quando **Online**, o **Link de inscrição** deve ser **obrigatório** e em **formato de URL**; quando **Presencial**, **Endereço** deve ser **obrigatório**.
- Incluímos critérios para **feedback claro ao usuário**, **prevenção de duplicidade** (clique duplo) e **persistência real** das operações (criar/excluir refletindo na listagem após recarregar).

## Critérios de Aceite (alto nível)
1. É possível **cadastrar** curso com dados válidos → exibir **mensagem de sucesso** e o curso aparece em **Lista de cursos**.
2. **Validações**:
   - Campos obrigatórios não podem ser vazios (Nome; e os condicionais conforme o Tipo).
   - **Datas**: _data de início_ não pode ser maior que _data de fim_.
   - **Online**: exige **Link de inscrição** em formato `http(s)://...`.
   - **Presencial**: exige **Endereço**.
3. **Excluir curso**: requer confirmação; após confirmar, item não deve constar na **Lista** (mesmo após recarregar).
4. **UX**: mensagens claras; botão **Cadastrar** desabilitado até o formulário ficar válido; impedir **criação duplicada** por clique duplo.

## Definition of Done (DoD)
- Casos de teste (sucesso + erro) executados e evidenciados (MP4).
- Bugs P1 resolvidos ou claramente documentados.
- Planilha (Google Sheets) e README atualizados com links.
- User Story e decisões acessíveis no repositório.
