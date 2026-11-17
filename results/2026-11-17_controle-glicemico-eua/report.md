# Relatório da missão 003: suplementos para controle glicêmico — EUA

## Escopo e execução

- **Data de execução (UTC):** 2026-11-17, das 20:50 às 21:35. As buscas na Meta Ad Library foram feitas entre 20:52 e 21:23 UTC. As páginas de venda foram lidas entre 21:12 e 21:29 UTC.
- **Missão de origem:** Missão 003. Pedido: até 10 ofertas de suplementos para controle de açúcar no sangue nos EUA, com descoberta livre de mecanismo, em inglês e espanhol, e pesquisa aprofundada.
- **Mercado de venda:** Estados Unidos. Filtros usados: `country=US` na Meta Ad Library e `region=US` no Google Ads Transparency.
- **Problema:** controle glicêmico e metabolismo da glicose. Os subnichos pedidos foram explorados: blood sugar support, healthy glucose, glicemia pós-refeição/picos, resistência à insulina, saúde metabólica, desejo por açúcar, pré-diabetes, metabolismo feminino, berberina, canela-do-ceilão e cromo. Também entraram mecanismos encontrados durante a pesquisa: GLP-1 natural, di-hidroberberina, gotas sublinguais, chás funcionais, gymnema, melão-de-são-caetano, nopal e inositol.
- **Idiomas pesquisados:** inglês e espanhol (público hispânico dos EUA).
- **Ferramentas realmente usadas:**
  - Navegador embutido do Orca, sem login, para Meta Ad Library, Google Ads Transparency, páginas de venda e Amazon.
  - Script local que lê os cards exibidos: ID, data "Veiculação iniciada em", página, nº de anúncios que usam o criativo, link de destino e texto.
  - Capturas de tela guardadas em `evidence-local/glicemia-eua-2026-11-17/`, fora do Git.
  - Não foram usados WebSearch, TikTok Creative Center, transcrição de áudio nem download de vídeos.
- **Limites de pesquisa:**
  - 43 buscas por palavra-chave (descoberta temática e nomes de marca) e 43 buscas por frase exata (domínio, marca ou produto), num total de 86 consultas únicas registradas em `data/queries_log.tsv`.
  - 14 consultas ao Google Ads Transparency (`data/google_ads_transparency.tsv`).
  - 19 páginas de venda, advertoriais ou Amazon abertas.
- **Parâmetros de priorização:** padrão de `docs/prioritization-criteria.md`.
  - Idade mínima relevante: 30 dias.
  - Faixas: alta ≥ 100, média 20–99 e observação < 20 anúncios ativos da oferta.
  - Categoria: suplementos consumíveis.
- **Limitação central desta missão:** a Meta bloqueou a paginação. O botão "Ver mais" devolvia `{"errors":[{"message":"Rate limit exceeded","code":1675004}]}`. A restrição não foi contornada. Por isso:
  - cada consulta mostra só a **1ª página**, com até 30 cards ordenados por impressões;
  - o volume da oferta usa o **contador "~N resultados" da própria Meta**, que é uma estimativa (`count_is_estimate: true`);
  - longevidade e faixas de idade valem **só para a amostra**. O "anúncio ativo mais antigo" é o mais antigo *observado*, e pode haver anúncios mais antigos fora da amostra.
- **Motivo do encerramento:**
  - 10 ofertas distintas documentadas com evidência mínima.
  - As últimas 10 buscas por palavra-chave trouxeram só candidatos com < 30 anúncios ou fora do problema.
  - A paginação seguiu bloqueada nas novas tentativas, às 21:08 e 21:23.

## Resumo executivo

- **Candidatos de suplemento para glicemia identificados:** 22, sem contar as referências conhecidas. Ficaram 10 no relatório principal. 9 foram registrados como "não selecionados" e 6 marcas ou grupos como fora de escopo.
- **Ofertas com evidência mínima:** 10.
- **Por prioridade:** alta 4 · média 5 · em observação 1. Há 2 emergentes: PureCeylon (alta, entrada recente forte) e True Nutra (em observação).
- **Referências excluídas do ranking, conforme a missão:**
  - **Metabolae** é o anunciante dominante do tema: 352 anúncios, incluindo variações, só nos cards de descoberta, presentes em 23 das 43 buscas por palavra-chave.
  - **Resilia** apareceu em "glucose spikes", "post-meal" e "nature's ozempic".
  - Gentilia, Liréa e Kenzendo não apareceram no filtro EUA.
- **Padrões principais:**
  1. **Família white-label "Ceylon Cinnamon 7200mg Equivalent with MCT Oil" (12:1 + MCT, softgel).** O produto tem nome idêntico em Metabolae, Resia e Liraé, e a mesma fórmula na PureCeylon (ES). Somam-se Gentilia (IT), Liréa (FR) e Kenzendo (JP), já nas referências. É o subnicho com mais volume e com a oferta mais longeva: Liraé tem anúncio ativo desde 04/09/2025.
  2. **Scripts compartilhados entre marcas:**
     - "X was created for people who've tried everything to manage their blood sugar—and still feel like they're fighting a losing battle…" aparece em Metabolae, Resia e Liraé.
     - "Please don't buy X…" aparece em Metabolae e Resia.
     - "Tu azúcar estará equilibrada, tus antojos desaparecerán…" aparece em Glucora (ES) e, traduzido, em True Nutra (EN).
     - PureCeylon e Nervora usam o mesmo template de página de venda.
  3. **Berberina como "Ozempic natural / GLP-1 natural"** é o subnicho com **mais anunciantes distintos** (GLOV, Sandhu Sangluco, JSHealth, Santo Remedio, Ovia, Gratitude Health, IM8, Nature's Bounty, Kind Patches). Mas o volume por oferta é menor, e o posicionamento se mistura com perda de peso e desejo por açúcar.
  4. **Mercado hispânico dos EUA** com ofertas próprias e longevas (Glucora 251 d) e entradas recentes fortes (PureCeylon, Nervora). Há copy espelhada entre ES e EN.
  5. **Estrutura comercial padrão:** 1 / 2+1 / 3+2 (ou 1+1 / 2+3 / 3+5 nas gotas), garantia de 30–90 dias que "reembolsa embalagens vazias" e assinatura mensal.
- **Lacunas:**
  - Contagens completas e auditadas indisponíveis por causa do bloqueio de paginação.
  - Página da GLOV bloqueada para a região.
  - Ovia sem página de venda ativa.
  - Sem TikTok.
  - Sem histórico de anúncios inativos, porque a Meta não os mostra fora da UE.

> Prioridade ordena a investigação. Quantidade e idade de anúncios **não** indicam vendas, investimento ou lucro.

---

## Ranking A — Subnichos e mecanismos

A ordem combina três critérios:

- **força das evidências publicitárias:** volume da oferta e longevidade observada;
- **concorrência:** nº de anunciantes de suplemento distintos na 1ª página das buscas;
- **potencial de recompra.**

Os contadores das buscas temáticas incluem anúncios fora de suplementos (apps, CGMs, clínicas) e servem só como termômetro do tema.

| # | Subnicho / mecanismo | Contador Meta (buscas temáticas, estimativa) | Ofertas de suplemento observadas | Volume / longevidade das ofertas | Recompra | Leitura |
|---|---|---|---|---|---|---|
| 1 | **Canela-do-ceilão 12:1 + MCT (softgel 7.200 mg eq.)** | "ceylon cinnamon" ~29.000; "cinnamon MCT" ~24.000; "7200mg" ~19.000; "canela de ceilán" ~1.600 | Metabolae (ref.), Resia, Liraé, PureCeylon; Resilia (ref., outra fórmula) | Resia ~2.000; Liraé ~380–450 com mais antigo de **439 d**; PureCeylon ~240 | 1 softgel/dia, frasco de 30 d, kits de 90–150 d, assinatura | Maior volume e longevidade. Alta concentração de clones: fórmula, nome e copy iguais. Diferenciação baixa |
| 2 | **Berberina / "Ozempic natural" / GLP-1 natural** (inclui di-hidroberberina) | "berberine" ~23.000; "nature's ozempic" ~17.000; "natural GLP-1" ~7.200; "berberina" ~2.200; "dihydroberberine" ~620; "liquid berberine" ~750 | GLOV, Sangluco, JSHealth, Santo Remedio, Ovia, Gratitude Health, IM8, Nature's Bounty, Nuora (missão 001), Kind Patches (adesivo) | GLOV ~2.800 (nome) com 127 d; Ovia 182 d; Sangluco ~49 com 181 d; JSHealth ~63 com 104 d | 2 cáps./dia, 30 d, assinatura comum | Mais anunciantes distintos. Mistura glicemia, peso e desejo por açúcar. Risco regulatório alto (comparação com GLP-1) |
| 3 | **Gotas sublinguais multi-ingrediente** (berberina + canela + cromo + gymnema + melão-de-são-caetano…) | "gotas glucosa" ~27; "blood sugar drops" ~17.000 (dominado por Metabolae) | Glucora (ES), True Nutra (EN) | Glucora ~140–150 com **251 d**; True Nutra recente (41 d) | 2 mL/dia; 1 frasco ≈ 1 mês (Glucora); 15 d (True Nutra) | Formato diferenciado (líquido, "absorção"). Transferência ES → EN em curso |
| 4 | **Chás funcionais para glicemia** | "blood sugar tea" ~11.000 (dominado por Metabolae/PiPi Tea) | Herbaly Glucose Tea, Dr. Eve Sugar Cutting (KR); PiPi Tea (colesterol, fora de escopo) | Herbaly ≥23 cards, todos com 30+ d (182 d); Dr. Eve ~22–30 (62 d) | 28 sachês = 14 d (Herbaly) | Volume menor e longevidade boa. Categoria limítrofe (chá) |
| 5 | **Complicações do diabetes** (neuropatia com R-ALA/complexo B; DE diabética) — adjacente | "diabetes natural" ~18.000; "metformin" ~18.000 | Nervora (ES), Noverly, TryNuvel, Omvyra, Aurivita | Nervora ~550 (48 d); Noverly ~9.600 (multi); TryNuvel ~1.100 (82 d) | Diária | Muita atividade recente; usa diabetes como gancho para outro problema. Fora do núcleo |
| 6 | **Desejo por açúcar / apetite (mulheres 40+, perimenopausa)** | "sugar cravings" ~22.000; "blood sugar menopause" ~10.000 | Ovia, GLOV ("Metabolism After 40"), Kind Patches, Absorb WLP-1, Bioma | Ovia 142 anúncios na amostra (página fora do ar) | Diária | Forte em anúncios, mas a fronteira com emagrecimento é difusa |
| 7 | **Resistência à insulina / SOP / saúde metabólica feminina** | "insulin resistance" ~12.000; "inositol" ~4.300; "resistencia a la insulina" ~7.500 | Black Girl Vitamins, Daily Curb, Serelia (cortisol + mio-inositol, ES), arrae | Poucos anúncios por produto, ou recentes (Daily Curb < 30 d) | Diária | Fragmentado; mais conteúdo médico e clínicas que ofertas |
| 8 | **Picos pós-refeição / bloqueador de carboidrato** | "glucose spikes" ~4.400; "post-meal" >50.000 (genérico) | CleverPro Carbivore, GOOD IDEA (bebida) | ~20 e ~6 anúncios, recentes | Por refeição | Dominado por CGMs (Dexcom, Stelo, Signos). Emergente |
| 9 | **Pré-diabetes** | "prediabetes" ~3.100; "diabetes tipo 2" ~500 | — (aparece como gancho em Liraé, Resia, Glucora) | — | — | Anúncios institucionais (CDC/Ad Council, Cruz Vermelha, clínicas). Não é categoria de produto |
| 10 | **Cromo isolado** | "chromium picolinate" ~600 | Nenhuma oferta isolada; cromo aparece em blends (Sangluco, Glucora, Ovia) | — | — | Ingrediente de apoio, sem oferta própria observada |

**Ingredientes com mais atenção publicitária (frequência nos cards de descoberta e nas fórmulas):** canela-do-ceilão (12:1 + MCT), berberina e di-hidroberberina, melão-de-são-caetano, cromo, gymnema, vinagre de maçã, cúrcuma, R-ácido alfa-lipoico (neuropatia), inositol (SOP) e chás com banaba, tupinambo e oolong.

---

## Ranking B — As 10 ofertas mais relevantes

| # | Marca — produto | URL | Prioridade | Anúncios ativos da oferta (estimativa Meta) | Amostra: cards (anúncios c/ variações) · 30+ d | Mais antigo observado | Ativos marca/domínio | Mecanismo | Recorrência / assinatura | Evidência | Fonte e data |
|---|---|---|---|---|---|---|---|---|---|---|---|
| 1 | Resia — Ceylon Cinnamon 7200mg Eq. + MCT | https://tryresia.com/products/ceylon-cinnamon-7200mg-equivalent-with-mct-oil | **prioridade_alta** | ~2.000 | 30 (37) · 29 | 173 d (28/05/2026) | ~2.000; Google 90 (OneStopMrkt LLC) | Ceilão 12:1 + MCT, "absorção", Cássia × Ceilão | 30 softgels = 30 d; 2+1 / 3+2 · alegada | sinais_de_atividade | Meta "tryresia.com", 2026-11-17 21:03Z/21:23Z |
| 2 | Liraé — Ceylon Cinnamon 7200mg Eq. + MCT | https://getlirae.com/products/ceylon-cinnamon-7-200mg | **prioridade_alta** | ~380–450 | 33 (33) · 30 (23 com 180+) | **439 d** (04/09/2025) | ~380–450; Google 200 (Tanvin Joy) | Ceilão 12:1 + MCT; "antes da insulina" | 30 / 90 / 150 Day Supply · verificada | sinais_de_atividade | Meta "getlirae.com" e "Liraé", 21:08Z/21:22Z |
| 3 | Glucora Lab — Glucora (gotas, ES) | https://glucora-lab.com/products/glucora | **prioridade_alta** | ~140–150 | 28 (31) · 27 | 251 d (11/03/2026) | ~140; Google 16 (DOMINUS ECOM LLC) | Gotas sublinguais; berberina + 6 ervas/minerais | 2 mL/dia; 1+1 = 2 meses · verificada (15%) | sinais_de_atividade | Meta "glucora-lab.com" e "Glucora", 21:00Z/21:21Z |
| 4 | PureCeylon — Controla tu Azúcar (ES) | https://pureceylon.co/products/controla-tu-azucar-canela-de-ceilan-concentrada-12-1-con-aceite-mct | **prioridade_alta** (emergente) | ~240 | 30 (34) · 14 | 54 d (24/09/2026) | ~240; Google 0 | Ceilão 12:1 + MCT em espanhol | 1 softgel/dia; recarga a cada 30 d · verificada | sinais_de_atividade | Meta "pureceylon.co" e "PureCeylon", 21:04Z/21:22Z |
| 5 | GLOV — Berberine Complex | https://glovbeauty.com/products/berberine-complex-cellular-energy-metabolism-support | prioridade_media | ~2.800 (busca pelo nome) | 31 (34) · 25 | 127 d (13/07/2026) | ~13.000 (multiproduto); Google 200 | Berberina + cofatores; mulheres 40+, desejo por açúcar | página bloqueada · nao_observada | sinais_de_atividade | Meta "GLOV Berberine", 21:20Z |
| 6 | Sandhu's — Sangluco Berberine Complex | https://www.amazon.com/dp/B0FXNQY3H3 | prioridade_media | ~49 | 30 (30) · 9 | 181 d (20/05/2026) | marca também anuncia produto articular; Google 0 (gosandhus.com) | Berberina + Ceilão + cromo + melão-de-são-caetano + cúrcuma + vinagre de maçã; "Ozempic natural" | 60 cáps., 2/dia = 30 d · verificada (Amazon S&S) | **evidencia_de_tracao** ("3K+ bought in past month") | Meta "Sangluco", 21:08Z |
| 7 | JSHealth Vitamins — Berberine+ Formula | https://us.jshealthvitamins.com/products/berberine-formula | prioridade_media | ~63 | 29 (40) · 14 | 104 d (05/08/2026) | ~30 no domínio; Google 12 | Berberina; criadoras de conteúdo | 1 Month Supply; 2 cáps./dia · verificada | sinais_de_atividade | Meta "JSHealth Berberine", 21:23Z |
| 8 | Herbaly — Glucose Functional Tea | https://herbaly.com/pages/glucose-tea-a | prioridade_media | ≥23 cards observados ("Glucose tea" ~19) | 23 (23) · 23 | 182 d (19/05/2026) | ~220; Google 38 | Chá de 12 ervas; "double grams" | 28 sachês, 2/dia = 14 d; 3+3 = 84 d · verificada | sinais_de_atividade | Meta "herbaly.com" e "Glucose tea", 21:10Z/21:20Z |
| 9 | Dr. Eve — Sugar Cutting Tea (KR) | https://www.dreveus.com/pages/amazon-sugar-cutting | prioridade_media | ~22–30 | 29 (30) · 27 | 62 d (16/09/2026) | ~22; Google 0 | Chá coreano (banaba, melão-de-são-caetano, tupinambo, hortênsia) | dose/unidades não vistas · nao_observada | sinais_de_atividade | Meta "dreveus.com", 21:03Z |
| 10 | True Nutra — 7-in-1 Blood Sugar Complex | https://truenutra.com/products/fb-en-bsc003 | em_observacao (**emergente**) | ≥8 cards observados | 8 (8) · 2 | 41 d (07/10/2026) | ~1.900 (multiproduto); Google 300 (R5 Brands LLC) | Gotas de complexo de berberina; copy da Glucora em inglês | 15 mL = 15 d · verificada | sinais_de_atividade | Meta "truenutra.com", 21:18Z |

Notas:

- "Anúncios ativos da oferta" vem do contador aproximado da Meta para a consulta indicada. Nas ofertas de domínio de produto único (1–4), toda a amostra levava ao produto. Nas marcas com vários produtos (5, 10), o contador da marca não foi atribuído à oferta.
- Os dados por anúncio estão em `data/ads_<oferta>.csv` e os agregados em `data/agg_<oferta>.json`.

---

## Consultas realizadas (resumo)

O log completo, com URL e horário de cada consulta, está em `data/queries_log.tsv`.

| Idioma | Busca (Meta, palavra-chave) | Contador | Principais suplementos na 1ª página |
|---|---|---|---|
| EN | blood sugar support | ~44.000 | Metabolae (dominante), PiPi Tea, Sangluco |
| EN | healthy glucose | ~22.000 | Metabolae, Liraé, Sangluco |
| EN | glucose spikes | ~4.400 | Metabolae, Resilia, Nuora, Dr. Eve; Dexcom (fora) |
| EN | insulin resistance | ~12.000 | Liraé, Black Girl Vitamins, Evident; Power Plate (fora) |
| EN | prediabetes | ~3.100 | institucionais (Cruz Vermelha, "Do I Have Prediabetes", clínicas) |
| EN | sugar cravings | ~22.000 | Nuora, Kind Patches, Ovia, GLOV, Goli |
| EN | berberine | ~23.000 | Metabolae, Sangluco, Nuora, Kind Patches, IM8, Nature's Bounty |
| EN | ceylon cinnamon | ~29.000 | Metabolae, Liraé, Resia, Sangluco |
| EN | A1C | >50.000 | Metabolae; personas sem link (lead forms) |
| EN | natural GLP-1 / nature's ozempic | ~7.200 / ~17.000 | Sangluco, Ovia, JSHealth, Absorb WLP-1, Bioma, Kind Patches |
| EN | chromium picolinate | ~600 | Kind Patches, Transparent Labs, Santo Remedio |
| EN | gymnema / bitter melon | ~1.700 / ~2.600 | Herbaly, GLOV, Glucora, Sangluco, Dr. Eve |
| EN | metformin | ~18.000 | Metabolae, Aurlux (fora), PiPi Tea |
| EN | blood sugar menopause | ~10.000 | Ovia, Nuora, SPN, Mykalm |
| EN | 7200mg / cinnamon MCT | ~19.000 / ~24.000 | Metabolae, Resia, Liraé |
| EN | Sugar Defender / GlucoTrust / Glucoberry | ~140 / ~22 / 0 | Ofertas clássicas de afiliado praticamente ausentes no Meta EUA; os resultados de "GlucoTrust" eram redes de "diabetic man" (Nervora, Omvyra, Aurivita, Noverly) e um link hop.clickbank (GlucoTonic) |
| EN | inositol / insulin | ~4.300 / ~44.000 | Black Girl Vitamins, arrae, Aurlux; Omnipod (fora) |
| EN | glucose support / post-meal / sugar balance | ~18.000 / >50.000 / ~24.000 | Metabolae, Resilia, Sangluco, Liraé, GOOD IDEA |
| EN | blood sugar drops / tea / gummies | ~17.000 / ~11.000 / ~5.000 | Metabolae, PiPi Tea, SPN, Ovia, Resilia |
| EN | dihydroberberine / liquid berberine | ~620 / ~750 | WonderBiotics, Gratitude Health, IM8, Glucora, True Nutra, Kind Patches |
| ES | azúcar en la sangre / glucosa | ~4.200 / ~2.700 | Glucora, Sangluco (ES), Santo Remedio; apps (fora) |
| ES | berberina / canela de ceilán | ~2.200 / ~1.600 | Glucora, Serelia, Metabolae (ES), PureCeylon |
| ES | diabetes natural / diabetes tipo 2 | ~18.000 / ~500 | Metabolae (Dr. Juan Castillo), Glucora, Mama Bear Oasis (neuropatia) |
| ES | gotas glucosa | ~27 | PureCeylon, Glucora, TryNuvel, esencialluz.es (cópia da Glucora) |
| ES | resistencia a la insulina / azúcar alta | ~7.500 / ~1.700 | clínicas, Evident (SOP), Clínicas del Azúcar |

O Google Ads Transparency (região EUA, por domínio, 21:2x UTC) está em `data/google_ads_transparency.tsv`:

| Domínio | Contagem | Anunciante |
|---|---|---|
| truenutra.com | 300 | R5 Brands LLC |
| misantoremedio.com | 300 | Santo Remedio LLC |
| getlirae.com | 200 | Tanvin Joy |
| glovbeauty.com | 200 | GLOV BEAUTY LLC |
| metabolae.com | 200 | BAT Partners LLC |
| tryresia.com | 90 | OneStopMrkt LLC |
| oviaessentials.com | 43 | Dextris LLC |
| herbaly.com | 38 | Herbaly Marketplace Inc. |
| glucora-lab.com | 16 | DOMINUS ECOM LLC |
| jshealthvitamins.com | 12 | JSHealth Vitamins US, Inc. |
| pureceylon.co, gosandhus.com, dreveus.com, mynervora.com | 0 | — |

---

## Ofertas investigadas

### Oferta 1 — Resia: Ceylon Cinnamon 7200mg Equivalent with MCT Oil

- **Mercado de venda:** EUA, em inglês.
- **Origem da marca:** desconhecida. No Google Ads Transparency, o anunciante verificado é OneStopMrkt LLC.
- **Problema e público:** glicemia alta, pré-diabetes e diabetes tipo 2; adultos 50+.
- **Mecanismo alegado no marketing:**
  - canela-do-ceilão verdadeira × cássia, que teria cumarina e faria mal ao fígado;
  - extrato 12:1 equivalente a 7.200 mg em 1 softgel;
  - MCT como veículo de absorção;
  - "help your cells respond to insulin".
- **Página:** https://tryresia.com/products/ceylon-cinnamon-7200mg-equivalent-with-mct-oil (2026-11-17 21:12Z)
- **Preço:**
  - 1 unidade: $29.99 (de $59.99);
  - Buy 2 Get 1: $54.99;
  - Buy 3 Get 2: $79.99.
  - Garantia de 90 dias, inclusive para embalagens vazias.

#### Histórico publicitário

- **Consultas na Meta:**
  - frase exata "tryresia.com": ~2.000, às 21:03Z e 21:23Z;
  - "Resia": ~1.900, às 21:22Z.
- **Método:** amostra da 1ª página, 30 cards (37 anúncios com variações), com `count_is_estimate: true`.
- **Faixas de idade da amostra:** < 30 d: 1 · 30–59 d: 13 · 60–89 d: 7 · 90–179 d: 9 · 180+ d: 0.
- **Mais antigo observado:** `1220457543389037`, iniciado em 28/05/2026, com 173 d.
- **Produto específico:** 30/30 cards levam ao produto, incluindo `/pages/advertorial-resia` e a variante `-cc`.
- **Páginas anunciantes:**
  - Resia 18;
  - Try Resia 5;
  - personas: Sarah Collins 2, Linda Marsh RN, Paul Mitchell, Sarah Peekmill, Melissa Burkens, Robert Mitchell.
- **Criativos únicos (texto) na amostra:** 13.
- **Google Ads Transparency:** 90 anúncios, OneStopMrkt LLC.

#### Recorrência

- **Tipo:** `consumivel_recorrente`.
- **Dose e unidades:** 1 softgel por dia. Um anúncio da marca (12/10/2026) diz "Real Resia comes with thirty softgels".
- **Duração calculada:** 30 unidades ÷ 1 por dia = **30 dias**. Kits de 90 e 150 dias.
- **Assinatura:** `alegada`. Só há o link "Manage Subscription"; a opção não aparece no seletor de compra.
- **Potencial de recompra (inferência):** alto.

#### Criativos

- **Ganchos observados:**
  - "Please don't buy Resia…" (persona educadora em diabetes);
  - "I'm a nurse with type 2 diabetes. I refused Metformin for 14 months";
  - lista Cássia × Ceilão com ❌;
  - ancoragem de preço "Two bags is $59.98. Three bags is $54.99";
  - "They refund the empty pouches";
  - alerta "If you … are taking it three times a day, STOP!".
- **Formatos:**
  - estático "A1C 5.9 → NOW WHAT?";
  - foto de caixa "FLASH SALE";
  - vídeo de produto (captura `meta_tryresia.com.png`).
- **Copy compartilhada:** "Resia was created for people who've tried everything…" é idêntica à de Metabolae e Liraé.

#### Classificação

- **Evidência:** `sinais_de_atividade`.
- **Prioridade:** `prioridade_alta`, com contador ~2.000 (estimativa), 29 de 30 cards com 30+ d e uso diário.
- **Confiança:** moderada.
- **Regulatório:** alegações sobre insulina, A1C e metformina sugerem efeito de tratamento. Verificar também se as personas "RN" e educadora são reais.

### Oferta 2 — Liraé: Ceylon Cinnamon 7200mg Equivalent with MCT Oil

- **Mercado de venda:** EUA, em inglês. A página tem seletor de muitos países, todos em USD.
- **Anunciante no Google:** Tanvin Joy (200 anúncios).
- **Página:** https://getlirae.com/products/ceylon-cinnamon-7-200mg (21:12Z)
- **Preço:**
  - 30 Day Supply: $29.99 (de $59.99);
  - Buy 2 Get 1 (90 Day Supply): $54.99;
  - Buy 3 Get 2 (150 Day Supply): $79.99.
  - Garantia de 30 dias.
  - "Save More with Automatic Refills!" e "Subscription Portal" no menu.
- **Mecanismo:** igual ao da Resia. Ângulo próprio: "90 days before insulin becomes the next step" e "Natural Support Before Insulin Becomes Necessary".

#### Histórico publicitário

- **Consultas na Meta:** "getlirae.com" ~380 (21:08Z) e "Liraé" ~450 (21:22Z).
- **Amostra:** 33 cards. Faixas de idade:
  - < 30 d: 3;
  - 30–59 d: 1;
  - 60–89 d: 1;
  - 90–179 d: 5;
  - **180+ d: 23**.
- **Mais antigo observado:** `775665505364183`, de **04/09/2025**, com **439 d**. Outros: 06/09/2025, 13/09/2025 e 19/10/2025.
- **Páginas:** Liraé 30 e "Honest Health Reviews" 3. Esta última leva a um advertorial em `bloodsugar.vitalydaily.org`, citado no anúncio.
- **Criativos únicos:** 9. Rotação baixa e criativos muito antigos ainda ativos.

#### Recorrência

- 1 softgel por dia; frasco de "30 Day Supply" (a página não mostra o número de unidades).
- Kits de 90 e 150 dias.
- **Assinatura:** `verificada` (opção de reposição automática no seletor).

#### Criativos

- vídeo com **animação 3D de vaso sanguíneo** ("in twelve weeks");
- vídeo de comida e açúcar;
- vídeo de calendário "Day 10";
- história de "Sarah, 58", com glicemia de 165 → 98 em 8 semanas (alegação).

#### Classificação

- **Evidência:** `sinais_de_atividade`.
- **Prioridade:** `prioridade_alta`. É a oferta com maior longevidade observada da missão.
- **Confiança:** moderada.
- **Atenção à deduplicação:** o nome lembra **Liréa** (França, referência anterior), mas o domínio, o mercado e a grafia são diferentes. Qualquer relação é **hipótese não verificada**. Se o usuário considerar as duas a mesma marca, Herbaly ou Dr. Eve sobem uma posição e o candidato seguinte é Ovia (ver "não selecionados").

### Oferta 3 — Glucora Lab: Glucora, gotas sublinguais para glicose (espanhol)

- **Mercado:** EUA, em espanhol, para público hispânico. Há uma cópia da copy em `esencialluz.es`.
- **Anunciante no Google:** DOMINUS ECOM LLC (16 anúncios).
- **Página:** https://glucora-lab.com/products/glucora (21:12Z)
- **Ingredientes listados (7):**
  - berberina;
  - canela-do-ceilão;
  - glucomanano;
  - melão-de-são-caetano;
  - Gymnema sylvestre;
  - picolinato de cromo;
  - cúrcuma.

  Anúncios e outra seção da página falam em **10** ingredientes. A inconsistência foi observada na própria página.
- **Dose:** 2 mL por dia, sob a língua.
- **Preços exibidos:**
  - Compra 1: $39.95 (de $59.90);
  - Compra 1 Recibe 1 ("Tratamiento 2 meses"): valor ambíguo na leitura ($39.95 / $119.80);
  - 2+3 ("5 meses"): $76.95;
  - 3+5: $109.95.
  - "Suscríbete y Ahorra 15% — Enviado mensualmente".
  - Garantia de 90 dias.

#### Histórico publicitário

- **Consultas na Meta:** "glucora-lab.com" ~140 (21:00Z) e "Glucora" ~150 (21:21Z).
- **Amostra:** 28 cards (31 anúncios). Faixas de idade:
  - < 30 d: 1;
  - 30–59 d: 2;
  - 60–89 d: 6;
  - 90–179 d: 18;
  - 180+ d: 1.
- **Mais antigo:** `3149105422144141`, de 11/03/2026, com 251 d.
- **Páginas:** Glucora Lab 13, "Comunidad Control Diabetes" 10 e Adriana Medina 5.
- **Destinos:** `/pages/glucora-listicle` 14, produto 11 e `/pages/adv1` 3.
- **Textos únicos:** só 2. A variação está na mídia.

#### Recorrência

- `consumivel_recorrente`.
- A página associa 2 frascos a 2 meses, o que sugere ~1 frasco por mês. O volume do frasco não foi observado.
- **Assinatura:** `verificada`.
- A página recomenda 6 meses de tratamento.

#### Criativos

- vídeo de jaleco "Cómo tomar berberina — por investigadora de cáncer";
- estático com glicosímetro antes/depois, "341 → 97: Miles ya bajaron su azúcar con Glucora";
- vídeo do frasco;
- CTA "Si tomas metformina mira esto";
- persona "ex-enfermera de UCI por 38 años".

#### Classificação

- **Evidência:** `sinais_de_atividade`.
- **Prioridade:** `prioridade_alta`. O volume está perto do limiar de 100 e depende do contador aproximado.
- **Confiança:** moderada.
- **Regulatório (grave):**
  - "¡Lleva tu diabetes a remisión!";
  - "su cuerpo aprendió a regularse solo";
  - orientação de uso junto com Metformina ou Mounjaro, com aviso de que "tu azúcar puede bajar más rápido". Há risco de hipoglicemia.

### Oferta 4 — PureCeylon: Controla tu Azúcar (canela-do-ceilão 12:1 + MCT, espanhol)

- **Mercado:** EUA, em espanhol. As páginas anunciantes incluem "Bienestar Latino USA".
- **Página:** https://pureceylon.co/products/controla-tu-azucar-canela-de-ceilan-concentrada-12-1-con-aceite-mct (21:12Z)
- **Preço:**
  - 1 unidade: $29.99 (de $39.99);
  - 2+1: $59.98;
  - 3+2: $81.00, com brindes.
  - "Recarga cada 30 días | Cancela cuando quieras".
  - Garantia de 90 dias.
- **Template de página** idêntico ao da Nervora (R-ALA, também em espanhol): mesmos preços $29.99 / $59.98 / $81.00 e o mesmo texto "Este producto se agotó 12 veces el año pasado…". Possível operador comum (hipótese).

#### Histórico publicitário

- **Consultas na Meta:** "pureceylon.co" ~240 (21:04Z) e "PureCeylon" ~240 (21:22Z).
- **Amostra da oferta:** 30 cards (34 anúncios). Faixas de idade:
  - < 30 d: 16;
  - 30–59 d: 14.
- **Mais antigo:** 24/09/2026, com 54 d.
- **Páginas:** Bienestar Latino USA 14, PureCeylon 6, Dr. Rafael Osorio 5 e "Yesenia Rodríguez, RN" 5.
- **Textos únicos:** 26. A rotação de criativos é alta.
- **Google:** 0 anúncios.

#### Recorrência

- 1 softgel por dia. Recarga a cada 30 dias, o que sugere frasco de 30 dias (inferência).
- **Assinatura:** `verificada`.

#### Criativos

- persona de cirurgião de transplante hepático com imagem de ultrassom;
- "No es un ayuno de 72 horas ❌… Es UNA cápsula con el desayuno";
- "¿Cuántas veces te han dicho que dejes el arroz?";
- vídeo UGC tipo talking head.

#### Classificação

- **Evidência:** `sinais_de_atividade`.
- **Prioridade:** `prioridade_alta`, **emergente** (entrada recente forte em ES).
- **Confiança:** moderada.

### Oferta 5 — GLOV: Berberine Complex

- **Mercado:** EUA, em inglês.
- **Marca:** multiproduto (beleza e bem-estar), com contador de domínio ~13.000 e anunciante Google GLOV BEAUTY LLC (200 anúncios).
- **Página:** a URL do produto e `/pages/gbq1` retornaram **"Access Denied … not available in your region"** (21:13Z e 21:28Z). Preço, dose e assinatura **não verificados**.
- **O que os anúncios dizem:**
  - "6 (ou 7) clinically studied ingredients supporting healthy blood sugar, metabolic function, and craving control";
  - "Buy 2, Get 1 FREE. 60-Day Money-Back. 9,042+ women trust it";
  - "Absorption Is The Whole Game".
- **Histórico publicitário:**
  - frase exata "GLOV Berberine" ~2.800 (21:20Z);
  - amostra de 31 cards com destino ao produto ou quiz. Faixas de idade:
    - < 30 d: 6;
    - 30–59 d: 3;
    - 60–89 d: 2;
    - 90–179 d: 20.
  - Mais antigo: 13/07/2026, com 127 d.
  - Páginas: Glov Beauty 19, "Metabolism After 40" 6, "Dr Jennifer Miller" 3, "Her Wellness Daily" 2 e "Dr Sheryl Williams" 1.
  - O advertorial `herwellnessdaily.com/top-5-berberine-supplements-women-v1-fb` faz um ranking comparativo.
- **Criativos:**
  - infográfico "CRUSH CRAVINGS. FREE YOUR METABOLISM." com ícones de sintomas;
  - vídeo do produto na mão;
  - "You don't have 8 separate problems. You have one.";
  - foto "Don't buy berberine until you read this".
- **Classificação:**
  - Evidência: `sinais_de_atividade`.
  - Prioridade: **`prioridade_media`**. Caiu uma faixa porque a recorrência não pôde ser verificada na página.
  - Confiança: baixa.

### Oferta 6 — Sandhu's Nutrition: Sangluco Berberine Complex

- **Mercado:** EUA, com anúncios em inglês e espanhol. A venda é na **Amazon**: https://www.amazon.com/dp/B0FXNQY3H3 (21:27Z).
- **Funil:** as pontes `gosandhus.com/blood-N` têm só o botão "BUY NOW ON AMAZON". Há também links via `ampd.to`.
- **Fórmula:** berberina HCl, canela-do-ceilão, cromo, melão-de-são-caetano, cúrcuma e vinagre de maçã.
- **Dose e duração:** 60 cápsulas, 2 por dia (anúncio) = **30 dias** (cálculo).
- **Amazon:**
  - $29.99 (List $31.99);
  - Subscribe & Save com entrega a cada 1–6 meses (`verificada`) e cupom de 20%;
  - **"3K+ bought in past month"**, indicador público do marketplace, não auditado.
- **Histórico publicitário:**
  - frase exata "Sangluco" ~49 (21:08Z);
  - 30 cards. Faixas de idade:
    - < 30 d: 21;
    - 60–89 d: 8;
    - 180+ d: 1.
  - Mais antigo: 20/05/2026, com 181 d.
  - Páginas: "Blood sugar balance community" 18, Sandhu Products Inc 11 e "Salud desde Adentro" (ES) 1.
  - A busca exata por "gosandhus.com" retornou 0 cards. O Google retornou 0 para o domínio.
- **Ganchos:**
  - "For people priced out of GLP-1 drugs…";
  - "nature's Ozempic";
  - "Under $1 a day";
  - ES: "Té detox. Metformina. Canela en polvo. Pastillas de cromo sueltas. Nada funcionó".
- **Classificação:**
  - Evidência: `evidencia_de_tracao` (anúncios + indicador Amazon + S&S).
  - Prioridade: `prioridade_media` (faixa 20–99).
  - Confiança: moderada.
  - Regulatório: comparação com Ozempic e GLP-1; interação da berberina com medicamentos.

### Oferta 7 — JSHealth Vitamins: Berberine+ Formula

- **Mercado e origem:** marca australiana ("Australian Made") com loja nos EUA. Na leitura, a URL dos EUA redirecionou para `jshealthvitamins.com/products/berberine-formula` (21:27Z).
- **Preço:**
  - 1 Month Supply: $47.50;
  - 2 Month: $89.99;
  - assinatura mensal: $39.94;
  - trimestral: $112.78 (Black Friday).
- **Dose:** "twice-daily capsule".
- **Assinatura:** `verificada`.
- **Histórico publicitário:**
  - "JSHealth Berberine" ~63 (21:23Z);
  - 29 cards (40 anúncios), 14 com 30+ d;
  - mais antigo: 05/08/2026, com 104 d.
  - Quase tudo é **anúncio de parceria com criadoras** (branded content), por exemplo "Ariana Wellness Pharmacist com JSHealth Vitamins".
- **Classificação:**
  - Evidência: `sinais_de_atividade`.
  - Prioridade: `prioridade_media`.
  - Confiança: moderada.
  - "63.000+ reviews" e "10 Million Bottles Sold" são alegações da marca.

### Oferta 8 — Herbaly: Glucose Functional Tea

- **Mercado:** EUA, em inglês.
- **Página:** https://herbaly.com/pages/glucose-tea-a (21:14Z)
- **Produto:** "12 research-backed herbs"; 28 sachês pirâmide de 2,5 g.
- **Dose:** 2 xícaras por dia, 15 min antes das refeições grandes.
- **Duração calculada:** 28 ÷ 2 = **14 dias** por pacote.
- **Kits:**
  - 1+1: 56 doses, 28 d;
  - 2+2: 112 doses, 56 d;
  - 3+3: 168 doses, 84 d, por $96 (de $192).
  - Pacote avulso: $24.00.
- **Assinatura:** "Subscribe & Save" `verificada`. Garantia de 30 dias. A página recomenda 3–6 meses de uso.
- **Histórico publicitário:**
  - "herbaly.com" ~220 e "Glucose tea" ~19;
  - 23 cards da oferta, **todos com 30+ d** (90–179 d: 15; 180+ d: 4);
  - mais antigo: 19/05/2026, com 182 d.
  - Google: 38 anúncios (Herbaly Marketplace Inc.).
- **Criativos:**
  - "People say Herbaly Glucose Tea is expensive. They're right.";
  - "Let's say the thing you're already thinking. It's just tea.";
  - estático de chá gelado "The easiest habit for healthy blood sugar";
  - vídeo talking head com potes de chá.
- **Classificação:**
  - Evidência: `sinais_de_atividade`.
  - Prioridade: `prioridade_media`.
  - Categoria **limítrofe** (chá funcional): confirmar enquadramento como suplemento.

### Oferta 9 — Dr. Eve: Sugar Cutting Tea ("Bangpae Tea", Coreia)

- **Página-ponte:** https://www.dreveus.com/pages/amazon-sugar-cutting, que leva à Amazon (21:28Z).
- **Preço:** $29.99 → $19.99.
- **Origem:** "Made in Korea".
- **Ingredientes (anúncio):** tupinambo, melão-de-são-caetano, banaba e pétala de hortênsia.
- **Não observados:** dose, unidades e assinatura.
- **Histórico publicitário:**
  - "dreveus.com" ~22 (21:03Z);
  - 29 cards (30 anúncios), 27 com 30+ d (60–89 d);
  - mais antigo: 16/09/2026, com 62 d.
  - A busca "Sugar Cutting" (~190) mistura outras marcas.
- **Criativos:**
  - **ilustrações e animação estilo cartoon**, com personagens bebendo chá;
  - vídeo de xícara;
  - "You eat lunch. An hour later, crashed, foggy, craving something sweet. That's your blood sugar.";
  - "Korea's #1 blood sugar tea".
- **Classificação:**
  - Evidência: `sinais_de_atividade`.
  - Prioridade: `prioridade_media`.
  - Confiança: baixa.

### Oferta 10 — True Nutra: 7-in-1 Blood Sugar Complex (gotas)

- **Página:** https://truenutra.com/products/fb-en-bsc003 (21:27Z)
- **Produto:** 15 mL = 15 doses de 1 mL por dia (**15 dias**). O kit sugere "twice a day".
- **Preço:** Buy One $28.95; Buy 2 Get 2 $38.95. A exibição é ambígua.
- **Assinatura:** "Subscribe, Save 59%" `verificada`. Garantia de 90 dias.
- **Alegação:** "helps lower A1C".
- **Histórico publicitário:**
  - domínio ~1.900 (21:18Z), mas a maior parte é o "6-in-1 Lymphatic Complex";
  - **8 cards** do Blood Sugar Complex na amostra, 2 com 30+ d;
  - mais antigo: 07/10/2026, com 41 d.
  - Google: 300 anúncios (R5 Brands LLC).
- **Por que está na lista:** é a **versão em inglês da copy da Glucora** ("Your blood sugar will be balanced, your cravings gone — and you'll feel absolutely amazing"). É um sinal de transferência ES → EN do mesmo formato.
- **Classificação:**
  - Evidência: `sinais_de_atividade`.
  - Prioridade: `em_observacao`, **emergente: sim**.
  - Confiança: baixa.

---

## Descoberta de padrões

1. **Mecanismos que se repetem entre marcas:**
   - "Ceilão 12:1 + MCT = absorção": Metabolae, Resia, Liraé e PureCeylon, além de Gentilia, Liréa e Kenzendo nas referências.
   - "Berberina = GLP-1/Ozempic natural": Sangluco, Ovia, JSHealth, Kind Patches, Bioma, Absorb.
   - "Absorção líquida/sublingual > cápsula": Glucora, True Nutra, Ovia ("only 1% absorbs" em cápsula) e GLOV ("Absorption Is The Whole Game").
   - "Cássia barata faz mal ao fígado": toda a família Ceilão.
2. **Ofertas que compartilham roteiros ou estruturas de página:**
   - Texto idêntico "X was created for people who've tried everything to manage their blood sugar…" em Metabolae, Resia e Liraé.
   - "Most cinnamon supplements use fake Cassia bark…" em Metabolae e Liraé.
   - "Please don't buy…" em Metabolae e Resia.
   - Nome de produto idêntico, "Ceylon Cinnamon 7200mg Equivalent with MCT Oil", em Metabolae, Resia e Liraé.
   - Glucora (ES), True Nutra (EN) e esencialluz.es usam a mesma copy.
   - PureCeylon e Nervora usam o mesmo template de página de venda.
   - Páginas chamadas "Blood Sugar Balance Community" anunciam Metabolae e "Blood sugar balance community" anuncia Sangluco. A relação entre elas não foi verificada.
3. **Marcas com animações, desenhos ou explicações visuais:**
   - Liraé: animação 3D de vaso sanguíneo.
   - Dr. Eve: personagens ilustrados em estilo cartoon.
   - GLOV: infográfico de sintomas.
   - Glucora: infográfico de glicosímetro antes/depois.
   - Resia: gráfico "A1C 5.9".
   - Kenzendo (referência): "viagem da cápsula" em 3D.
   - Os demais usam sobretudo texto longo + foto, UGC e talking head.
4. **Concentração de anunciantes:**
   - Mais **anunciantes distintos**: berberina / GLP-1 natural.
   - Mais **volume e longevidade por oferta**: Ceilão 12:1 + MCT, puxado por Metabolae, Resia e Liraé.
   - Em espanhol, o mercado tem poucas marcas, mas Glucora é longeva e PureCeylon e Nervora estão crescendo.
5. **Ganchos recorrentes:**
   - recusa ou efeitos colaterais da metformina;
   - números de A1C e glicemia de jejum;
   - personas de enfermeira (RN), médico ou cirurgião;
   - "Please don't buy";
   - ancoragem de preço por kit;
   - garantia que reembolsa embalagens vazias;
   - "food noise" e desejo por açúcar;
   - mulheres 40+ e perimenopausa.
6. **Diferenciação comercial relevante:**
   - **Formato líquido sublingual** (Glucora / True Nutra) num mercado dominado por softgels.
   - **Chá funcional** como hábito diário (Herbaly, Dr. Eve), com consumo rápido (14 d por pacote).
   - **Venda via Amazon com pontes** (Sangluco, Dr. Eve), que tira proveito de prova social e assinatura do marketplace.
   - **Branded content com criadoras** (JSHealth).
   - **Segmento hispânico** com personas latinas (PureCeylon, Glucora).

---

## Fora de escopo (não suplementos ou outro problema)

| Marca — produto | Categoria | URL | Motivo |
|---|---|---|---|
| Kind Patches — Berberine Patch / Metabolic Trio | adesivo transdérmico | https://kindpatches.com/collections/bundles/products/metabolic-trio-bundle-1 | não ingerível; ~780 anúncios no domínio |
| PiPi Tea — oolong | chá / colesterol | https://shop.pipitea.com/ppch/sp-nm | problema principal é colesterol; alguns anúncios usam história de glicemia |
| Signos, Dexcom, Stelo, Eversense, Omnipod, apps de glicemia | dispositivos, medicamentos, apps | — | não são suplementos |
| Equine Veterinary Essentials — Metabo-Balance | suplemento equino | https://evesupplements.com | animal |
| GOOD IDEA — água com aminoácidos | bebida | https://www.goodidea.us/ | bebida; ~6 anúncios |
| Omvyra Labs / Aurivita | DE em diabéticos | https://omvyralabs.co/pages/adv-13-diabetic-ed | outro problema (diabetes só como gancho) |

## Candidatos não selecionados e por quê

- **Ovia Essentials — Cutting Drink Mix** (berberina líquida, cromo, 5-HTP; mulheres na perimenopausa):
  - Na amostra: 44 cards e 142 anúncios, 38 com 30+ d, mais antigo de 182 d. O contador "Ovia" deu ~1.800.
  - Mas o CTA do listicle leva a `oviaessentials.com/products/cutting-drink-mix`, que exibiu **"Sorry, this site is no longer available."** (21:27Z). Sem página de venda verificável.
  - É o 1º suplente se a página voltar.
- **Santo Remedio — Berberine+ (GlucoVantage, di-hidroberberina; ES):** marca com ~130 anúncios e 300 no Google, mas só 2 cards do Berberine+ na amostra. Assinatura de 10% verificada; 2 cápsulas por dia.
- **Nervora — Ácido R-Alfa Lipoico 600 mg (ES):** subnicho adjacente (neuropatia diabética). ~550 anúncios, mais antigo de 48 d, mesmo template da PureCeylon.
- **Gratitude Health — di-hidroberberina:** ~10 anúncios, todos < 30 d. Emergente; usa demonstração com monitor de glicose ("I tested a Big Mac on my glucose monitor").
- **CleverPro — Carbivore:** ~20 anúncios, 19 com < 30 d. Bloqueador de carboidrato pós-refeição.
- **Daily Curb — bebida para SOP/PMOS:** ~25 anúncios, todos < 30 d.
- **Black Girl Vitamins — PCOS Relief Gummies:** marca multiproduto (~780); poucos cards específicos.
- **UMZU Sensolin** (~2 anúncios) e **Glucocil** (1 anúncio): volume insignificante.
- **Nuora** (`mynuora.com`, ~1.800): os anúncios com berberina levam ao "Gut capsule" e às gomas femininas, já registrados na missão 001.
- **Serelia (ES):** cortisol + mio-inositol (~1.500). Problema principal é cortisol/estresse.
- **Afiliados clássicos** (Sugar Defender, GlucoTrust, Glucoberry): praticamente ausentes na Meta EUA. Só 1 link `hop.clickbank.net` (GlucoTonic) com página "Raelbecshopville".

## Recomendações de aprofundamento

1. **Repetir as contagens da Meta** quando o limite de taxa expirar (sessão nova ou outro horário), com rolagem completa para Resia, Liraé, Glucora, PureCeylon, GLOV e Sangluco. Objetivos: confirmar o `active_ads_offer` real e o anúncio ativo mais antigo.
2. **Mapear a cadeia white-label do Ceilão 12:1 + MCT:** fornecedor, operadores (OneStopMrkt LLC, Tanvin Joy, BAT Partners LLC) e, se possível, rótulos e Supplement Facts.
3. **Glucora → True Nutra:** acompanhar se a versão em inglês ganha volume nas próximas semanas (emergente).
4. **Acessar a GLOV** por outra rota, como Amazon ou cache público, para obter preço, dose e unidades.
5. **TikTok Creative Center / TikTok Shop:** verificar berberina e canela no TikTok EUA. Não foi coberto nesta missão.
6. **Revisão regulatória obrigatória** antes de adaptar qualquer copy:
   - remissão de diabetes;
   - redução de A1C;
   - uso com metformina ou GLP-1;
   - "Ozempic natural";
   - personas de profissionais de saúde.

## Limitações de acesso e de confiabilidade

- **Meta Ad Library:** paginação bloqueada por limite de taxa (`Rate limit exceeded`, código 1675004) em todas as tentativas, de 20:5x a 21:23Z. Os números de volume são o contador aproximado da Meta. Distribuição por idade e "mais antigo" referem-se à amostra da 1ª página, ordenada por impressões, que tende a favorecer anúncios antigos e de alto alcance. **Não houve extrapolação.**
- **Histórico truncado:** fora da UE, anúncios comerciais inativos não são exibidos. A "primeira veiculação" da oferta é desconhecida.
- **Contagem de variações:** cards marcados como "Esse anúncio tem várias versões" contam como 1 anúncio. Só "N anúncios usam esse criativo" foi somado.
- **Páginas inacessíveis:** GLOV ("Access Denied" para a região) e Ovia ("site no longer available").
- **Valores ambíguos:** alguns preços de kits (Glucora 1+1, True Nutra) foram lidos de forma ambígua e estão registrados assim.
- **Alegações não auditadas:** avaliações, "vendido X vezes", "3K+ bought in past month" e depoimentos são alegações ou indicadores públicos não auditados.
- **Fontes não usadas:** TikTok, transcrição de áudio e análise quadro a quadro de vídeos. As observações visuais vêm de capturas da 1ª tela da Ad Library, guardadas em `evidence-local/glicemia-eua-2026-11-17/` (não versionado).
