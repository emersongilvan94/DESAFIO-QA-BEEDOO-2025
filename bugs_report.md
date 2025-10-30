# Relatório de Bugs – Beedoo Challenge 2025

## Bug 01 – Curso não é removido da lista após exclusão
**Severidade:** Alta  
**Status:** Aberto  
**Tipo:** Funcional  
**Descrição:** Ao excluir um curso, o sistema exibe a mensagem “Curso excluído com sucesso”, mas o curso permanece na listagem após atualizar a página.  
**Passos para reproduzir:**
1. Criar um curso qualquer.  
2. Acessar “Listar Cursos”.  
3. Clicar em “Excluir”.  
4. Atualizar a página.  
**Resultado Esperado:** Curso removido permanentemente da lista.  
**Resultado Obtido:** Curso ainda aparece na listagem.  
**Impacto:** Dados inconsistentes e falha na exclusão efetiva do curso.

---

## Bug 02 – Sistema permite criar curso sem preencher campos obrigatórios
**Severidade:** Alta  
**Status:** Aberto  
**Tipo:** Validação  
**Descrição:** O sistema permite cadastrar cursos sem preencher campos obrigatórios como nome, descrição ou datas.  
**Passos para reproduzir:**
1. Acessar “Cadastrar Curso”.  
2. Deixar campos obrigatórios em branco.  
3. Clicar em “Cadastrar Curso”.  
**Resultado Esperado:** Sistema deve exibir mensagens de erro e impedir o cadastro.  
**Resultado Obtido:** Curso é criado mesmo com campos vazios.  
**Impacto:** Pode gerar dados incompletos e inconsistentes no sistema.

---

## Bug 03 – Datas inválidas aceitas (data final anterior à inicial)
**Severidade:** Alta  
**Status:** Aberto  
**Tipo:** Validação  
**Descrição:** É possível cadastrar um curso com data de fim anterior à data de início.  
**Passos para reproduzir:**
1. Definir data inicial = 01/11/2025.  
2. Definir data final = 01/10/2025.  
3. Clicar em “Cadastrar Curso”.  
**Resultado Esperado:** Sistema deve exibir mensagem de erro e bloquear o cadastro.  
**Resultado Obtido:** Curso criado com datas inválidas.  
**Impacto:** Pode gerar confusão na exibição e controle de cursos.

---

## Bug 04 – Campo “Link de inscrição” não é obrigatório em cursos online
**Severidade:** Média  
**Status:** Aberto  
**Tipo:** Validação  
**Descrição:** O sistema permite criar cursos do tipo “Online” sem informar o link de inscrição.  
**Passos para reproduzir:**
1. Acessar “Cadastrar Curso”.  
2. Selecionar tipo “Online”.  
3. Deixar o campo “Link de inscrição” em branco.  
4. Clicar em “Cadastrar Curso”.  
**Resultado Esperado:** Exibir erro informando que o link é obrigatório.  
**Resultado Obtido:** Curso é criado normalmente.  
**Impacto:** Usuários não conseguem se inscrever, causando quebra no fluxo.

---

## Bug 05 – Falta de botão para retornar à tela inicial
**Severidade:** Baixa  
**Status:** Aberto  
**Tipo:** Navegação  
**Descrição:** Após cadastrar ou listar cursos, não há opção visível para retornar à tela inicial.  
**Passos para reproduzir:**
1. Cadastrar ou listar um curso.  
2. Procurar opção “Voltar” ou “Home”.  
**Resultado Esperado:** Botão ou link para retornar à tela inicial.  
**Resultado Obtido:** Usuário fica limitado às opções de “Cadastrar” ou “Listar Cursos”.  
**Impacto:** Dificulta a navegação e a experiência do usuário.
