# DESAFIO QA BEEDOO 2025

Este repositório contém a documentação e artefatos do desafio de QA Júnior.

## Links da Entrega
- **Aplicação (módulo Cursos)**: https://creative-sherbet-a51eac.netlify.app/
- **Planilha (Casos de Teste)**: _cole aqui o link público do Google Sheets_
- **Evidências (MP4) – Drive**: _cole aqui o link público da pasta_
- **User Story (Markdown)**: ./user_story.md
- **Relatório de Bugs**: _opcional: ./bugs_report.md_

## Metodologia
- **Padrão de documentação**: IEEE 829 (simplificado) para clareza e rastreabilidade.
- **Abordagem de testes**: Testes manuais funcionais + sessões curtas de **teste exploratório**.
- **Critérios de saída**: Fluxo feliz validado; casos críticos cobertos; bugs P1 resolvidos; evidências anexadas.

## Como foram tomadas as decisões da User Story
1. **Fonte**: análise do módulo público (link acima) com foco nas ações _Cadastrar_, _Listar_ e _Excluir_ cursos.
2. **Premissas**: campos observados no formulário (Nome, Descrição, Datas, Tipo, Endereço/Link, URL da imagem) e comportamento condicional por **Tipo** (Online vs Presencial).
3. **Critérios de aceite**: definidos para garantir **validações mínimas**, **mensagens claras** e **persistência real** nas operações.
4. **Cobertura**: incluímos testes **positivos** (sucesso) e **negativos** (erros/validações), além de casos “fora da caixa” (clique duplo, XSS básico).
5. **Evidências**: vídeos MP4 curtos por fluxo principal para facilitar verificação pelo avaliador.

## Estrutura
```
.
├── README.md
├── user_story.md
└── casos_de_teste_cursos.csv   # CSV para importar no Google Sheets
```
