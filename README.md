# DAVINCI

> Uma skill de design para vibecoders. DAVINCI transforma um pedido simples ("cria a landing page do meu SaaS") num briefing de design rico e estruturado, pronto para ser executado por qualquer agente de código — Claude Code, Cursor, ou outro.

## O problema

Vibecoders constroem MVPs rápido, mas o design das landing pages sai genérico: hero sem hierarquia, features em parágrafo, zero prova social, CTA perdido no meio da página. O agente de código faz o que se pede — o problema é que o pedido em si raramente contém boas decisões de design.

## A ideia

DAVINCI não é mais um gerador com LLM por trás. É uma **skill baseada em regras e templates**: recebe uma descrição curta do produto, identifica o tipo de SaaS, e devolve um prompt enriquecido — com estrutura de secções, hierarquia de copy, e princípios de design já aplicados — que qualquer agente de IA pode executar diretamente.

```
Prompt cru:
"landing page para o meu SaaS de gestão de stock"

        ↓ DAVINCI aplica regras + templates ↓

Prompt enriquecido:
Hero com headline focado em resultado (não em feature),
subheadline de mecanismo, CTA duplo (primário + secundário),
faixa de prova social com números concretos logo abaixo,
grid de 4 features (ícone + título curto + 1 frase de benefício),
paleta de gradiente suave, cards com cantos arredondados...
```

## Como funciona

1. **Input** — o utilizador descreve o produto em 1-2 frases
2. **Classificação** — DAVINCI identifica o tipo de página (SaaS B2B, SaaS Consumer, AI Tool ou Fintech). Se não estiver claro no pedido, a skill **pergunta ao utilizador** em vez de assumir silenciosamente.
3. **Aplicação de regras** — princípios de tipografia, cor, layout e copywriting são combinados com templates de secção
4. **Output** — um prompt estruturado e específico, pronto para colar em qualquer assistente de código

Sem chamadas a APIs externas de LLM. Sem dependências pesadas. Determinístico e auditável.

## Estrutura do projeto

```
design-DAVINCI/
├── SKILL.md                   # ponto de entrada — como e quando a skill é ativada,
│                               #  inclui o passo interativo de classificação
├── rules/                     # princípios de design em texto
│   ├── typography.md
│   ├── color-systems.md
│   ├── layout-grids.md
│   └── copywriting.md
├── templates/
│   ├── sections/               # blocos reutilizáveis (hero, features, pricing,
│   │                           #  testimonials, faq, cta)
│   └── page-types/             # combinações completas por tipo de produto
│       ├── saas-b2b.md
│       ├── saas-consumer.md
│       ├── ai-tool.md
│       └── fintech.md
├── references/
│   └── design-patterns.md      # padrões extraídos de referências reais de landing pages
├── examples/
│   └── before-after-prompts.md
└── docs/
    └── architecture.md
```

## Para quem é

Vibecoders e independent hackers que constroem MVPs de SaaS rapidamente com IA e querem que a primeira versão da landing page já nasça com boas decisões de design — sem precisar contratar um designer.

## Contribuir

Este projeto está em fase inicial. Issues e PRs com novas referências, regras de design ou templates de secção são bem-vindos.
