# Relatório da missão 002: mineração aberta de suplementos nos EUA

## Escopo e execução

- **Data de execução (UTC):** 2026-11-17, das 19:20 às 20:40, aproximadamente. As contagens da Meta foram feitas entre 19:25 e 20:30 UTC. O Google Ads Transparency foi consultado às 20:18–20:19 UTC.
- **Missão de origem:** "Missão 002 — Mineração aberta de suplementos nos EUA". Pede 10 ofertas distintas, sem lista prévia de marcas e com diversidade de categorias. Serve como benchmark de descoberta autônoma.
- **Mercado de venda:** Estados Unidos (`country=US` na Meta Ad Library e `region=US` no Google Ads Transparency).
- **Problema, mecanismo e ingredientes:** abertos. A descoberta passou por 37 temas: sono, intestino, menopausa, testosterona, cognição, peso, GLP-1, glicemia, energia, cortisol, magnésio, cabelo, colágeno, fígado, próstata, zumbido, visão, bexiga, café de cogumelos, creatina, colostro, shilajit, neuropatia, probiótico feminino, pressão arterial, colesterol, tireoide, ansiedade, ITU, libido feminina, ereção, eletrólitos, fibra, vitaminas infantis e probiótico oral.
- **Idioma:** inglês.
- **Ferramentas realmente usadas:**
  - Navegador embutido do Orca, sem login, para Meta Ad Library, Google Ads Transparency e páginas de venda.
  - Script local que lê os cards da Ad Library: ID, data de início, página, nº de anúncios que usam o criativo, destino e texto.
  - Subagentes `web-fetch` para 4 páginas de venda.
  - Não foram usados TikTok Creative Center, transcrição nem download de vídeos.
- **Limites de pesquisa:**
  - 37 buscas de descoberta por palavra-chave.
  - 21 buscas por frase exata (domínio ou marca).
  - 14 consultas ao Google Ads Transparency.
  - 26 páginas de venda ou advertoriais lidas.
  - No máximo 3 rodadas de aprofundamento por oferta.
- **Parâmetros de priorização:** padrão de `docs/prioritization-criteria.md`.
  - Idade mínima relevante: 30 dias.
  - Faixas: alta ≥ 100, média 20–99 e observação < 20 anúncios ativos da oferta.
  - Categoria: suplementos consumíveis para humanos.
- **Convenção de contagem:**
  - "Anúncios" soma as variações exibidas ("N anúncios usam esse criativo e esse texto").
  - "Cards" são as entradas distintas da biblioteca.
  - Faixas de idade contam cards.
  - Idade = 2026-11-17 − "Veiculação iniciada em".
- **Motivo do encerramento:**
  - 10 ofertas distintas, de 10 categorias, documentadas com página de venda, recorrência e histórico publicitário.
  - A paginação da Meta ficou indisponível sem login, e insistir não traria dados novos.
  - A missão manda parar ao consolidar o ranking.

> **Limitação principal (ler antes do ranking):**
>
> - Por volta das 19:55 UTC, a Meta Ad Library sem login parou de carregar páginas adicionais de resultados. As requisições respondiam 200, mas sem cards.
> - O bloqueio não foi contornado: nenhum login, nenhuma troca de filtros para "fatiar" resultados.
> - Depois disso, cada busca trouxe só a 1ª página (~25–30 cards).
> - Por isso, **todas as contagens são pisos.** Elas resultam da união dos IDs únicos vistos em todas as buscas, e `count_is_estimate = true`.
> - Rolagem ampla só foi possível para Happy V (282 cards), Nuora (288 cards; os IDs se perderam ao reescrever o arquivo e só o agregado ficou) e ProstaGenix (rolagem completa).
> - O contador "~N resultados" da Meta vale para o domínio ou termo inteiro e é registrado como estimativa da fonte.

## Resumo executivo

- **Candidatos encontrados (suplementos para humanos):** 20. Ficaram 10 no relatório principal; 9 foram registrados como "não selecionados" e 1 (Metabolae) foi excluído por deduplicação.
- **Ofertas com evidência mínima:** 10.
- **Por prioridade:** alta 4 · média 6 · em observação 0 no top 10. Fora do top 10: Reliva (zumbido) em observação, possivelmente emergente.
- **Categorias no top 10:** 10 distintas, uma por oferta:
  1. saúde íntima feminina;
  2. incontinência feminina;
  3. próstata;
  4. cardiovascular/beterraba;
  5. cognição/nootrópico;
  6. creatina;
  7. metabolismo/inchaço na menopausa;
  8. testosterona;
  9. sono/cortisol (magnésio);
  10. intestino/SIBO.
- **Padrões comerciais observados:**
  1. **Páginas-persona e storytelling longo:** "Alicia Darling" (Nuora, 152 anúncios na rolagem da marca), "Carol Warren" (Nutrition Therapy, 68), "The Health Haven" e "Leslie Hosmer" (Rosabella) e "Wellness Tips" (SPNutrition). Histórias em primeira pessoa com 1.000+ palavras levam a advertoriais.
  2. **Parceria com criadores profissionais:** um farmacêutico (Philsmypharmacist, para Avantera, desde 2024-06), um ginecologista ou perfil "obgyn.mom" e criadoras de UGC (Happy V).
  3. **Front-end barato + refil:** Lovy anuncia US$ 19 no 1º mês e o texto menciona "$49.99 Refill Ships In 30 Days". Rosabella usa "Buy 3 Get 3" e refil automático a cada 30, 60 ou 90 dias. Primal Viking anuncia "72% OFF on subscription".
  4. **Ângulo "não é gordura, é cortisol/biofilme/inflamação":** aparece em Nuora, SPNutrition, Primal Viking e Standard Lab. É a mesma estrutura de reenquadramento aplicada a problemas diferentes.
  5. **Ângulo anti-fármaco:** "natural GLP-1" (Nuora, Akka), "No more relying on ED drugs" (ProstaGenix), comparação com finasterida (STĒLO) e anti-Imodium (Nutrition Therapy). Também é o principal foco de risco regulatório.
- **Lacunas:**
  - Contagens completas por oferta (paginação).
  - Preços da SPNutrition.
  - Doses verbatim da ProstaGenix.
  - Nenhum dado de TikTok.
  - Histórico de anúncios inativos indisponível fora da UE.

> Prioridade ordena a investigação. Quantidade e idade de anúncios **não** indicam vendas, investimento ou lucro.

## Ranking de prioridade

| # | Oferta (marca — produto) | Categoria | Prioridade | Anúncios ativos da oferta (cards) — piso | Ativos da marca/domínio | Anúncio ativo mais antigo (dias) | Cards 30+ / 90+ | Tipo / duração | Assinatura | Evidência | Fonte e data da contagem |
|---|---|---|---|---|---|---|---|---|---|---|---|
| 1 | Happy V — Prebiotic + Probiotic | saúde íntima feminina | **prioridade_alta** | ≥839 (277); só PDP: ≥234 (103) | ≥851; Meta ~2.200; Google ~400 | ≥52* | 215 / 0 | consumível · 30 porções = 30 d | verificada | evidencia_de_tracao | Meta frase exata "happyv.com", 282 cards rolados, 2026-11-17 ~19:40Z |
| 2 | Lovy — UroControl | incontinência feminina | **prioridade_alta** | ≥362 (50) | ≥362; Meta "UroControl" ~880; Google ~300 | 234 | 41 / 20 | consumível · 60 cáps. = 30 d | alegada | evidencia_de_tracao | Meta "bladder leaks supplement" + "UroControl" + "Lovy", 19:45–20:05Z |
| 3 | ProstaGenix — Multiphase Prostate | próstata 55+ | **prioridade_alta** | ≥140 (46) | ≥140; Meta ~56 (domínio); Google 24 | 384 | 30 / 14 | consumível · "One Month Supply" | nao_observada | sinais_de_atividade | Meta "prostagenix.com", rolagem completa, ~19:50Z |
| 4 | Rosabella — Beetroot 1.300 mg | cardiovascular / circulação | **prioridade_alta** | ≥140 (112) | ≥140; Google n/c | 89 | 61 / 0 | consumível · 30 porções = 30 d | verificada | sinais_de_atividade | Meta, buscas temáticas (pressão, glicemia, intestino, sono) + frase exata, 19:25–20:22Z |
| 5 | Avantera — Elevate | cognição / nootrópico | prioridade_media | ≥56 (34) | ≥122; Meta ~360; Google ~200 | **894** | 30 / 25 | consumível · 28 d | alegada | evidencia_de_tracao | Meta "avanterahealth.com" + "memory focus supplement", 19:30–20:05Z |
| 6 | Crave — Creatine Gummies | creatina | prioridade_media | ≥89 (26) | ≥89; Meta ~890; Google 3 | 495 | 26 / 20 | consumível · 3 gomas/dia | verificada | sinais_de_atividade | Meta "trycrave.com" + "creatine gummies" |
| 7 | Nuora — Gut Ritual (berberina) | metabolismo / inchaço na menopausa | prioridade_media | ≥51 (22) | ≥379 (rolagem de 288 cards); Meta ~1.800; Google ~800 | 291 (marca: 405) | 22 / 22 | consumível · 60 cáps. = 30 d | alegada | evidencia_de_tracao | Meta "mynuora.com", rolagem ~19:35Z (agregado) + amostras |
| 8 | Primal Viking — Ancestral Testosterone Booster | testosterona | prioridade_media | ≥78 (67) | ≥78; Meta ~2.800; Google 0 | 180 | 49 / 20 | consumível · 48 cáps. = 24 d (cálculo) | verificada | sinais_de_atividade | Meta "primalviking.com" + "testosterone booster men" |
| 9 | SPNutrition — Magnesium Bisglycinate Gummies | sono / cortisol | prioridade_media | ≥72 (42) | ≥109; Meta ~4.900; Google ~200 | 256 | 34 / 11 | consumível · 30 porções | alegada | evidencia_de_tracao | Meta "spnutrition-us.com" + "magnesium", "sleep", "cortisol" |
| 10 | Nutrition Therapy — Oil of Oregano Drops | intestino / SIBO / IBS-D | prioridade_media | ≥79 (25) | ≥79; Meta ~320; Google 0 | 144 | 25 / 17 | consumível · 60 mL = 30 d | verificada | sinais_de_atividade | Meta "nutritiontherapy.co" + "bloating", "gut health" |

\* No caso da Happy V, todos os 282 cards rolados começaram em 2026-09-26 ou depois. Esse valor reflete a ordem de exibição da Meta, não necessariamente o anúncio mais antigo da oferta.

### Links diretos das páginas de venda

1. Happy V: https://happyv.com/products/probiotics-vaginal-health-supplement
2. Lovy UroControl: https://secure.trylovy.com/urocontrol-s-bof
3. ProstaGenix: https://www.prostagenix.com/
4. Rosabella Beetroot: https://track.tryrosabella.com/cdc16426-3e48-40a7-9fad-21098084f6cf (link de tracking dos anúncios que leva à PDP de Beetroot; os 4 links de tracking observados levam à mesma oferta)
5. Avantera Elevate: https://avanterahealth.com/pages/elevate-shop
6. Crave: https://trycrave.com/products/crave-creatine-gummies
7. Nuora Gut Ritual: https://mynuora.com/pages/gut-capsule
8. Primal Viking: https://primalviking.com/products/primal-reindeer-testosterone-support
9. SPNutrition: https://spnutrition-us.com/products/maximum-absorption-magnesium-bisglycinate-gummies
10. Nutrition Therapy: https://nutritiontherapy.co/products/oil-of-oregano

### Anúncios de referência (IDs da Meta Ad Library)

A lista completa por oferta está em `data/ads_<oferta>.csv`. URL de cada anúncio: `https://www.facebook.com/ads/library/?id=<ID>`.

| Oferta | Ativo mais antigo (ID, início) | Outros IDs antigos |
|---|---|---|
| Happy V | 1070888349269354 (2026-09-26) | 1105326328703918, 1825083412244409 |
| Lovy UroControl | 1354871836658279 (2026-03-28) | 2321580634918235 (2026-04-05), 2018523345538087 (2026-04-11) |
| ProstaGenix | 24896050666726199 (2025-10-29) | 2367267987026167 (2025-10-29), 1756102741716589 (2025-11-03) |
| Rosabella | 1273690935826594 (2026-08-20) | 4573235272948595 (2026-08-20), 3658038091030785 (2026-08-25) |
| Avantera Elevate | 1081955446237798 (2024-06-06) | 1171823840810456 (2024-06-25), 3809222252731154 (2024-07-10) |
| Crave | 2020770371994276 (2025-07-10) | 1115849997026202 (2025-07-12), 593238203579693 (2025-07-15) |
| Nuora Gut Ritual | 1438360120994908 (2026-01-30) | 1852212378817743, 1213209437672888 (2026-02-11); marca: 782108268048154 (2025-10-08) |
| Primal Viking | 952973200670606 (2026-05-21) | 2461748607631261, 862472436325307 (2026-06-03) |
| SPNutrition Magnésio | 863178650084986 (2026-03-06) | 1432406478580122 (2026-03-08), 1607505907213420 (2026-04-19) |
| Nutrition Therapy | 1045429338426637 (2026-06-26) | 1685613519433600, 1710774990232111 (2026-06-26) |

## Comparativo de categorias, mecanismos e modelos de recompra

| # | Categoria | Mecanismo anunciado | Formato | Dose / duração | Preço de entrada observado | Modelo de recompra | Ângulo criativo dominante |
|---|---|---|---|---|---|---|---|
| 1 | saúde íntima feminina | probiótico 7 cepas + prebiótico PreforPro, "90 dias para rebalancear" | cápsula | 30 porções | US$ 40,49 (assinatura) | assinatura 1/3/6 meses (−10/−15/−20%) | vergonha/confiança ("down there"), UGC de criadoras |
| 2 | incontinência feminina | isoflavonas + semente de abóbora + magnésio | cápsula | 2/dia · 60 = 30 d | US$ 19 (1 mês) | front-end barato + refil (texto) | depoimento longo de mulher 50+, hysterectomy hook |
| 3 | próstata | beta-sitosterol "francês" + ConsumerLab | cápsula | 3/dia (resumo) · 1 mês | US$ 49,95 | pacotes 3/5 meses, sem assinatura | carta de vendas com celebridade, "Prostate Shrinking" |
| 4 | cardiovascular | nitratos da beterraba | cápsula | 2/dia · 30 d | US$ 11,99–19,97/frasco | BOGO + refil 30/60/90 d (até −40%) | ficção longa ("Nine Words, a Gravel Lane...") por páginas-persona |
| 5 | cognição | cafeína + L-teanina + colinérgicos | cápsula | 2/dia · 28 d | US$ 24,98 (1º pedido) | entrega a cada 4 semanas | farmacêutico criador, "Limitless" |
| 6 | creatina | creatina monohidratada em goma | goma | 3/dia | US$ 35 (assinatura) | assinatura, kit 90 d | "creatina que tem gosto de doce", comparativo |
| 7 | metabolismo / menopausa | berberina "GLP-1" + bromelina "anti-biofilme" | cápsula | 2/dia · 30 d | US$ 29–49 | refil automático (texto), 3 meses | confissão ("I lied"), inchaço da menopausa |
| 8 | testosterona | órgãos de rena + testículo bovino | cápsula | 2/dia · 24 d | US$ 25/pote (assinatura) | assinatura "72% OFF", bundles de até 9 potes | "barriga de cerveja", estudo, ancestralidade |
| 9 | sono / cortisol | bisglicinato de magnésio 400 mg | goma | 2/dia · 30 d | n/obs. | refil 30 d (texto) + rota "sem assinatura" | depoimento 5 estrelas, "cortisol overloaded" |
| 10 | intestino / SIBO | carvacrol antimicrobiano em gotas | líquido | 2 mL/dia · 30 d | US$ 31,99 | refil 30 d com −20% | médico do navio, "nunca foi IBS-D" |

**Leitura comparativa (inferência):**
- As ofertas com mais volume observado (1–4) combinam três elementos: problema íntimo ou constrangedor, público 45+ e uso "para sempre" (bexiga, próstata, pH vaginal, circulação).
- As ofertas de maior longevidade individual (Avantera 894 d, Crave 495 d, ProstaGenix 384 d) usam poucos criativos reaproveitados por muito tempo: 8 a 11 textos distintos.
- As ofertas com páginas-persona (Rosabella, Nuora, Nutrition Therapy, SPNutrition) giram mais criativos.

## Ofertas investigadas

### Oferta 1 — Happy V: Prebiotic + Probiotic

- **Mercado de venda:** EUA, com frete grátis para assinaturas nos EUA.
- **Origem da marca:** HAPPY V, LLC (anunciante verificado no Google).
- **Categoria e problema:** saúde vaginal (odor, corrimento, desequilíbrio de pH), mais intestino e imunidade.
- **Mecanismo alegado:** "7 clinically studied probiotic strains with PreforPro". Sequência anunciada: "Week 1… Month 1… Month 3".
- **Página:** https://happyv.com/products/probiotics-vaginal-health-supplement (lida em 2026-11-17 ~20:10Z).
- **Preço:**
  - Avulso: US$ 44,99.
  - Assinatura: US$ 40,49 (1 frasco), US$ 38,24/frasco (3) e US$ 35,99/frasco (6).
  - Black Friday: +20% na 1ª assinatura.
  - A página exibe "4.9 · 6.145" avaliações. É dado do próprio site.

#### Histórico publicitário

- **Consulta:** Meta frase exata "happyv.com", US, ativos. Contador da fonte: ~2.200 resultados (estimativa). 282 cards rolados antes do bloqueio.
- **Anúncios da oferta:** ≥839 em 277 cards, contando PDP e kits que contêm o produto (Fresh Start Kit, pH Balance Kit, pre-pro-mega).
  - Só com destino direto na PDP: ≥234 anúncios em 103 cards, 85 deles com 30+ dias.
- **Marca:** ≥851.
- **Por idade (cards):** <30 d 62 · 30–59 d 215 · 60+ 0.
- **Anúncio ativo mais antigo na amostra:** 1070888349269354, 2026-09-26, 52 dias. Provavelmente truncado pela ordem de exibição.
- **Páginas:** Happy V 634 · Mik Zazon 42 · Daniella Levy 30 · thyriifrazier 25 · obgyn.mom 25.
- **Criativos:** 12 textos distintos. 118 dos 277 cards são vídeos.
- **Google Ads Transparency:** cerca de 400 anúncios, HAPPY V, LLC verificado.

#### Recorrência

- **Tipo:** consumível recorrente.
- **Embalagem:** "1 bottle = 30 servings", ou seja, 30 dias (cálculo com 1 porção por dia; dose explícita não observada no texto lido).
- **Assinatura:** **verificada**. Seletor "Subscribe & Save / One-time Purchase" visível, com 1, 3 ou 6 frascos.
- **Potencial de recompra (inferência):** alto. A própria página pede 90 dias contínuos.

#### Criativos

- **Hooks:**
  - "Don't skip out on plans because your issues "down there"…" (93 cards)
  - "Prioritize your vaginal health…" (60)
  - "Don't let odor, imbalance, or discomfort stop you…" (57)
- **Formatos:** vídeo UGC com criadoras via parceria e imagens de kit.

#### Classificação

- **Evidência:** `evidencia_de_tracao`. Meta e Google ativos, com anunciante verificado.
- **Prioridade:** `prioridade_alta`. ≥234 anúncios só na PDP, 85 cards da PDP com 30+ dias, consumível com assinatura verificada.
- **Confiança:** média, porque a amostra cobre cerca de 13% do contador.
- **Riscos regulatórios:**
  - Anúncio com "Reduce Symptoms of BV, YI & UTI" se aproxima de alegação de doença.
  - "Clinically studied" não verificado.

### Oferta 2 — Lovy: UroControl

- **Categoria e problema:** perda urinária e urgência em mulheres. Hooks citam histerectomia e menopausa.
- **Mecanismo alegado:** "Magnesium citrate helps relax bladder muscle spasms" e isoflavonas de trevo-vermelho.
- **Página:** https://secure.trylovy.com/urocontrol-s-bof (2026-11-17 ~20:25Z).
- **Preço e estrutura:**
  - 1 mês: US$ 19 (riscado US$ 59).
  - 2 meses: US$ 39.
  - 3 meses: US$ 59.
  - Texto "$49.99 Refill Ships In 30 Days".
  - Garantia de 90 dias, elegível para HSA/FSA.
  - Selos "52,312+ Customers" e "67% OFF TODAY ONLY" (contador).
- **Anunciante no Google:** Mngn Brands LLC.

#### Histórico publicitário

- **Anúncios da oferta:** ≥362 em 50 cards. Destino direto na LP: 340.
- **Por idade (cards):** <30 9 · 30–59 14 · 60–89 7 · 90–179 8 · 180+ 12.
- **Anúncio ativo mais antigo:** 1354871836658279, 2026-03-28, 234 dias.
- **Páginas:** Lovy 352 · Unstoppable After 50 6 · Lovy Secret Deals 2.
- **Contadores da fonte:** "UroControl" ~880; "Lovy" ~1.400 (termo ambíguo).
- **Google:** cerca de 300 anúncios.
- **Criativos:** 15 textos distintos. Um depoimento concentra muitas variações. Nenhum vídeo na amostra.

#### Recorrência

- 2 cápsulas por dia; 60 cápsulas, "last for about a month". Duração: 30 dias.
- **Assinatura:** `alegada`. Aparecem "Refill Every 30 Days" e "Pause or Stop Anytime", mas não ficou claro qual opção a ativa.
- A FAQ fala em 3 a 6 meses de uso.
- **Hipótese:** front-end de US$ 19 com refil de US$ 49,99. Confirmar no checkout, sem comprar.

#### Classificação

- **Evidência:** `evidencia_de_tracao`.
- **Prioridade:** `prioridade_alta` (≥362; 41 cards com 30+ dias; consumível).
- **Confiança:** média.
- **Riscos:**
  - "Cranberry extract helps protect against UTIs" é alegação de prevenção de doença.
  - "no reported side effects".
  - Percentuais de pesquisa interna (87–94%).
  - Âncora de preço riscado.
- **Faltam:** doses (tabela só em imagem).

### Oferta 3 — ProstaGenix: Multiphase Prostate Supplement

- **Categoria:** próstata, homens 55+.
- **Mecanismo alegado:** beta-sitosterol "French Maritime Pine" com "CrystalPure Extraction", mais quercetina, semente de uva e romã. Cita o prêmio ConsumerLab.
- **Página:** https://www.prostagenix.com/ (lida via Orca e web-fetch, 2026-11-17).
- **Preço:** 1 mês US$ 49,95 (de US$ 69,95), 3 meses US$ 99,95, 5 meses US$ 149,95, pagamento único. Os valores de 3 e 5 meses vieram do resumo do subagente; confirmar verbatim.
- **Garantia:** 90 dias.

#### Histórico publicitário

- **Consulta:** Meta frase exata "prostagenix.com". **Rolagem completa:** 41 cards / 86 anúncios, contra ~56 exibidos.
- **União com as buscas temáticas:** 46 cards / ≥140 anúncios, incluindo prostagenixvip.com, da mesma página anunciante.
- **Por idade (cards):** <30 16 · 30–59 16 · 180+ 14.
- **Anúncio ativo mais antigo:** 24896050666726199, 2025-10-29, 384 dias.
- **Página:** ProstaGenix.com (140).
- **Criativos:** 8 textos distintos, muito reaproveitamento; 4 vídeos.
- **Google:** 24 anúncios. Anunciante exibido: "Superbalife International, LLC - DO NOT USE - IN OCA", registrado como observado.

#### Recorrência

- 3 cápsulas por dia (resumo; não verbatim), "One Month Supply".
- **Assinatura:** `nao_observada`. Recompra por pacotes de 3 e 5 meses.

#### Classificação

- **Evidência:** `sinais_de_atividade`.
- **Prioridade:** `prioridade_alta` (≥140; 30 cards com 30+ dias; 14 com 180+).
- **Confiança:** média.
- **Riscos altos:**
  - "Prostate Shrinking Super Pill", "No more relying on ED drugs", "27 TIMES More Effective".
  - Celebridade e urologista como endossantes; narrativa "Big Pharma".

### Oferta 4 — Rosabella: Beetroot (1.300 mg)

- **Categoria:** circulação, saúde cardíaca e pressão (copy). Público 50+.
- **Mecanismo alegado:** "naturally rich in dietary nitrates, to aid healthy circulation".
- **Página:** https://track.tryrosabella.com/cdc16426-3e48-40a7-9fad-21098084f6cf. Os 4 links de tracking observados foram verificados e abrem a mesma oferta de Beetroot.
- **Preço:**
  - De US$ 19,97 a US$ 11,99/frasco, conforme o bundle (Buy 1/2/3 Get 1/2/3 Free).
  - Refil: 2 frascos a cada 30 dias por US$ 39,95; 4 a cada 60 dias por US$ 69,95; 6 a cada 90 dias por US$ 84,95 (+US$ 5,95 de frete).
  - Garantia de 90 dias.
  - "Rated 4.4/5 on Amazon (as of Nov 5, 2026)": não verificado.

#### Histórico publicitário

- **Anúncios:** ≥140 em 112 cards, a maior parte vinda das buscas "blood pressure", "blood sugar", "gut health" e "sleep".
  - A frase exata "tryrosabella.com" mostra só ~56 resultados, porque o domínio aparece só no link de tracking.
- **Por idade (cards):** <30 51 · 30–59 32 · 60–89 29 · 90+ 0.
- **Anúncio ativo mais antigo:** 1273690935826594, 2026-08-20, 89 dias.
- **Páginas:** The Health Haven 46 · Leslie Hosmer 16 · Mary Edwards 11 · Essential Health Finds 11 · The Heart Health Project 11 · Eric Bussey 7, entre outras.
- **Criativos:** 55 textos distintos, a maior diversidade da missão. Nenhum vídeo.

#### Recorrência

- 2 cápsulas por dia, 30 porções: 30 dias.
- **Assinatura:** **verificada** ("Subscribe & Save 40% every 90 days").
- A página recomenda 90 dias de uso.

#### Classificação

- **Evidência:** `sinais_de_atividade`.
- **Prioridade:** `prioridade_alta` (≥140; 61 cards com 30+ dias; assinatura verificada).
- **Confiança:** média, porque a atividade é recente (nada com 90+ dias) e concentrada em personas.
- **Riscos:**
  - Páginas-persona com nomes de pessoas.
  - Ficção apresentada como história.
  - Risco de associação implícita com tratamento de hipertensão.

### Oferta 5 — Avantera: Elevate

- **Categoria:** foco, memória e energia.
- **Mecanismo:** 95 mg de cafeína do chá-verde, 200 mg de L-teanina, bacopa (50% bacosídeos), juba-de-leão, CDP-colina, rhodiola e cúrcuma. Alegação: "supports your brain's acetylcholine pathway".
- **Página:** https://avanterahealth.com/pages/elevate-shop.
- **Preço:** US$ 24,98 (de US$ 49,95), com "28-day supply delivered every 4 weeks. Pause or cancel anytime."
- **Garantia:** 30 dias. Há aviso FDA.

#### Histórico publicitário

- **Anúncios do Elevate:** ≥56 em 34 cards. Marca: ≥122.
- **Contador do domínio:** ~360. Google: ~200.
- **Por idade (cards):** <30 4 · 30–59 5 · 90–179 5 · 180+ 20.
- **Anúncio ativo mais antigo:** 1081955446237798, **2024-06-06, 894 dias**.
- **Páginas:** Philsmypharmacist 39 · Avantera 13.
- **Criativos:** 11 textos distintos; 21 dos 34 cards são vídeos.

#### Recorrência

- 2 cápsulas por dia, 28 dias.
- **Assinatura:** `alegada`. O texto descreve entrega a cada 4 semanas, mas o seletor não foi confirmado.

#### Classificação

- **Evidência:** `evidencia_de_tracao`.
- **Prioridade:** `prioridade_media`. Faltou o piso de 100 anúncios do produto.
- **Destaque:** maior longevidade da missão. Um criador farmacêutico veicula o mesmo vídeo há ~2,5 anos.
- **Riscos:** "Limitless" e "neuroprotective".

### Oferta 6 — Crave: Creatine Monohydrate Gummies

- **Categoria:** creatina para energia, força e foco. Há LP "after-35".
- **Página:** https://trycrave.com/products/crave-creatine-gummies.
- **Preço e estrutura:** US$ 35 / US$ 44; Variety Pack de 90 dias. A FAQ trata de gerenciar a assinatura. 308 avaliações no site.
- **Histórico:**
  - ≥89 anúncios em 26 cards, todos com 30+ dias (90–179: 8; 180+: 12).
  - Mais antigo: 2020770371994276, 2025-07-10, 495 dias.
  - Meta ~890; Google 3 (anunciante "Michael Potter").
  - 20 dos 26 cards são vídeos.
- **Recorrência:** 3 gomas por dia. Unidades por pote não observadas. Assinatura **verificada**.
- **Classificação:** `sinais_de_atividade` · `prioridade_media` (piso de 89).
- **Risco:** gramas de creatina por porção não observados; a categoria tem histórico de subdosagem.

### Oferta 7 — Nuora: Gut Ritual / "Gut Capsule"

- **Categoria:** inchaço e peso abdominal na menopausa.
- **Fórmula (Supplement Facts):** berberina 350 mg, bromelina 200 mg, ashwagandha 200 mg, dente-de-leão, quercetina, gymnema, açafrão e *Bacillus coagulans*.
- **Página:** https://mynuora.com/pages/gut-capsule.
- **Preço:** 1/2/3 meses a US$ 49 / 39 / 29 por unidade. As opções estavam marcadas "Unavailable" na leitura.
- **Histórico:**
  - Produto: ≥51 anúncios em 22 cards, todos com 30+ dias. Mais antigo: 1438360120994908, 2026-01-30, 291 dias.
  - **Marca, rolagem de 288 cards às ~19:35Z:** 379 anúncios, 269 cards com 30+ dias, mais antigo 782108268048154 (2025-10-08, 405 dias), Alicia Darling 152, Nuora 96, Dr. Destiny Robinson 27.
  - Meta ~1.800; Google ~800 (Lienov Solutions LLC).
- **Recorrência:** 2 cápsulas por dia, 30 porções (30 dias). Assinatura `alegada` ("Automatic refills", "Manage Subscription").
- **Classificação:** `evidencia_de_tracao` · `prioridade_media`. O produto específico ficou abaixo de 100 na amostra disponível.
- **Confiança:** baixa (IDs da rolagem perdidos).
- **Riscos altos:**
  - Calculadora "you could lose up to 24lbs in 3 months" e "mimics GLP-1".
  - Depoimentos com imagens rotuladas como geradas ou editadas por IA.
  - Prova social inconsistente (524k vs 32k).
  - Doses divergentes entre a tabela e o texto.

### Oferta 8 — Primal Viking: Ancestral Testosterone Booster

- **Categoria:** testosterona e libido masculina, 30–55+.
- **Fórmula:** blend proprietário de 337,5 mg (fígado, coração e rim de rena, testículo bovino) mais rhodiola 33,75 mg.
- **Página:** https://primalviking.com/products/primal-reindeer-testosterone-support.
- **Preço (assinatura):**
  - US$ 25/pote no Buy 1 Get 1.
  - US$ 23,33/pote no Buy 2 Get 3.
  - US$ 20/pote no Buy 4 Get 5.
  - "72% OFF on subscription" e "+609k JARS SOLD" (autodeclarado).
- **Histórico:**
  - ≥78 anúncios em 67 cards; 49 com 30+ dias.
  - Mais antigo: 952973200670606, 2026-05-21, 180 dias.
  - Meta ~2.800 (domínio); Google 0.
  - 41 textos distintos.
- **Recorrência:** 2 cápsulas por dia, 48 cápsulas: **24 dias (cálculo)**. Assinatura **verificada**.
- **Classificação:** `sinais_de_atividade` · `prioridade_media`.
- **Riscos:** "94% increased their testosterone", "Testosterone Tripled", hook de tamanho peniano, produto de órgãos animais (origem e importação).

### Oferta 9 — SPNutrition: Magnesium Bisglycinate Gummies

- **Categoria:** sono, estresse e cortisol (mulheres e homens 40+).
- **Fórmula:** 400 mg de bisglicinato de magnésio por 2 gomas; 30 porções; sem açúcar.
- **Página:** https://spnutrition-us.com/products/maximum-absorption-magnesium-bisglycinate-gummies. O site bloqueia o navegador automatizado ("using browser developer tools is not permitted"). O bloqueio não foi contornado; os dados vieram de web-fetch parcial.
- **Preço:** não observado. Promoção "Buy 3 Magnesium Bags Get Free D3 + K2".
- **Histórico:**
  - ≥72 anúncios do magnésio em 42 cards; 34 com 30+ dias.
  - Mais antigo: 863178650084986, 2026-03-06, 256 dias.
  - Marca: ≥109 anúncios; Meta ~4.900; Google ~200 (Ecom Victory LLC).
- **Recorrência:** 30 dias. Assinatura `alegada` ("Auto Refills Ship Every 30 Days"). O anúncio oferece rota "without a subscription".
- **Classificação:** `evidencia_de_tracao` · `prioridade_media`.
- **Riscos:**
  - Hook com narrativa sexual explícita.
  - "Safe … alongside your medication".
  - "Absorption jumps to around 90%" sem fonte.
  - Aviso FDA não observado.

### Oferta 10 — Nutrition Therapy: Oil of Oregano Drops

- **Categoria:** diarreia crônica, IBS-D e SIBO.
- **Página:** https://nutritiontherapy.co/products/oil-of-oregano.
- **Preço:** US$ 31,99/frasco; bundles de US$ 62,99 e US$ 94,99; "20% off automatic refills / Refills Every 30 Days".
- **Garantia:** 60 dias.
- **Histórico:**
  - ≥79 anúncios em 25 cards, **todos com 30+ dias** (90–179: 17).
  - Mais antigo: 1045429338426637, 2026-06-26, 144 dias.
  - Meta ~320; Google 0.
  - Persona "Carol Warren" (68 anúncios).
- **Recorrência:** "2 dropperfuls daily (2mL)", 60 mL = 30 dias (afirmado pela página). Assinatura **verificada**.
- **Classificação:** `sinais_de_atividade` · `prioridade_media`.
- **Riscos:** "The Most Effective Gut-Healing Formula Ever Created", "SIBO-Targeted" (tratamento de doença) e narrativa de que médicos "escondem" a causa.

## Oportunidades para investigação criativa posterior

1. **Rosabella:** ficção longa ("Nine Words, a Gravel Lane…") por mais de 15 páginas-persona; 55 textos distintos. Vale mapear a estrutura narrativa e o ponto de transição para o produto.
2. **Avantera / Philsmypharmacist:** vídeo de criador farmacêutico ativo desde 2024-06. Vale estudar o roteiro de longevidade e a credencial.
3. **Happy V:** UGC de criadoras e obgyn.mom. Vale mapear como o tema íntimo é abordado sem violar política.
4. **Nuora:** vídeos de confissão ("I need to publicly apologize… because I lied"), de 1 a 4 minutos.
5. **Nutrition Therapy:** histórias médicas em primeira pessoa (navio de cruzeiro, "nunca foi IBS-D") com longevidade de 90+ dias.
6. **Lovy:** depoimento único com muitas variações e hook de histerectomia, um subnicho específico.

Use o `creative-reference-analyst` só com acesso legítimo ao player, sem baixar nem republicar.

## Candidatos não selecionados (fora do top 10)

| Marca — produto | Dados (Meta, 2026-11-17, pisos) | Motivo |
|---|---|---|
| Nuora — Feminine Balance Gummies (1B CFU, 60 gomas) | ≥43 anúncios (39 cards), 37 com 30+ dias, mais antigo 404 dias | Mesma marca da oferta 7 e mesma categoria da 1 |
| Akka Superbiotics — Akkermansia + silimarina (fígado) | ≥70 (26 cards), mais antigo 107 d; Meta ~330; Google ~700 | Média; alegações de altíssimo risco ("natural replacement for Ozempic", "death is inevitable") |
| STĒLO — Stream (equol, próstata) | ≥57 (39 cards), mais antigo 267 d | Mesma categoria de ProstaGenix; alegações de PSA/DHT |
| OMNI Creatine | ≥76 (50 cards), mais antigo 225 d | Mesma categoria de Crave |
| Everyday Dose — café de cogumelos | ≥113 (50 cards), só 14 com 30+ d; Google ~600 | Bebida funcional; picos de Black Friday |
| The Standard Lab — NAC + NAD (fígado) | ≥68 (33 cards), mais antigo 61 d; Google ~200 | Recente |
| Uromend — próstata/bexiga | ≥65 (58 cards), 45 com <30 d; Google 81 | Entrada recente; terceira oferta de próstata |
| Bloomin — gomas femininas | ≥38 (13 cards), mais antigo 157 d | Aparece em várias buscas femininas; monitorar |
| Reliva — zumbido | 45 cards, 0 com 30+ d | `em_observacao`, possivelmente **emergente**; produto não confirmado como suplemento |

## Excluídos por deduplicação

- **Metabolae** (canela-do-ceilão; ≥892 anúncios, maior volume visto): já está na base `knowledge/referencias/canela-ceilao-2026-11-17/`.
- **Missão de articulações** (results/2026-11-17_articulacoes-eua): Arthrogenix, VitalHydra, Nova, Haka, Ilyra, BioRoot, GoodGrove, Plants Basically, Regensil, Collanol, Halsten, OsteoShield.
- **Black Girl Vitamins:** citada na missão anterior.

## Fora de escopo

| Marca — produto | Categoria | URL | Motivo |
|---|---|---|---|
| Dova — dispositivo para zumbido | dispositivo | https://dovaonline.store/products/struggling-with-constant-ringing-even-though-your-hearing-test-came-back-normal | "This revolutionary device" |
| Hey Erth, nama, BATCH — gomas para sono | canabinoides (THC/CBN/CBD) | https://erthwellness.com/products/sleep-gummies-cbn-thc-live-resin-750mg | regime regulatório distinto |
| Nutrafol, Keeps, hims | cabelo / medicamento | — | medicamentos ou marcas de varejo consolidadas |
| Canine Drops, Chewy, Paw Balance | pet | — | público animal |

## Recomendações de aprofundamento

1. **Refazer as contagens com paginação** (Meta logada no navegador do Orca, por decisão do usuário, ou em outro horário). Prioridade: Avantera, Crave, Primal Viking, SPNutrition e Nuora. Os contadores de ~360 a ~4.900 sugerem que vários pisos médios podem passar de 100.
2. **Recuperar os IDs da Nuora** e dividir os anúncios por produto (Gut Ritual × Feminine Balance).
3. **Abrir os anúncios mais antigos** (IDs acima) para checar plataformas e possíveis reativações.
4. **Confirmar no checkout, sem comprar,** as assinaturas `alegada` (Lovy, Avantera, Nuora, SPNutrition) e o valor real do refil da Lovy.
5. **Google Ads Transparency de tryrosabella.com** e do domínio final da loja Rosabella.
6. **Monitorar Reliva e Uromend** em 2–4 semanas para confirmar se são emergentes.
7. **Revisão regulatória obrigatória** antes de qualquer transferência de ângulo: próstata (DE/HPB), GLP-1/peso, ITU, SIBO e pressão arterial.

## Limitações de acesso e de confiabilidade

- **Paginação da Meta indisponível sem login a partir de ~19:55 UTC.** Não foi contornada. Todas as contagens são pisos e `count_is_estimate = true`.
- **Faixas de idade** contam cards. A ordem de exibição da Meta não é cronológica, então o "mais antigo" só vale para a amostra.
- **Fora da UE**, anúncios comerciais inativos não aparecem; o histórico pode estar truncado.
- **Google Ads Transparency:** contador por domínio em "Qualquer horário", incluindo anúncios inativos.
- **SPNutrition** bloqueia ferramentas de navegador automatizado; as leituras de 4 páginas vieram de web-fetch, com parte em resumo do subagente (marcado nas fichas).
- **Requisições diretas** aos endpoints JSON do Shopify foram negadas pelo controle de permissões e não foram usadas.
- **Não usados:** TikTok Creative Center, transcrição e download de vídeos.
- **Prova social** (avaliações, "X customers", "jars sold") é sempre autodeclarada e não foi verificada.

## Arquivos

- `offers.json`: índice estruturado com 10 ofertas, candidatos não selecionados, fora de escopo, exclusões por deduplicação e limitações.
- `data/ads_<oferta>.csv`: IDs da Meta Ad Library por oferta, com início, idade, nº de variações, página, destino e URL.
- `data/agg_<oferta>.json`: agregados por oferta e por marca (método, regex de filtro, faixas de idade, páginas, destinos).
- `data/queries_log.tsv`: 58 buscas na Meta, com contador da fonte, nº de cards e horário.
- `data/google_ads_transparency.tsv`: 14 domínios.
- **Evidências locais, fora do Git:** `evidence-local/eua-aberta-2026-11-17/`. Contém o JSON bruto das buscas e o markdown das páginas de venda em `pages/`.
