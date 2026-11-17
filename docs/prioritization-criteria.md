# Critérios de mineração e priorização

Objetivo do Offer Miner: descobrir **ofertas internacionais de suplementos** com sinais relevantes de **atividade publicitária**, **potencial de escala** e **possibilidade de recompra**.

Este documento é a referência única dos critérios. `CLAUDE.md`, as skills e os templates apontam para cá. Os números são **parâmetros ajustáveis** (uma missão pode sobrescrevê-los explicitamente), não regras absolutas.

> **Prioridade ≠ validação.** A prioridade só ordena o que investigar primeiro. Quantidade e idade de anúncios **não** medem vendas, investimento, lucro, CPA ou ROAS. A classificação de evidência (`descoberta` → `validacao_comercial_comprovada`, ver `docs/evidence-standard.md`) é independente e continua obrigatória.

## Parâmetros padrão

| Parâmetro | Valor padrão |
|---|---|
| Idade mínima relevante de anúncio ativo | 30 dias |
| Marcos de destaque de longevidade | 60, 90 e 180+ dias |
| Volume forte (anúncios ativos da oferta) | ≥ 100 |
| Volume médio | 20–99 |
| Volume baixo | < 20 |
| Categoria da lista principal | suplementos consumíveis |

## 1. Longevidade dos anúncios

Registrar sempre:

- `checked_at_utc` — data/hora da consulta à biblioteca.
- **Idade de cada anúncio individual ativo** = data da consulta − "veiculação iniciada em". Faixas: `<30`, `30–59`, `60–89`, `90–179`, `180+` dias.
- **Anúncio ativo mais antigo** da oferta (ID, data de início, idade em dias).
- **Histórico publicitário da oferta** = primeira data de veiculação observada entre **todos** os anúncios da oferta (ativos e inativos) até a data da consulta. É diferente da idade de um anúncio individual: uma oferta pode ter histórico de 6 meses e nenhum anúncio ativo com mais de 20 dias (criativos trocados com frequência).
- **Distribuição por faixa** dos anúncios ativos (quantos com 30+, 60+, 90+ dias).

Cuidados:

- Usar a data exibida pela fonte (ex.: Meta "Veiculação iniciada em"). Nunca estimar data de início.
- Fora da UE/Reino Unido, a Meta pode não exibir anúncios comerciais inativos → o histórico pode estar **truncado**. Registrar essa limitação.
- Anúncio reativado ou duplicado pode ter data de início mais recente que o criativo original; registrar como observado.

## 2. Volume de anúncios

Registrar **separadamente**:

| Campo | Significado |
|---|---|
| `active_ads_offer` | anúncios **ativos** ligados ao **produto específico** (mesmo produto/LP; filtrado por texto, destino ou criativo) |
| `active_ads_brand_or_domain` | todos os anúncios ativos da marca/domínio/página, inclusive outros produtos |
| `total_shown_by_source` | contador exibido pela fonte (ex.: Meta "~2.200 resultados"), marcado como estimativa |
| `unique_creatives` | criativos distintos (texto + mídia), contando variações do mesmo criativo uma única vez |
| `pages_or_advertisers` | páginas/anunciantes que veiculam a oferta, com contagem por página |
| `count_source` | biblioteca/consulta exata (URL), data e método (amostra, rolagem completa, API, agregador) |
| `count_is_estimate` | `true` quando o número vem de contador aproximado, agregador terceiro ou amostra parcial |

Regras de contagem:

- A meta de volume (100+/20–99/<20) usa `active_ads_offer`, nunca o total da marca/domínio.
- Variações (mesmo criativo em vários anúncios, ex.: "3 anúncios usam esse criativo e esse texto"; tamanhos; idiomas da mesma peça) contam como **anúncios**, mas **não** como produtos ou ofertas diferentes. Registrar também `unique_creatives`.
- Anúncios de várias páginas (marca, personas, "comunidades") que levam ao mesmo produto/LP somam na mesma oferta; listar as páginas.
- Domínios espelho/irmãos só são somados quando a relação estiver **observada** (mesmo produto, mesma marca no anúncio); caso contrário, contar à parte e marcar como hipótese.
- Amostra parcial (só os primeiros N cards) → informar N e `count_is_estimate: true`. Não extrapolar.
- Agregadores terceiros (admanage.ai etc.) = estimativa não auditada; preferir a biblioteca oficial quando acessível.

## 3. Tipo de produto e recompra

Lista principal: **somente suplementos**. Produtos de outras categorias vão para "fora de escopo" no relatório, salvo pedido explícito da missão.

Classificar o tipo:

- `consumivel_recorrente` — uso diário/contínuo, embalagem se esgota (cápsulas, pós, gomas, líquidos).
- `consumivel_ocasional` — uso pontual ou ciclos curtos (ex.: detox de 7 dias).
- `nao_consumivel` — fora do foco.

Investigar e registrar, separando **observado** de **calculado**:

- Dose diária indicada (página/rótulo).
- Unidades por embalagem.
- **Duração estimada da embalagem** = unidades ÷ dose diária → marcar como cálculo.
- Kits/bundles (ex.: 1, 2+1, 3+2, "cure 4 mois") com preço e duração total.
- **Assinatura / entrega recorrente:** `verificada` (opção visível na página/checkout sem compra), `alegada` (mencionada em texto/FAQ sem opção visível), `nao_observada`.
- Desconto por recompra/assinatura, quando verificável.

**Potencial de recompra** (inferência a partir do tipo de produto e duração) é diferente de **assinatura comprovadamente disponível** (fato observado). Os dois campos ficam separados.

## 4. Classificação de prioridade

| Prioridade | Condições (todas) |
|---|---|
| `prioridade_alta` | `active_ads_offer` ≥ 100 **e** ≥ 1 anúncio ativo com 30+ dias **e** `consumivel_recorrente` |
| `prioridade_media` | `active_ads_offer` 20–99 **e** histórico consistente **e** potencial de recompra |
| `em_observacao` | < 20 anúncios ativos, atividade só recente (< 30 dias) **ou** evidência insuficiente |

- **Histórico consistente:** anúncios da oferta observados em pelo menos 2 meses distintos **ou** ao menos 1 anúncio ativo com 30+ dias.
- Se faltar um critério da faixa, cair uma faixa e explicar qual critério faltou.
- Dados não verificáveis (biblioteca inacessível, só agregador) → no máximo `prioridade_media`, com justificativa; sem nenhum dado de anúncio → `em_observacao`.
- **Oportunidade emergente:** não descartar por volume baixo. Marcar `emergente: true` quando houver sinal de entrada recente forte (ex.: muitos anúncios lançados nos últimos 30 dias, novo mercado de uma oferta já ativa em outro país). Fica em `em_observacao`, mas aparece destacada.
- Toda prioridade vem com justificativa curta citando os números, a fonte e a data.

## 5. Regras de investigação

1. Continuar pesquisando por país, problema, mecanismo, ingrediente e idioma, conforme a missão.
2. **Antes de atribuir prioridade**, investigar o histórico publicitário da oferta: biblioteca oficial por domínio (frase exata), marca, nome do produto e páginas anunciantes; separar produto específico do restante da marca.
3. Investigar recorrência na página de venda (dose, embalagem, kits, assinatura).
4. Nunca confundir quantidade de anúncios com volume de vendas, investimento ou lucratividade.
5. Nunca declarar oferta validada comercialmente sem evidência adequada (ver `docs/evidence-standard.md`).
