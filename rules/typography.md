# Regras — Tipografia

## 1. Par de fontes (máximo 2)

- **Display/heading**: uma fonte com personalidade — geométrica (Inter, Manrope, General Sans) para tom técnico/SaaS B2B, ou serifada (Fraunces, Instrument Serif) para tom editorial/premium.
- **Corpo de texto**: sempre uma sans-serif de alta legibilidade (Inter, Manrope, System UI). Nunca usar a mesma fonte de display no corpo se ela for decorativa.
- Nunca mais que 2 famílias tipográficas na página inteira. Um terceiro elemento tipográfico (ex: mono para números/código) é aceitável em produtos técnicos.

## 2. Escala hierárquica

Usar uma escala modular, não valores arbitrários:

| Elemento | Tamanho (rem) | Peso |
|---|---|---|
| Hero headline | 3.5–5.5 | 600–700 |
| Section heading | 2–2.5 | 600 |
| Subheadline / lead | 1.125–1.375 | 400–500 |
| Corpo | 1–1.0625 | 400 |
| Label / caption | 0.75–0.875 | 500 (com letter-spacing +0.02em) |

- A diferença entre hero e section heading deve ser óbvia à primeira vista — se parecem do mesmo tamanho, a hierarquia falhou.

## 3. Comprimento de linha e quebra

- Headlines: quebrar manualmente em 2–3 linhas curtas, nunca deixar o browser quebrar sozinho um headline de mais de 6 palavras.
- Corpo de texto: 45–75 caracteres por linha (max-width ~60ch).
- Parágrafos de feature/benefício: 1 frase, no máximo 2. Se precisar de mais, é sinal de que o benefício não está claro.

## 4. Peso e contraste

- Nunca usar peso 300 (light) para texto abaixo de 18px — falha em telas de baixa qualidade e em modo escuro.
- Título principal sempre em contraste máximo com o fundo; texto secundário pode reduzir opacidade (70–80%) mas nunca abaixo de 60%.

## 5. Quando usar serif vs sans

- Serif no hero → sinaliza confiança, produto maduro, preço mais alto (ex: consultoria, educação premium).
- Sans-serif geométrica no hero → sinaliza velocidade, tech, produto self-serve (ex: dev tools, dashboards).
- Produtos de IA/dados: sans-serif com um elemento mono (para métricas, código, dados) reforça credibilidade técnica.
