# Regras — Layout e Grid

## 1. Ordem canónica de secções

Esta é a ordem-padrão observada nas referências (desviar só com razão específica):

1. Nav (logo + 3-5 links + CTA)
2. Hero (headline + subheadline + CTA duplo)
3. Faixa de prova social (logos ou números)
4. Grid de features (3-5 blocos)
5. Secção de aprofundamento (1-2 features "hero" com mais detalhe/imagem)
6. Prova social aprofundada (testemunhos ou caso antes/depois)
7. Pricing (se aplicável)
8. FAQ
9. CTA final (repete o CTA do hero, standalone, fundo destacado)
10. Footer

## 2. Espaçamento

- Escala de espaçamento em múltiplos de 8px (8, 16, 24, 32, 48, 64, 96, 128).
- Espaço entre secções: mínimo 64px em mobile, 96–128px em desktop. Secções coladas sem respiro são o erro nº1 de MVP.
- Padding lateral: nunca conteúdo colado à borda — mínimo 24px mobile, 5-8% da largura em desktop.

## 3. Grid de conteúdo

- Largura máxima de conteúdo: 1200–1280px, centrado. Fundos/gradientes podem esticar full-bleed, texto nunca.
- Grid de features: 3 colunas desktop / 1 coluna mobile é o padrão seguro. 4 colunas só se os blocos forem muito curtos (ícone + título, sem descrição).
- Cards: gap mínimo de 24px entre eles, nunca encostados.

## 4. Hierarquia visual por posição

- O primeiro elemento visível (above the fold) deve conter: headline, subheadline, CTA. Nada mais. Se a screenshot da hero section tem mais de 3 elementos de texto, está sobrecarregada.
- Imagens/screenshots de produto: sempre depois do CTA, nunca antes — o texto vende primeiro, a imagem confirma.

## 5. Responsividade

- Mobile-first: grid de features colapsa para 1 coluna, nav colapsa para hambúrguer, hero reduz headline para 2 linhas máximo.
- CTAs em mobile: full-width dentro do padding, nunca do tamanho do texto.

## 6. Cards e cantos

- Border-radius consistente em toda a página: 8-12px para elementos pequenos (botões, badges), 16-24px para cards e imagens grandes. Nunca misturar dois raios diferentes na mesma família de elementos.
