---
name: evidence-validation
description: Confere evidências das ofertas, separa sinais de atividade de vendas reais, detecta lacunas e classifica risco.
---

# Auditoria de evidências

Para toda observação exigir: **afirmação concreta**, URL, tipo de fonte, data de consulta e limite de verificação. Preferir dados de primeira mão, mas nunca confundir declaração comercial com comprovação independente.

## Classificação

- `descoberta`: marca/produto identificado e URL rastreável.
- `sinais_de_atividade`: página comercial e/ou anúncios publicamente observáveis.
- `evidencia_de_tracao`: múltiplos sinais comerciais independentes contextualizados (ainda não prova vendas/lucro).
- `validacao_comercial_comprovada`: dados verificáveis e relevantes de vendas/performance. Raro para concorrentes; documentar explicitamente a origem e limitações.

Uma nota de prioridade pode ajudar a ordenar as pesquisas, mas **não representa receita ou lucratividade**. Separar observações de hipóteses, listar conflitos e marcar campos desconhecidos como `null`, não estimá-los.

## Prioridade (independente da classificação acima)

Aplicar `docs/prioritization-criteria.md`: `prioridade_alta`, `prioridade_media`, `em_observacao` (+ `emergente`). Antes de aceitar uma prioridade, conferir:

- Longevidade: data da consulta e "veiculação iniciada em" registradas por anúncio; idade calculada a partir delas; idade de anúncio individual separada do histórico da oferta; histórico possivelmente truncado (anúncios inativos ocultos) sinalizado.
- Volume: contagem do **produto específico** separada do total da marca/domínio; variações do mesmo criativo não tratadas como produtos diferentes; domínios/páginas somados só com relação observada; fonte, método (amostra/rolagem/agregador) e `count_is_estimate` presentes.
- Recorrência: dose e unidades citadas da página; duração marcada como cálculo; assinatura só `verificada` se a opção foi vista.
- Categoria: só suplementos na lista principal.
- Coerência: nenhuma frase trata quantidade/idade de anúncios como vendas, investimento ou lucro; nenhuma oferta sobe de classificação de evidência por causa da prioridade.

## Suplementos

Registrar alegações de mercado como alegações, sem afirmar eficácia. Sinalizar ausência de informação verificável sobre formulação, segurança, regulação e compatibilidade com o país de destino. Nunca apresentar marketing como evidência clínica.
