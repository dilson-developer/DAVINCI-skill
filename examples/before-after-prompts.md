# Exemplos — Antes / Depois

Cada exemplo mostra o pedido cru do utilizador e o prompt enriquecido gerado pela skill DAVINCI, seguindo o fluxo definido em `SKILL.md`.

---

## Exemplo 1 — SaaS B2B

**Prompt cru:**
> "cria a landing page do meu SaaS de gestão de stock para pequenos negócios"

**Classificação:** SaaS B2B (explícito — "pequenos negócios" + produto de gestão)

**Prompt enriquecido:**
```
Cria uma landing page para um SaaS de gestão de stock para pequenos negócios. Tom direto e factual, focado em eficiência operacional.

1. Hero: headline de resultado (ex: "Nunca mais fiques sem stock a meio da semana"), quebrado em 2 linhas. Subheadline explicando o mecanismo (previsão automática baseada no histórico de vendas). CTA duplo: "Começar grátis" + "Ver demonstração".

2. Faixa de prova social: logos de pequenos negócios clientes, em escala de cinza, logo após o hero.

3. Features: 3-4 blocos (ícone + título de benefício + 1 frase), ex: "Alertas antes de faltar stock", "Relatórios automáticos", "Integração com o teu POS".

4. Testemunhos: 1-2 citações reais de donos de negócio, com nome e nome do negócio.

5. Pricing: 2-3 planos nomeados por escala (Solo/Equipa/Negócio), plano do meio destacado.

6. FAQ: 4-6 perguntas sobre integração, cancelamento e período de teste.

7. CTA final: fundo destacado, botão único, reforço "sem cartão de crédito".

Design: sans-serif geométrica, azul-escuro + um único acento (verde), fundo claro, cantos arredondados consistentes, muito espaço entre secções.
```

---

## Exemplo 2 — AI/Dev Tool

**Prompt cru:**
> "preciso de uma página para a minha API de tradução automática"

**Classificação:** AI Tool / Dev Tool (explícito — API)

**Prompt enriquecido:**
```
Cria uma landing page para uma API de tradução automática, dirigida a developers. Tom confiante e técnico, mas acessível.

1. Hero: headline confiante (ex: "Traduz qualquer texto em 3 linhas de código"), pode citar termos técnicos como prova de categoria. CTA duplo: "Começar grátis" + "Ver documentação".

2. Prova social: logos de empresas que usam a API, ou menção a volume processado.

3. Features: 3-5 blocos tech-forward (latência, número de idiomas, precisão, SDKs disponíveis).

4. Secção de aprofundamento: snippet de código real da integração.

5. Testemunhos: citações técnicas ou métricas de performance.

6. Pricing: planos Free/Pro/Enterprise, baseado em volume de chamadas.

7. FAQ: incluir pergunta sobre limites de uso e compatibilidade com linguagens/frameworks.

8. CTA final: fundo destacado.

Design: dark mode como padrão, gradiente roxo/azul subtil, sans-serif geométrica + elemento mono para código/métricas, acento neon único nos CTAs.
```

---

## Exemplo 3 — SaaS Consumer (sem tipo explícito no pedido)

**Prompt cru:**
> "quero uma página bonita para uma app que ajuda a criar hábitos"

**Classificação:** não explícita — a skill teria de perguntar ao utilizador antes de avançar (ver `SKILL.md`, passo 2). Neste exemplo assume-se que o utilizador respondeu **SaaS Consumer**.

**Prompt enriquecido:** (ver o prompt completo gerado para este caso na resposta principal desta conversa)

---

## Como usar estes exemplos

Ao adicionar um novo padrão de referência ou ajustar uma regra, criar um novo par antes/depois aqui para validar que a mudança produz o resultado esperado — isto funciona como um "teste manual" da skill.
