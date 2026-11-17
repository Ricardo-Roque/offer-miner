# Padrão de evidências e classificação

## Regras mínimas

- Cada oferta deve conter **uma URL de produto/marca verificável**, data de acesso e identificação de mercado.
- Cada alegação sobre preço, criativo, promoção, duração, ingrediente ou anúncio deve apontar a evidência correspondente.
- A evidência deve descrever **o que foi observado**, não a inferência.
- URLs inacessíveis são registradas como `unverified` com motivo; não inventar a visualização.
- Ao comparar mercados, diferenciar fonte local, importação e apenas presença de idioma.
- Um resultado insuficiente é melhor que preencher campos vazios de maneira especulativa.

## Estados

| Estado | Condição |
|---|---|
| descoberta | produto e fonte identificados |
| sinais_de_atividade | atividade comercial observada |
| evidencia_de_tracao | múltiplos sinais independentes, mas sem garantia de vendas |
| validacao_comercial_comprovada | prova explícita e conferível de performance/vendas |

**Anúncio ativo ≠ ROAS positivo.** Número de criativos ≠ gasto. Tempo em veiculação ≠ lucratividade. Avaliações públicas podem ser manipuladas ou não representar volume real de vendas.

## Prioridade de investigação

A prioridade (`prioridade_alta`, `prioridade_media`, `em_observacao`) é definida em `docs/prioritization-criteria.md` a partir de longevidade, volume de anúncios ativos da oferta e potencial de recompra. Ela é **independente** dos estados acima: uma oferta `prioridade_alta` continua `sinais_de_atividade` enquanto não houver prova de vendas. Toda contagem de anúncios registra fonte, data da consulta, método e se é estimativa; idade de anúncio individual e histórico da oferta são campos distintos.

## Qualidade

Marque confiança como `alta`, `moderada` ou `baixa` com justificativa. Não calcule score numérico de faturamento inferido. Para propostas de reprodução de formato criativo, priorize análise de padrões, sem copiar indevidamente material protegido.

## Prontidão para adaptação

Separe três análises: apelo comercial, plausibilidade de alegações, permissibilidade regulatória no país de destino. Ofertas de suplementos podem exigir revisão jurídico-regulatória antes de qualquer teste publicitário.
