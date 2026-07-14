---
name: davinci
description: Usar esta skill sempre que o utilizador pedir para criar, melhorar ou desenhar uma landing page, página de vendas, ou website para um produto SaaS/MVP. Transforma uma descrição crua do produto num prompt estruturado e rico em decisões de design, usando regras e templates determinísticos — sem chamar nenhuma LLM externa. Aciona-se com pedidos como "cria a landing page do meu SaaS", "melhora o design do meu site", "página de vendas para o meu produto".
---

# DAVINCI — Skill de Design para Landing Pages

## Fluxo de execução

### 1. Ler o pedido cru do utilizador

Extrair: o que o produto faz, para quem é, e (se mencionado) o tipo de página.

### 2. Classificar o tipo de página — PASSO OBRIGATÓRIO E INTERATIVO

Verificar se o utilizador já indicou claramente um destes tipos:

- **SaaS B2B** — produto de gestão/dados/infraestrutura vendido a empresas
- **SaaS Consumer** — produto usado por indivíduos (produtividade pessoal, bem-estar, social, criativo)
- **AI Tool / Dev Tool** — ferramenta técnica, API, ou produto de IA para developers/equipas técnicas
- **Fintech** — produto financeiro (pagamentos, banca, investimento)

**Se o tipo não estiver claro no pedido, PARAR e perguntar ao utilizador antes de continuar.** Nunca assumir silenciosamente. Exemplo de pergunta:

> "Que tipo de produto é este? (a) SaaS B2B — vendido a empresas (b) SaaS Consumer — para uso pessoal (c) AI/Dev Tool — ferramenta técnica (d) Fintech — produto financeiro"

Só avançar depois de ter a resposta. Se o utilizador der contexto suficiente para inferir com confiança (ex: "app de gestão financeira pessoal para milhares de utilizadores" → SaaS Consumer, tom próximo de Fintech), pode assumir e dizer explicitamente qual assumiu, dando ao utilizador a opção de corrigir — nunca assumir em silêncio sem mencionar.

### 3. Carregar o template do tipo de página

Ler o ficheiro correspondente em `templates/page-types/`:
- `saas-b2b.md`
- `saas-consumer.md`
- `ai-tool.md`
- `fintech.md`

Este ficheiro define a ordem de secções e as regras específicas do tipo (tom, cor, tipografia).

### 4. Montar as secções

Para cada secção listada no template do tipo, ler o ficheiro correspondente em `templates/sections/` (`hero.md`, `features.md`, `pricing.md`, `testimonials.md`, `faq.md`, `cta.md`) e preencher os placeholders com a informação do produto.

### 5. Aplicar as regras transversais

Consultar `rules/typography.md`, `rules/color-systems.md`, `rules/layout-grids.md` e `rules/copywriting.md` conforme referenciado em cada template de secção — as referências cruzadas (ex: `[rules/copywriting.md #1]`) indicam exatamente qual regra aplicar em cada ponto.

### 6. Gerar o output

Produzir um único prompt estruturado, na língua do utilizador, pronto para ser colado em qualquer agente de código (Claude Code, Cursor, v0, etc.) para gerar a página real.

## Regras de segurança do conteúdo

- Nunca inventar métricas, testemunhos ou logos de clientes — se não existirem dados reais, usar as alternativas descritas em `templates/sections/testimonials.md`.
- Nunca pular o passo 2 (classificação) mesmo que o utilizador peça pressa — é a decisão que mais influencia todas as seguintes.

## Ficheiros desta skill

```
SKILL.md                        ← este ficheiro
rules/                          ← princípios de design (tipografia, cor, layout, copy)
templates/sections/             ← blocos reutilizáveis (hero, features, pricing...)
templates/page-types/            ← combinações completas por tipo de produto
references/design-patterns.md   ← padrões extraídos de referências reais
```
