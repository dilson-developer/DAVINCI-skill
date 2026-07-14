# Template — Hero

Usar como bloco inicial de qualquer prompt gerado. Preencher os placeholders com base no input do utilizador e na classificação do produto (ver `templates/page-types/`).

```
Secção: Hero
- Headline: {{resultado_desejado}}, sem {{fricção_habitual}}. Máx. 8-10 palavras, quebrado em 2-3 linhas.
  Formato: [rules/copywriting.md #1]
- Subheadline: 1 frase explicando o mecanismo — como {{headline}} acontece na prática.
- CTA primário: verbo de ação + objeto claro (ex: "Começar grátis")
- CTA secundário: ação de baixo compromisso (ex: "Ver demonstração")
- Tipografia: headline 3.5-5.5rem, peso 600-700 [rules/typography.md #2]
- Fundo: {{paleta_do_tipo_de_produto}} — ver rules/color-systems.md #6
- Sem imagem de produto nesta secção — texto vende primeiro [rules/layout-grids.md #4]
```

## Variantes por tom

- **B2B/dados**: headline factual, foco em eficiência/ROI. Ex.: "Toda a tua operação, numa só vista."
- **AI/dev tool**: headline confiante, pode incluir termo técnico como prova de categoria. Ex.: "Deploy em minutos, não em sprints."
- **Consumer/pessoal**: headline pode ser mais poética/emocional, CTA único em vez de duplo. Ver caso Interlude em `references/design-patterns.md`.
