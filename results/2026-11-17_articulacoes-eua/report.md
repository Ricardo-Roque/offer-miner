# Relatório da missão: suplementos para saúde articular, rigidez e mobilidade — EUA

## Escopo e execução

- **Data de execução (UTC):** 2026-11-17, aproximadamente das 18:40 às 19:30. As contagens por domínio foram feitas entre 19:01 e 19:14 UTC.
- **Missão de origem:** primeira mineração autônoma. Até 10 ofertas internacionais de suplementos para saúde articular, rigidez e mobilidade, com foco nos EUA e mecanismos em descoberta livre.
- **Mercado de venda:** Estados Unidos (filtro `country=US` na Meta Ad Library; `region=US` no Google Ads Transparency).
- **Problema:** dor e rigidez articular, joelho, quadril, artrite e mobilidade.
- **Mecanismos:** descoberta livre. Foram observados ácido hialurônico, cúrcuma + boswellia, mexilhão-de-lábios-verdes, cereja ácida (tart cherry), extrato herbal líquido, silício + colágeno + K2 e colágeno "3D" + cúrcuma.
- **Idiomas pesquisados:** inglês, além de espanhol para o público hispânico dos EUA.
- **Ferramentas realmente usadas:**
  - Navegador embutido do Orca, sem login, para Meta Ad Library, Google Ads Transparency, páginas de venda e Amazon.
  - Script local para ler os cards da Ad Library: ID, data de início, página, nº de anúncios que usam o criativo e link de destino.
  - Capturas de tela, guardadas em `evidence-local/`, fora do Git.
  - Não foram usados WebSearch, TikTok Creative Center, transcrição de áudio nem download de vídeos.
- **Limites de pesquisa:**
  - 21 buscas de descoberta por palavra-chave na Ad Library, até 7 cargas de rolagem cada.
  - 18 buscas por frase exata (domínio ou marca), até 16 cargas cada.
  - 12 consultas ao Google Ads Transparency.
  - Cerca de 20 páginas de venda ou advertoriais lidas.
- **Parâmetros de priorização:** padrão de `docs/prioritization-criteria.md`.
  - Idade mínima relevante: 30 dias.
  - Faixas: alta ≥ 100, média 20–99 e observação < 20 anúncios ativos da oferta.
  - Categoria: suplementos consumíveis para humanos.
- **Convenção de contagem:**
  - `anúncios ativos da oferta` soma os anúncios ativos, incluindo variações ("N anúncios usam esse criativo e esse texto"), deduplicados pelo ID da biblioteca.
  - `cards` são as entradas distintas exibidas pela Ad Library.
  - As faixas de idade contam cards.
  - Idade = 2026-11-17 menos a data "Veiculação iniciada em".
- **Motivo do encerramento:** 10 ofertas distintas documentadas com histórico publicitário, página de venda e dados de recorrência. As três últimas buscas de descoberta trouxeram poucos candidatos novos e relevantes.

## Resumo executivo

- **Candidatos encontrados (suplementos para humanos):** 16. Ficaram 10 no relatório principal; 6 foram registrados sem ficha (ver "Candidatos não selecionados").
- **Ofertas com evidência mínima:** 10.
- **Por prioridade:** alta 9 · média 1 · em observação 0 no top 10. Fora do top 10: 1 em observação, possivelmente emergente (OsteoShield).
- **Padrões comerciais observados:**
  1. **Template de copy compartilhado:** "You've tried X… But you've probably never felt it actually do anything. That's because most supplements cut corners…" aparece em Arthrogenix, VitalHydra, BioRoot Labs, Ilyra e GoodGrove. Hipótese, não verificada: mesma agência ou mesmo operador.
  2. **Redes de páginas-persona e "comunidades":** "Dr. … MD", "Rheumatologist", "Joint Health Club", "Living with joint pain – Community". Elas veiculam histórias longas em primeira pessoa e levam ao mesmo produto. É o caso de Nova (11 páginas), BioRoot (19), GoodGrove (5), VitalHydra (7) e Ilyra (5).
  3. **Cereja ácida (tart cherry) como categoria em alta para articulação e gota:** pelo menos 3 marcas ativas (GoodGrove, Ilyra, Nature Heart), com anúncios comparativos entre elas.
  4. **Estrutura de oferta padrão:** 1 / "Buy 2 Get 1" / "Buy 3 Get 2", assinatura com 15–52% de desconto e garantia de 60–365 dias.
  5. **Ângulo menopausa + dor no quadril** (Nova "Her Again", Halsten): segmento feminino 45+ explorado como subnicho.
- **Lacunas:**
  - Rolagem parcial em 3 ofertas.
  - Dose ou unidades não observadas em 4 ofertas.
  - Nenhum dado de TikTok.
  - Histórico de anúncios inativos indisponível fora da UE.

> Prioridade ordena a investigação. Quantidade e idade de anúncios **não** indicam vendas, investimento ou lucro.

## Ranking de prioridade

| # | Oferta (marca — produto) | País / idioma | Prioridade | Anúncios ativos da oferta (cards) | Ativos da marca/domínio | Anúncio ativo mais antigo (dias) | Histórico desde | Tipo / recompra | Assinatura | Evidência | Fonte e data da contagem |
|---|---|---|---|---|---|---|---|---|---|---|---|
| 1 | Arthrogenix — fórmula articular "14-in-1" | EUA / EN | prioridade_alta | 496 (236) | 500 | 354 | 2025-11-28 | consumivel_recorrente · 60 cáps. = 30 d | alegada | sinais_de_atividade | Meta, frase exata "arthrogenix.org", 2026-11-17T19:06Z, rolagem completa (~260 exibidos) |
| 2 | VitalHydra — ácido hialurônico em cápsulas | EUA / EN | prioridade_alta | 288 (266) | 288 | 277 | 2026-02-13 | consumivel_recorrente · "30 day supply" | verificada | sinais_de_atividade | Meta "vitalhydra.co", 19:07Z, 266 de ~320 |
| 3 | The Nova Bottle — Curcumin + Boswellia | EUA / EN | prioridade_alta | 348 (306) | 559 | 271 | 2026-02-19 | consumivel_recorrente · 60 cáps. = 30 d | verificada | evidencia_de_tracao | Meta "hernovabottle.com" + "thenovabottle.com", 19:01Z; Google 28 + 18 |
| 4 | Haka Life — GLX3 mexilhão-de-lábios-verdes | EUA / EN | prioridade_alta | 243 (229) | 243 | 263 | 2026-02-27 | consumivel_recorrente · 60 softgels = 30 d | verificada | evidencia_de_tracao | Meta "hakalife.com", 19:02Z, completa; Google 27 |
| 5 | Ilyra — Tart Cherry Extract | EUA / EN | prioridade_alta | ≥284 (223) — amostra | ≥295 | ≥98 | 2026-08-11 | consumivel_recorrente · dose n/obs. | alegada | sinais_de_atividade | Meta "tryilyra.com", 19:10Z, 230 de ~1.400 |
| 6 | BioRoot Labs — Turmeric Curcumin 1.000 mg | EUA / EN | prioridade_alta | ≥291 (226) — amostra | ≥312 | ≥108 | 2026-08-01 | consumivel_recorrente · 3 cáps./dia, "1 month" | alegada | evidencia_de_tracao | Meta "biorootlabs.com", 19:09Z, 247 de ~1.300; Google 74 |
| 7 | GoodGrove — Tart Cherry Extract | EUA / EN | prioridade_alta | ≥245 (229) — amostra | ≥295 | ≥55 | 2026-09-23 | consumivel_recorrente · dose n/obs. | verificada | evidencia_de_tracao | Meta "trygoodgrove.com", 19:04Z, 277 de ~1.700; Google 73 |
| 8 | Plants Basically — Juicy Joint Extract | EUA / EN | prioridade_alta | 156 (149) | 156 | 224 | 2026-04-07 | consumivel_recorrente · 60 porções 1 mL | verificada | evidencia_de_tracao | Meta "plantsbasically.com", 19:03Z, completa; Google 43 |
| 9 | Regensil — Joint Repair | EUA / EN | prioridade_alta | 131 (91) | 131 | 169 | 2026-06-01 | consumivel_recorrente · 2 cáps./dia, "1 Month" | alegada | sinais_de_atividade | Meta "regensil.com", 19:06Z, completa; Google 2 |
| 10 | Collanol — colágeno "3D" + cúrcuma | EUA / EN + ES | prioridade_media | 54 (54) | 54 | 300 | 2026-01-21 | consumivel_recorrente · 20 cáps. = 20 d | verificada (Amazon) | evidencia_de_tracao | Meta "collanol.com", 19:08Z, completa; Google 2; Amazon |

Em todos os casos, "histórico desde" é a data do anúncio **ativo** mais antigo. Os anúncios inativos não são exibidos para os EUA, então o histórico pode estar truncado. As listas completas de IDs (data, página, destino e URL da biblioteca) estão em `data/ads_<oferta>.csv`, e as estatísticas em `data/agg_<oferta>.json`.

### Distribuição dos cards ativos por idade (2026-11-17)

| # | Oferta | <30 | 30–59 | 60–89 | 90–179 | 180+ | Textos distintos* | Páginas anunciantes |
|---|---|---|---|---|---|---|---|---|
| 1 | Arthrogenix | 97 | 63 | 30 | 44 | 2 | 14 | 3 |
| 2 | VitalHydra | 47 | 57 | 19 | 94 | 49 | 78 | 7 |
| 3 | Nova Curcumin + Boswellia | 225 | 78 | 1 | 0 | 2 | 27 | 11 |
| 4 | Haka GLX3 | 172 | 28 | 8 | 14 | 7 | 8 | 2 |
| 5 | Ilyra (amostra) | 66 | 86 | 62 | 9 | 0 | 18 | 5 |
| 6 | BioRoot cúrcuma (amostra) | 99 | 76 | 41 | 10 | 0 | 20 | 19 |
| 7 | GoodGrove (amostra) | 145 | 84 | 0 | 0 | 0 | 43 | 5 |
| 8 | Plants Basically | 95 | 11 | 2 | 30 | 11 | 21 | 5 |
| 9 | Regensil | 59 | 7 | 2 | 23 | 0 | 5 | 1 |
| 10 | Collanol | 8 | 7 | 0 | 22 | 17 | 54 | 1 |

\* "Textos distintos" usa os primeiros 120 caracteres do texto como proxy de criativos únicos. Não distingue mídias diferentes com o mesmo texto e por isso **não** equivale a `unique_creatives`, que fica `null` no JSON.

## Consultas realizadas

| Idioma | Mercado | Busca | Fonte | Resultado/resumo |
|---|---|---|---|---|
| EN | US | joint supplement | Meta Ad Library (palavra-chave, ativos) | ~15.000; muitos pets; Plants Basically, BioRoot, Elavate |
| EN | US | joint pain | Meta | ~50.000; maioria joelheiras/dispositivos; Plants Basically |
| EN | US | knee pain | Meta | ~50.000; dispositivos; poucos suplementos |
| EN | US | stiff joints | Meta | ~23.000; Ilyra, GroundingWell (não suplemento), pets |
| EN | US | joint relief | Meta | ~32.000; Plants Basically, Pipitea, True Sea Moss |
| EN | US | cartilage | Meta | ~24.000; Regensil, AlgaeCal, Freedom Joint Drops, pets |
| EN | US | joint support | Meta | ~50.000; Nova (páginas-comunidade), Black Girl Vitamins |
| EN | US | glucosamine | Meta | ~16.000; Haka Life, pets |
| EN | US | turmeric joint | Meta | ~13.000; Collanol, BioRoot, Haka, Arthrogenix, GoodGrove |
| EN | US | achy joints | Meta | ~3.000; Elavate, Mara Labs, Youtheory, NativePath |
| EN | US | arthritis supplement | Meta | ~4.700; GoodGrove, Halsten, Nova, Noralife |
| ES | US | dolor de rodillas | Meta | ~7.200; muitos anunciantes mexicanos (fronteira); Sandhus |
| EN | US | joint pain supplement | Meta | ~9.100; Haka, Elavate, Nova, VitalHydra, Arthrogenix |
| EN | US | knee cartilage | Meta | ~13.000; GoodGrove, Regensil, Morning Vitality |
| EN | US | inflammation joints | Meta | ~21.000; Haka, GoodGrove |
| EN | US | collagen joints | Meta | ~19.000; True Sea Moss, Elavate, Black Girl Vitamins |
| EN | US | hip pain | Meta | ~27.000; Halsten, Nova, Bronoir (calçado) |
| ES | US | dolor articular | Meta | ~800; Collanol (ES), Sandhus |
| EN | US | bone on bone | Meta | ~50.000; ruído (fármacos, alimentos) |
| EN | US | hyaluronic acid joints | Meta | ~6.000; Elavate, VitalHydra, Arthrogenix |
| EN | US | morning stiffness | Meta | ~24.000; ruído (travesseiros, dispositivos) |
| — | US | "hernovabottle.com", "thenovabottle.com", "hakalife.com", "plantsbasically.com", "trygoodgrove.com", "trynoralife.com", "tryhalsten.com", "regensil.com", "arthrogenix.org", "vitalhydra.co", "morningvitality.com", "collanol.com", "biorootlabs.com", "mara-labs.com", "tryilyra.com", "gosandhus.com", "OsteoShield", "Sandhus" | Meta (frase exata, ativos) | contagens por oferta (acima e em `data/`) |
| — | US | 12 domínios | Google Ads Transparency (`region=US&domain=`) | contagens e anunciantes verificados nas fichas |

A busca por palavra-chave tem muito ruído: joelheiras, fármacos e suplementos para cães. Por isso, a seleção usou o destino dos anúncios para chegar ao domínio e, em seguida, a busca por frase exata desse domínio.

## Ofertas investigadas

### Oferta 1 — Arthrogenix

- **Mercado de venda confirmado:** EUA (frete grátis "on all US orders"; anúncios na Ad Library US).
- **Origem da marca:** não identificada. Não há anunciante no Google.
- **Categoria/problema:** articulação (rigidez, dor, inchaço, flexibilidade).
- **Mecanismo alegado no marketing:** "14-in-1"; ácido hialurônico "em uma pílula"; "3 causas": inflamação, dano à cartilagem e perda de fluido articular.
- **Página oficial:** https://arthrogenix.org/ — observada em 2026-11-17.
- **Preço e oferta:** 1 frasco US$ 49,95; 3 por US$ 99,95; 6 por US$ 149,95 ("Regular Price" riscado de US$ 99,95, 299,85 e 599,77). Frete grátis acima de US$ 49,95.

#### Histórico publicitário

- **Consulta:** Meta Ad Library, frase exata "arthrogenix.org", US, ativos — 2026-11-17T19:06:31Z.
- **Método:** rolagem até o fim (238 cards carregados de ~260 exibidos). `count_is_estimate`: sim.
- **Primeira data observada:** 2025-11-28. **Histórico possivelmente truncado:** sim.
- **Anúncio ativo mais antigo:** ID 1900180230587521, iniciado em 2025-11-28, com 354 dias.
- **Anúncios ativos da oferta:** 496 (236 cards); 139 cards com 30+ dias.
- **Anúncios ativos do domínio:** 500. **Contador exibido:** ~260 (estimativa).
- **Páginas anunciantes:** Arthrogenix (213 cards), Samantha Newhouse (12) e All American Pharma (11).
- **Google Ads Transparency:** 0 anúncios para arthrogenix.org (US, 2026-11-17T19:12Z).

#### Recorrência

- **Tipo:** consumivel_recorrente.
- **Dose e embalagem:** 2 cápsulas/dia; 60 cápsulas por frasco (FAQ). Duração calculada: 30 dias. Os kits correspondem a 90 e 180 dias.
- **Assinatura:** alegada. Há um item de menu "Subscribe And Save", mas a opção não foi vista no seletor de compra.
- **Potencial de recompra (inferência):** alto, por ser frasco de 30 dias com kits de até 6 meses.

#### Criativos e evidências

- **Hook dominante (210 cards):** "You've tried glucosamine. Turmeric. Fish oil. Collagen. And you've probably never felt any of them actually do anything. Here's why." Exemplo: 1902255797122321 (iniciado em 16/07/2026).
- **Formato observado em captura:** vídeo vertical com personagem animado de ingrediente (flor de papoula-da-califórnia). Exemplos: 1061062640190123 e 1054541170729821.
- **Estático "Black Friday — Pain Relief Blitz — 40% OFF"** pela página "All American Pharma": 878369528084990 (29/11/2025).
- **Advertorial/ranking em vídeo (1:51)** pela persona "Samantha Newhouse": 1740737730542243.

#### Classificação

- **Evidência:** sinais_de_atividade.
- **Prioridade:** prioridade_alta. Justificativa: 496 anúncios ativos (≥100), 139 cards com 30+ dias, e o produto é consumível de 30 dias. Meta US, 2026-11-17.
- **Confiança:** alta para a contagem; só há canal Meta.
- **Regulatório:**
  - "Guaranteed Fast Acting Relief", "5x faster", "no side effects" e um suposto endosso de "non-profit health organization" não identificada exigem revisão jurídica e científica.
  - As identidades das personas não foram verificadas.
- **Dados faltantes:** rótulo completo, empresa responsável e preço com assinatura.

### Oferta 2 — VitalHydra

- **Mercado de venda confirmado:** EUA (entrega expressa grátis com data nos EUA; Ad Library US).
- **Categoria/problema:** dor e rigidez no joelho e nas articulações; também lombar em depoimentos.
- **Mecanismo alegado:** ácido hialurônico em cápsula, "the joint molecule". Compara-se à injeção de HA no joelho, que custaria "US$ 350–500 por dose", e anuncia custo de "about US$ 1,13/day".
- **Página oficial:** https://vitalhydra.co/pages/vitalhydraha — 2026-11-17. Funil alternativo com quiz: try.vitalhydra.co/quiz-v2.
- **Preço:** 1 frasco ("30 day supply") US$ 31,96 (de US$ 39,95); "Buy 2, Get 1 Free" (90 dias) US$ 63,92; "Buy 3, Get 2 Free" (150 dias) US$ 95,88.

#### Histórico publicitário

- **Consulta:** Meta, frase exata "vitalhydra.co", 2026-11-17T19:07:30Z.
- **Método:** amostra de 266 cards de ~320 exibidos. Estimativa: sim.
- **Anúncio ativo mais antigo:** 1851132645542207, iniciado em 2026-02-13, com 277 dias. Histórico possivelmente truncado.
- **Anúncios ativos da oferta e do domínio:** 288 (266 cards).
- **Longevidade:** 219 cards com 30+ dias e 49 com 180+, a carteira de criativos antigos mais longeva do conjunto.
- **Páginas:** VitalHydra (112), Vital Hydra (109), Linda Campbell (24), "Dr. Rebecca Holloway PhD – Joint & Mobility Specialist" (15), The Healthy Joint Times (3), Rebecca Holloway (2) e "Dr. James Carter MD" (1).
- **Google Ads Transparency:** 0 anúncios (2026-11-17T19:12Z).

#### Recorrência

- **Dose:** 2 cápsulas/dia (página).
- **Unidades por frasco:** não informadas; a página diz "30 day supply". Duração (alegada): 30, 90 e 150 dias nos kits.
- **Assinatura:** verificada ("Save 52% with Automatic Refills — Zero commitment, Cancel Anytime").
- **Alegação da marca:** "16,000+ customers · 5,500+ active subscribers" (não auditada).
- **Potencial de recompra (inferência):** alto.

#### Criativos

- "You've heard hyaluronic acid helps your joints. But you've probably never felt it actually do anything." (46 cards): 958607710484903 (24/04/2026).
- Persona-depoimento "I almost didn't write this… I thought this joint pain brand was another online scam" (Linda Campbell): 1289552846577942 (15/05/2026).
- Persona-especialista "I spent three weeks investigating every joint pain solution…" (Dr. Rebecca Holloway): 1250869726857775.
- Educativo "Before you accept that your knees are simply 'getting old'…": 1985180078865672.

#### Classificação

- **Evidência:** sinais_de_atividade.
- **Prioridade:** prioridade_alta. Justificativa: 288 anúncios, 219 cards com 30+ dias e assinatura verificada.
- **Confiança:** alta.
- **Regulatório:** a equivalência com a injeção intra-articular é uma alegação terapêutica, e as personas com título "Dr."/"PhD" não foram verificadas.
- **Faltante:** cápsulas por frasco, mg de HA e empresa responsável.

### Oferta 3 — The Nova Bottle — Curcumin + Boswellia Joint Support

- **Mercado de venda:** EUA ("Ships from US"). O anunciante verificado no Google é "beyond row 15 pty ltd", que pelo sufixo aparenta ser empresa australiana. Mercado de venda ≠ origem.
- **Mecanismo alegado:** "duas vias inflamatórias"; 95% curcumina + boswellia + extrato de pimenta-preta + vitamina C ("4-in-1").
- **Página:** https://www.hernovabottle.com/products/curcumin-boswellia. Ela redireciona para try.thenovabottle.com (relação **observada**) — 2026-11-17.
- **Preço:** 1 frasco US$ 34,00 (ref. US$ 42,50); Buy 2 Get 1 US$ 68,00; Buy 3 Get 2 US$ 102,00; ebook brinde.

#### Histórico publicitário

- **Consulta:** Meta, frase exata "hernovabottle.com" (19:01:15Z) + "thenovabottle.com" (19:01:45Z), US, ativos.
- **Método:** rolagem completa (158/~160 e 285/~340), mais 11 IDs das buscas temáticas. Deduplicado por ID.
- **Filtro do produto:** destinos `curcumin-boswellia` e `nova-sale-page`. Foram excluídos `menopaused` e `her-again`.
- **Anúncios ativos da oferta:** 348 (306 cards); 81 com 30+ dias.
- **Anúncio ativo mais antigo:** 1982637528984426, iniciado em 2026-02-19, com 271 dias.
- **Ativos da marca (dois domínios):** 559, dos quais 199 são do produto de menopausa "Menopaused/Her Again" (contado à parte).
- **Páginas (11):** The Nova Bottle (63), Life with Arthritis Community page (63), Move Pain Free Daily (63), Thriving In Menopause (46), Living with joint pain – Community (21), "Sydney Sylvaine, Rheumatologist" (19), Everyday Joint Health (18) e outras.
- **Google Ads Transparency:** 28 anúncios (hernovabottle.com) + 18 (thenovabottle.com), anunciante "beyond row 15 pty ltd" (2026-11-17T19:12Z).

#### Recorrência

- 2 cápsulas pela manhã; 60 cápsulas = 30 dias (página). Os kits somam 90 e 150 dias (cálculo).
- **Assinatura:** verificada ("Save 20% With Automatic Refills", entrega mensal ou a cada 3 meses).
- **Potencial de recompra:** alto.

#### Criativos

- **Hook (146 cards):** "I spent years buying every arthritis supplement I could find because I was desperate to avoid taking ibuprofen every day. Collagen. Glucosamine. Fish oil. Turmeric…" — 4443599552521777.
- **Transformação:** "I reversed my gluteal tendinopathy in 4 weeks…" (29 cards) — 927956140251681.
- **Estático de produto "4-IN-1 Anti-inflammatory formula"** (captura); "The most powerful anti-inflammatory formula, a 4-in-1…" — 1654073289847769.
- **Provocativo:** "I don't give a f*ck if this upsets the medical community…" — 2114285166124636.
- **Formato:** predominam estáticos de produto com texto longo em primeira pessoa (capturas).

#### Classificação

- **Evidência:** evidencia_de_tracao (Meta com 11 páginas + Google com anunciante verificado).
- **Prioridade:** prioridade_alta (348 anúncios; 81 cards com 30+ dias).
- **Confiança:** alta.
- **Regulatório:** "No Joint Pain in 60 days or money back", "fix the inflammation at the source", reversão de tendinopatia, persona "Rheumatologist" não verificada e escassez ("sold out four times", "93% gone") não verificável.

### Oferta 4 — Haka Life Nutrition — GLX3 (óleo de mexilhão-de-lábios-verdes)

- **Mercado de venda:** EUA (telefone 800, frete nos EUA). Ingredientes da Nova Zelândia (página).
- **Mecanismo alegado:** óleo de mexilhão-de-lábios-verdes com ETA, "~30 ácidos graxos vs. 2–3 do óleo de peixe"; "só 3 ingredientes"; elegível a HSA/FSA.
- **Página:** https://www.hakalife.com/products/glx3-extra-strength-green-lipped-mussel-oil — 2026-11-17. LP principal dos anúncios: hakalife.com/pages/bogobigdeal.
- **Preço:** 30 porções US$ 54,99 (assinatura US$ 46,74); 60 porções US$ 103,53 (US$ 88,00); 90 porções US$ 139,98 (US$ 118,99).

#### Histórico publicitário

- **Consulta:** Meta, frase exata "hakalife.com", 2026-11-17T19:02:35Z.
- **Método:** completa (211 de ~210), mais 18 IDs das buscas temáticas.
- **Anúncios ativos da oferta:** 243 (229 cards); 57 com 30+ dias, 7 com 180+.
- **Anúncio ativo mais antigo:** 1525824885574625, iniciado em 2026-02-27, com 263 dias.
- **Ativos da marca:** 243. Os anúncios do produto para cães foram excluídos; nenhum apareceu no domínio.
- **Páginas:** Haka Life Nutrition (223) e Andrew Casey (6).
- **Google Ads Transparency:** 27 anúncios, anunciante verificado "Haka Life Nutrition".

#### Recorrência

- 2 softgels/dia (dose de ataque de 4/dia nas 2 primeiras semanas); 60 softgels por frasco. Duração calculada: 30 dias, ou ~22 dias no primeiro frasco com a dose de ataque.
- **Assinatura:** verificada (Subscribe & Save 15%, a cada 1, 2 ou 3 meses).
- **Alegação da marca:** "700,000+ bottles sold" / "150,000+ people" (não auditada).
- **Potencial de recompra:** alto.

#### Criativos

- **Hook (177 cards):** "GLX3 Green Lipped Mussel oil has helped over 150,000+ people with joint support since 2018" + bullets + garantia de 90 dias — 1385828753073784.
- **Estáticos "Buy One, Get One Free" e "GLX3 qualifies for HSA/FSA"** (capturas): 1080236311366419 e 1634656008315651.
- **Comparativo novo:** "Still taking fish oil?…" (17 cards, iniciados em 13/11/2026) — 1001969372979371.
- **UGC em vídeo** (mulher falando para a câmera): 872855722165983.

#### Classificação

- **Evidência:** evidencia_de_tracao (Meta + Google).
- **Prioridade:** prioridade_alta.
- **Confiança:** alta.
- **Regulatório:** alergênico de frutos do mar a confirmar no rótulo; elegibilidade HSA/FSA a verificar.

### Oferta 5 — Ilyra — Tart Cherry Extract

- **Mercado de venda:** EUA (Ad Library US; o seletor da loja mostrou "Brazil (USD $)" por geolocalização).
- **Mecanismo alegado:** cereja ácida extraída a frio, 3.600 mg por porção; inflamação, gota e ácido úrico, articulações.
- **Página:** https://tryilyra.com/products/tart-cherry-extract — 2026-11-17.
- **Preço:** 1 frasco US$ 34,99 (ref. US$ 59,99); Buy 2 Get 1 US$ 59,99; Buy 3 Get 2 US$ 84,99.

#### Histórico publicitário

- **Consulta:** Meta, frase exata "tryilyra.com", 2026-11-17T19:10:41Z.
- **Método:** **amostra** de 230 cards de ~1.400 exibidos. Os números são piso.
- **Anúncios ativos da oferta (amostra):** ≥284 (223 cards); 157 com 30+ dias.
- **Anúncio ativo mais antigo na amostra:** 936697478688764, iniciado em 2026-08-11, com 98 dias.
- **Exclusões:** produtos "sleep" e "toe fungus" do mesmo domínio, mais 2 cards de um concorrente.
- **Páginas:** Ilyra (155), Essential Joint Finds (40), "Dr. James Calder, MD" (13), Denise Holloway (12) e "Carol Rayes, RN" (3).
- **Google:** 0 anúncios.

#### Recorrência

- **Dose diária e cápsulas por frasco:** não observadas.
- **Assinatura:** alegada (só o link "Manage Subscription").
- **Potencial de recompra (inferência):** alto, por ser cápsula diária com kits de 3 e 5 frascos.

#### Criativos

- **Hook (207 cards):** "You've heard tart cherry helps with inflammation. But you've probably never felt it actually do anything." — 936697478688764.
- **Listicle "We tested 34 tart cherry supplements…"** (página Essential Joint Finds), em variações para gota, artrite e "alternativa ao alopurinol": 3687206698093592, 1832772427760234 e 3052289665130994.
- **Persona médica sobre ácido úrico:** "If your uric acid is between 6.0 and 7.9…" — 1631358488685785.

#### Classificação

- **Evidência:** sinais_de_atividade.
- **Prioridade:** prioridade_alta (≥284 anúncios na amostra; 157 cards com 30+ dias).
- **Confiança:** moderada (amostra).
- **Regulatório:** posicionamento como alternativa ao alopurinol (substituição de medicamento) e "stay out of a wheelchair": risco alto. A persona "MD" não foi verificada.
- **Observação:** o PDP tem frases idênticas às da GoodGrove ("3600mg of cold-extracted tart cherry", blocos "Convenient Daily Format", "Trusted Manufacturing"). Uma relação entre as marcas é **hipótese**: o anunciante Google da GoodGrove é Flophead Ventures LLC, e a Ilyra não tem anúncios no Google.

### Oferta 6 — BioRoot Labs — Turmeric Curcumin Capsules 1.000 mg

- **Mercado de venda:** EUA (Ad Library US). A página alega "trusted in 31 countries".
- **Mecanismo alegado:** 95% curcuminoides + pimenta-preta ("absorção até 2000%"). O mesmo SKU é anunciado com ângulos de articulação, fígado e cérebro.
- **Página:** https://biorootlabs.com/products/turmeric-curcumin-capsules-1000mg — 2026-11-17. Variante dos anúncios: `...-1-000mg-o2`.
- **Preço:** Buy 1 (1 mês), Buy 2 Get 1 (3 meses) e Buy 3 Get 2 (5 meses). Foi exibido em **GBP** (£ 20/40/60) por geolocalização; o preço em USD não foi observado.

#### Histórico publicitário

- **Consulta:** Meta, frase exata "biorootlabs.com", 2026-11-17T19:09:26Z.
- **Método:** **amostra** de 247 cards de ~1.300.
- **Anúncios ativos do SKU de cúrcuma (todas as posições):** ≥291 (226 cards); 127 com 30+ dias.
- **Anúncio ativo mais antigo:** 2509798346160939, iniciado em 2026-08-01, com 108 dias.
- **Ativos do domínio (amostra):** 312. Também há magnésio e outros produtos.
- **Páginas (19):** BioRoot Labs (119), Healthy Brain Community (34), Liver Support Community (32), The Joint Pain Journal (15), Dr Ruth White e creators em parceria (Kiser Sisters, Jillfluence, KIKI ELY etc.).
- **Google:** 74 anúncios, anunciante verificado "Hyperlink Digital LLC".

#### Recorrência

- 3 cápsulas/dia (página); "1 month supply" por frasco. O número de cápsulas não foi observado.
- **Assinatura:** alegada (link "Manage Subscription").
- **Potencial de recompra:** alto.

#### Criativos

- "You've heard turmeric helps with inflammation. But you've probably never felt it actually do anything…" (133 cards) — 1077813854907729.
- Vídeo de 2:53 "Tired of waking up stiff and sore?" — 1473085841585751.
- Ângulos fígado e cérebro pelas páginas-comunidade: 1732673554432520 e 1108723071632539.

#### Classificação

- **Evidência:** evidencia_de_tracao (Meta + Google).
- **Prioridade:** prioridade_alta.
- **Confiança:** moderada. A contagem é amostral e não separa os ângulos; o recorte só articular é menor que 291.
- **Regulatório:** alegações distintas para fígado, cérebro e articulação sobre o mesmo produto.

### Oferta 7 — GoodGrove — Cold-Pressed Tart Cherry Extract

- **Mercado de venda:** EUA ("Free USA Shipping"). O anunciante Google verificado é "FLOPHEAD VENTURES LLC".
- **Mecanismo alegado:** cereja ácida extraída a frio, 3.600 mg; articulações, cartilagem e ácido úrico.
- **Página:** https://trygoodgrove.com/products/tart-cherry-extract — 2026-11-17.
- **Preço:** 1 frasco US$ 39,99 (ref. US$ 59,99); 2 US$ 69,99; 3 US$ 89,99. Refil "US$ 69,99 — ships every 4 weeks".

#### Histórico publicitário

- **Consulta:** Meta, frase exata "trygoodgrove.com", 2026-11-17T19:04:10Z.
- **Método:** **amostra** de 277 cards de ~1.700 exibidos. É a maior diferença entre o contador e a amostra no conjunto.
- **Anúncios da oferta (amostra):** ≥245 (229 cards); 84 com 30+ dias.
- **Anúncio ativo mais antigo na amostra:** 2628634814276397, iniciado em 2026-09-23, com 55 dias.
- **Exclusões:** o produto "Tart Cherry Sleep" (50 cards) e 2 cards de concorrente.
- **Páginas:** Summit Point Health Hub (80), Melissa Hayes (70), Renee Donnelly (47), Joint Health Club (18) e Trevor Langford (14).
- **Google:** 73 anúncios.

#### Recorrência

- **Dose e cápsulas:** não observadas.
- **Assinatura:** verificada ("Save More With Automatic Refills"; "Refill Ships Every 4 Weeks").
- **Potencial de recompra:** alto.

#### Criativos

- "This almost never happens. GoodGrove is running a limited-time promotion…" (47 cards) — 27633474576329420.
- "Looking to Take Control of Your Joint Health Naturally? 🦵" (45 cards) — 4584094601865420.
- **Histórias longas de personas sem relação direta com o produto** (herança, "I am a sleep physician", gêmeas Amish): 1662494118813951, 1419806389785832 e 1562918968494259.
- **Vídeos UGC** (capturas).

#### Classificação

- **Evidência:** evidencia_de_tracao (Meta + Google).
- **Prioridade:** prioridade_alta (≥245 anúncios; 84 cards com 30+ dias).
- **Confiança:** moderada.
- **Regulatório:** alegações sobre gota e ácido úrico; personas com histórias pessoais possivelmente fictícias (risco de anúncio enganoso).

### Oferta 8 — Plants Basically — Juicy Joint Extract

- **Mercado de venda:** EUA ("Free Shipping USA Orders Over $75"). Fundador e rosto: John Palmere (anunciante Google verificado).
- **Mecanismo alegado:** extrato herbal líquido (ulmária, garra-do-diabo, salgueiro-branco, cavalinha, cúrcuma, gengibre, pimenta-preta; 333 mg/mL). Os anúncios focam em hérnia de disco e ciática, além de articulações.
- **Página:** https://www.plantsbasically.com/products/juicy-joint — 2026-11-17.
- **Preço:**
  - Kits de 1, 2 e 3 frascos com economia de US$ 18,00 / 41,99 / 71,99.
  - 2 frascos por assinatura: US$ 77,99 (de US$ 119,98), a cada 8 semanas.
  - "Try once" 30% off: US$ 83,99.
  - "4 Free Welcome Gifts".

#### Histórico publicitário

- **Consulta:** Meta, frase exata "plantsbasically.com", 2026-11-17T19:03:44Z.
- **Método:** completa (126 de ~130), mais 23 IDs das buscas temáticas.
- **Anúncios ativos da oferta:** 156 (149 cards); 54 com 30+ dias, 11 com 180+.
- **Anúncio ativo mais antigo:** 831960976591356, iniciado em 2026-04-07, com 224 dias.
- **Páginas:** Plantsbasically (118), "JJ palmere com Plantsbasically" (15), JJ palmere (10) e creators (Jessandgoodeats, Sarah Intentionally).
- **Google:** 43 anúncios ("John Palmere").

#### Recorrência

- 60 porções de 1 mL por frasco (tabela nutricional). A dose diária não foi observada, então a duração não foi calculada.
- **Assinatura:** verificada ("Subscribe & Save 35% — Delivers every 8 weeks").
- **Potencial de recompra:** alto.

#### Criativos

- **Black Friday** "Save up to 40% + 4 FREE gifts" (59 cards) — 3071183809886473.
- "Herniated discs don't just cause back pain…" (19 cards, desde 22/05/2026) — 1636908654278796.
- **Fundador em vídeo:** "The worst part of disc pain isn't the pain, it's the fear" — 4417929761758878.
- **Imagem de ressonância/raio-X de coluna** (captura): 1926676808289979.

#### Classificação

- **Evidência:** evidencia_de_tracao (Meta + Google).
- **Prioridade:** prioridade_alta.
- **Confiança:** alta.
- **Regulatório:** "Herniated Discs Can Recover"; salgueiro-branco (salicilatos) pede advertência de interação e alergia; "120,000+ Happy Customers" e garantia de 365 dias são alegações da marca.

### Oferta 9 — Regensil — Joint Repair

- **Mercado de venda:** EUA (Ad Library US; preços em USD).
- **Mecanismo alegado:** silício + colágeno + minerais + vitamina K2 + boswellia para "joint repair" e ossos. Ângulo "evitar cirurgia de joelho".
- **Página:** https://regensil.com/pages/regensil-offer-v2 — 2026-11-17. Outros destinos: /pages/expert-knee-pain e quiz.regensil.com.
- **Preço:** 1 pote ("1 Month") US$ 39,96; 2 potes US$ 29,96/pote; 3 potes US$ 23,96/pote (ref. US$ 59,99).

#### Histórico publicitário

- **Consulta:** Meta, frase exata "regensil.com", 2026-11-17T19:06:05Z.
- **Método:** completa (89 de ~93), mais 2 IDs.
- **Anúncios ativos:** 131 (91 cards, com muitas variações); 32 com 30+ dias.
- **Anúncio ativo mais antigo:** 1860194334649926, iniciado em 2026-06-01, com 169 dias.
- **Página:** Regensil (91).
- **Google:** 2 anúncios ("Regensil").

#### Recorrência

- 2 cápsulas/dia (FAQ). O número de cápsulas por pote não foi observado; a página nomeia "1 Month" por pote.
- **Assinatura:** alegada (link "Manage Auto-Refills"; opção não vista na oferta).
- **Potencial de recompra:** alto.

#### Criativos

- **Depoimento** "My doctor was talking knee surgery. Three months later, I'm back to gardening…" (Linda R., 58), mais de 80 cards — 782435418224190.
- **Imagem 3D de joelho com texto sobre regeneração de cartilagem:** captura reduzida, texto a confirmar — 1916987423014113.
- **Novo** "The doctor promised the knee injection would buy me time…" (iniciado em 13/11/2026) — 2579854325774422.
- Poucos textos distintos (5); as variações estão na mídia.

#### Classificação

- **Evidência:** sinais_de_atividade.
- **Prioridade:** prioridade_alta.
- **Confiança:** alta.
- **Regulatório:** a promessa implícita de regenerar cartilagem e evitar cirurgia é de risco alto.

### Oferta 10 — Collanol — colágeno "3D" + cúrcuma (cápsula dupla DUOCAP)

- **Mercado de venda:** EUA. Advertorial en-us e es-us que leva a Amazon (B0DTLMG528) e Walmart. O anunciante Google verificado é "ВИТАСЛИМ ИНОВЕ ООД"; a origem búlgara é inferida pelo nome.
- **Mecanismo alegado:** "colágeno 3D" não desnaturado + cúrcuma micelar em cápsula-dentro-de-cápsula; "1 cápsula supera 10.000 mg de colágeno hidrolisado".
- **Páginas:** https://collanol.com/articles/en-us/facebook/tr/news/3d-collagen/three-dimensional-collagen-US-fb-tr.html e https://www.amazon.com/dp/B0DTLMG528 — 2026-11-17.
- **Preço (Amazon):** 20 cápsulas US$ 52,95; Subscribe & Save US$ 47,65. Existe opção de 60 cápsulas (preço não registrado).

#### Histórico publicitário

- **Consulta:** Meta, frase exata "collanol.com", 2026-11-17T19:08:37Z.
- **Método:** completa (54 de ~54).
- **Anúncios ativos:** 54; 46 com 30+ dias, 17 com 180+.
- **Anúncio ativo mais antigo:** 891308733852853, iniciado em 2026-01-21, com 300 dias.
- **Idiomas:** anúncios em inglês e espanhol, com destino a LPs en-us e es-us.
- **Google:** 2 anúncios.
- **Amazon (fato observado na página):** "1K+ bought in past month" e 4,0★. É um indicador do marketplace, não auditado.

#### Recorrência

- 1 cápsula/dia (título da Amazon); 20 cápsulas → 20 dias (cálculo).
- **Assinatura:** verificada (Subscribe & Save da Amazon).
- **Potencial de recompra:** alto, porque a embalagem dura menos de um mês.

#### Criativos

- **Vídeos curtos (0:13–0:58) de depoimento** em EN e ES: "The knee pain vanished" (827883826837127), "Mis rodillas no me duelen nada en absoluto" (1022803120771024).
- **Título fixo do link:** "Newly discovered 3D collagen eliminates joint pain" / "Nuevo colágeno 3D elimina el dolor articular".
- **Funil:** advertorial em formato de notícia → marketplace.

#### Classificação

- **Evidência:** evidencia_de_tracao (Meta + Google + indicador público da Amazon).
- **Prioridade:** prioridade_media. Justificativa: 54 anúncios na faixa de 20–99 e histórico consistente (46 cards com 30+ dias). Faltou volume ≥100 para alta.
- **Confiança:** alta.
- **Regulatório:** "eliminates joint pain" é uma alegação de cura; nos depoimentos do advertorial, a identidade dos autores não foi verificada.

## Candidatos não selecionados (fora do top 10)

| Marca — produto | Dados | Motivo |
|---|---|---|
| The Nova Bottle — "Menopaused / Her Again" (dor de quadril/articulação na menopausa) | 199 anúncios (136 cards), 21 com 30+ dias, mais antigo 271 dias | Mesma marca da oferta 3. Registrado para não duplicar marca no top 10; candidato forte a uma ficha própria. |
| Morning Vitality — OsteoShield (densidade óssea; LP de joelho "bone-on-bone") | ~460 exibidos; 132 cards, 128 com <30 dias; mais antigo 41 dias; páginas-persona "Dr. Schilling", "Margaret Davis" | Foco em osteoporose. `em_observacao` com sinal de **emergente** (entrada recente forte). https://health.morningvitality.com/ga/ostknbt1clv4/ |
| Sandhus Nutrition — Vitamin D3+K2 "Joint" (anúncios em espanhol para hispânicos nos EUA, venda pela Amazon) | 35 anúncios (22 cards) no ângulo articular; 17 com 30+ dias; mais antigo 61 dias; marca ~740 | Prioridade média, abaixo do top 10. Interessante como referência de público hispânico. |
| Mara Labs — BrocElite Plus (sulforafano) | 58 anúncios; 8 cards com 30+ dias | Volume médio, recente, multi-benefício |
| Nature Heart — Tart Cherry | Visto em 2 anúncios comparativos que citam GoodGrove/Ilyra | Não investigado (orçamento) |
| Elavate — Multi-Collagen | Dezenas de anúncios; marca do Reino Unido | Foco em pele e cabelo; articulação secundária |

## Fora de escopo (não suplementos ou problema diferente)

| Marca — produto | Categoria | URL | Motivo |
|---|---|---|---|
| Halsten — Stride | dispositivo de luz | https://tryhalsten.com/pages/vsl3 | Não é suplemento (~620 resultados no domínio) |
| Noralife — óleo de krill | suplemento para colesterol | https://secure.trynoralife.com/noralife-lis-ako-us | Problema fora do escopo |
| Morning Vitality — Magnesium Freeze | tópico | https://health.morningvitality.com/ga/magpdkncta/ | Não consumível |
| Anaconda, Stryde, One Compress, Cuurt, Griqos, Levide | joelheiras, compressão, ventosas | — | Não suplemento |
| Wuffes, Dog is Human, Cosequin, Zesty Paws, WINPRO | suplementos articulares para cães | — | Público animal |
| Trybronoir (Bronoir) | calçados | trybronoir.com | Não suplemento |

## Candidatos descartados e por quê

- **Pipitea (shop.pipitea.com):** anúncios de história longa pela página "Cholesterol Relief Community"; produto e ângulo articular não confirmados. Não investigado.
- **Freedom Joint Drops, Gold Seal Supplements, True Sea Moss, LifeCell, Rho Nutrition, Jocko Fuel, Black Girl Vitamins:** poucos cards nas buscas temáticas, ou articulação como benefício secundário. Não aprofundados, por orçamento.

## Recomendações de aprofundamento

1. **Completar a rolagem** de GoodGrove (~1.700), Ilyra (~1.400) e BioRoot (~1.300). Os números atuais são piso.
2. **Abrir os detalhes dos anúncios mais antigos** (IDs nas fichas) para ver alcance, plataformas e se a data reflete reativação.
3. **Analisar vídeos** (Arthrogenix com personagem animado; UGC de Haka e Plants Basically; Collanol EN/ES) com o `creative-reference-analyst`: extrair quadros e transcrição, sem republicar.
4. **Ficha própria para Nova "Her Again"** (menopausa + quadril), um subnicho com 199 anúncios.
5. **Monitorar OsteoShield** em 2–4 semanas para confirmar se é emergente.
6. **Investigar a relação GoodGrove × Ilyra** (copy idêntica no PDP): políticas, CNPJ/EIN, termos e endereço.
7. **Consultar o TikTok Creative Center** para as mesmas marcas.
8. **Revisão regulatória** antes de qualquer adaptação: substituição de medicamento (Ilyra), regeneração de cartilagem (Regensil), "eliminates joint pain" (Collanol), equivalência a injeção (VitalHydra) e personas médicas.

## Limitações de acesso e de confiabilidade

- **Meta Ad Library (EUA):** não mostra anúncios comerciais inativos. A "primeira data observada" é a do anúncio **ativo** mais antigo, então o histórico real pode ser mais longo.
- **Busca por frase exata do domínio:** capta anúncios cujo texto ou legenda contém o domínio. Anúncios com link encurtado ou sem legenda podem ficar de fora (subcontagem).
- **O contador "~N resultados" da Meta** é aproximado e nem sempre coincide com os cards carregados. Todas as contagens têm `count_is_estimate: true`.
- **Rolagem parcial:** 3 ofertas (marcadas como amostra).
- **Navegador geolocalizado no Brasil:** preços podem variar por região; a BioRoot exibiu GBP. Preços sem checkout.
- **Formato dos criativos:** identificado por capturas pontuais (6 grades da Ad Library) e pela duração de vídeo no texto do card. Áudio não transcrito.
- **TikTok Creative Center** não foi consultado. O WebSearch não foi usado: a descoberta foi feita só pela Ad Library.
- **Alegações das marcas** (clientes, frascos vendidos, assinantes) não são auditadas. O indicador da Amazon ("1K+ bought in past month") é público, mas não auditado.
- **Nenhum dado** de vendas, gasto, CPA ou ROAS foi obtido ou inferido.

## Arquivos

- `offers.json` — índice estruturado (10 ofertas, candidatos não selecionados, fora de escopo, limitações).
- `data/ads_<oferta>.csv` — IDs da Ad Library por oferta, com data de início, idade, página, destino e URL.
- `data/agg_<oferta>.json` — estatísticas agregadas por oferta e por domínio.
- Evidências locais, fora do Git: `evidence-local/articulacoes-eua-2026-11-17/` (capturas da Ad Library, markdown das páginas de venda e JSON bruto das buscas).
