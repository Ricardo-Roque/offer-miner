# Investigação publicitária — 5 marcas de canela-do-Ceilão

- **Data de observação:** 2026-11-17
- **Rodada 1 (manhã):** WebSearch + WebFetch, agregadores terceiros (admanage.ai, adlibrary.com), imprensa (CNN). Sem acesso às bibliotecas oficiais.
- **Rodada 2 (tarde, ~18h10–18h50 UTC):** **navegador embutido do Orca** (`orca-ide`, app 1.4.253), controlado via CLI (`goto`, `exec read`, `eval`, `screenshot`). Acesso **direto e sem login** a:
  - **Meta Ad Library** — funcionou (lista, texto completo, IDs, datas, status, players de vídeo).
  - **Google Ads Transparency Center** — funcionou (anunciante verificado, país, contagem; criativo Gentilia oculto por restrição de idade, exigiria login).
  - **TikTok Commercial Content Library** — funcionou (busca executada), **0 resultados**.
- Nenhum CAPTCHA, bloqueio ou login foi contornado. Nenhuma credencial usada.

## Método da rodada 2 (reprodutível)

1. Meta: busca por **frase exata do domínio** (`search_type=keyword_exact_phrase`, `country=ALL`), p.ex. `https://www.facebook.com/ads/library/?active_status=all&ad_type=all&country=ALL&q=%22lireaofficiel.com%22&search_type=keyword_exact_phrase&media_type=all`. Para Kenzendo, também `q="健然堂"` com `country=JP`.
2. Rolagem (3–4×) e extração do texto dos cards carregados → **amostra das primeiras ~40–80 entradas**, não o universo. O contador "~N resultados" é o exibido pela Meta e **não foi auditado**.
3. Filtro por produto: só cards cujo texto menciona a canela (`cannelle/ceylan`, `cannella/ceylon`, `シナモン`, `cinnamon/ceylon`).
4. Anúncio individual aberto por `https://www.facebook.com/ads/library/?id=<ID>`.
5. Vídeo: player ampliado **localmente** (CSS no próprio navegador), `currentTime` ajustado em 0, 1, 2, 3, 5, 8, 15 s + 25/50/75 % + final, captura de tela de cada quadro. Nenhum arquivo de vídeo baixado. Áudio **não** transcrito; diálogo lido pelas legendas embutidas.
6. Capturas mantidas fora do repositório (diretório temporário da sessão) — ver "Capturas" no fim.

> Os rótulos de botão (CTA) aparecem traduzidos para o idioma da interface (pt-BR): "Comprar agora" ≈ *Shop Now*, "Saiba mais" ≈ *Learn More*, "Ver detalhes" ≈ *See details*.

---

## Resumo por marca (Meta, amostra carregada, só anúncios de canela)

| Marca | Total exibido pela Meta | Cards na amostra | De canela | Ativos / inativos | Com vídeo | Removidos pela Meta | Início mais antigo → mais recente | Páginas anunciantes |
|---|---|---|---|---|---|---|---|---|
| **Liréa** | ~2.200 | 75 | 63 | 48 / 15 | 25 (0:08–5:13) | 4 | 09/05/2026 → 04/11/2026 | 1: "Liréa" |
| **Gentilia** | ~1.100 | 70 | 65 | 39 / 26 | 0 (texto longo + imagem) | 1 (+4 de página desativada) | 21/08/2026 → 26/10/2026 | 6 (5 personas + "Gentilia") |
| **Kenzendo** (`kenzendo.store`) | ~51 | 38 | 16 | 16 / 0 | 11 (0:08–9:56) | 0 | 16/11/2026 (todos) | 2: "健然堂ポータル", "藤川 正則 医師" |
| **Kenzendo** (`"健然堂"`, JP) | ~54 | 36 | 23 | 23 / 0 | 6 | 0 | 14/10/2026 → 16/11/2026 | +1: "Takahashi Kenji - 高橋健司医師" (→ `rinaya-jp.com`) |
| **Metabolae** | ~26.000 | 67 | 63 | 62 / 1 | 35 (0:15–17:05) | 0 | 16/07/2026 → 06/11/2026 | 9 (marca + personas + "comunidades") |
| **Resilia** | ~4.400 | 78 | **6** | 6 / 0 | 5 (5:28–9:54) | 0 (+2 de página desativada) | 03/11/2026 → 15/11/2026 | 5 páginas "report/journal" |

- **Fato observado:** todas as 5 marcas têm anúncios reais na Meta; Liréa, Gentilia, Kenzendo e Metabolae anunciam majoritariamente **a canela**. Resilia anuncia sobretudo outros produtos (orégano, alho, circulação); canela é minoria recente.
- **Inferência:** volume e duração indicam investimento contínuo, **não** vendas. Classificação mantida em `sinais_de_atividade`.

## Google Ads Transparency (por domínio)

| Domínio | Anúncios | Anunciante verificado | País do anunciante | Formato observado |
|---|---|---|---|---|
| `lireaofficiel.com` | 6 | **ACH Group** (`AR09933043063859445761`) | França | Texto de pesquisa: "Cannelle de Ceylan en gélules – Gélules de cannelle bio"; "Régulation de la glycémie – Complément pour la glycémie" |
| `gentilia.it` | 1 | **ERCOWISE LLC** (`AR08257608344966004737`) | Estados Unidos | Conteúdo oculto ("restrição de idade", exige login) |
| `kenzendo.store` | 0 | — | — | — |
| `rinaya-jp.com` | 0 | — | — | — |
| `metabolae.com` | ~200 | **BAT Partners LLC** | (não lido) | — |
| `resilia.shop` | ~8.000 | **Sack Consulting Inc** | (não lido) | vídeo presente |

- **Fato observado:** razões sociais diferentes por marca no Google. **Não** confirma nem descarta operador comum (ver "Padrões entre marcas").

## TikTok Commercial Content Library

- Busca via interface (campo + "Pesquisar"), janela padrão de 30 dias: **0 anúncios** para `Lirea`/`cannelle` (FR), `Gentilia`/`cannella` (IT). Japão não é coberto pela biblioteca.
- **Limitação:** o resultado zero também aparece para termos genéricos (`cannelle`), então a busca pode não cobrir palavras do criativo, só nome do anunciante. Ausência = **confiança moderada**, não prova.

---

## Liréa (França, francês) — criativos efetivamente visualizados

Página anunciante: **Liréa** (`view_all_page_id=1138628302657905`). Plataformas exibidas: Facebook, Instagram, Audience Network, Messenger/Threads. Indicador "Transparência da UE" presente.

### L1 — Microdrama hospitalar (vídeo 5:06) · ID `2183910109197467`
- **Link:** https://www.facebook.com/ads/library/?id=2183910109197467
- **Status:** ativo · início 04/11/2026 · 1 anúncio com este criativo.
- **Formato:** vídeo vertical 9:16 (360×640), 5:06, legendas embutidas brancas em caixa.
- **Hook (copy):** "Six ans de metformine. Tous les jours. Sans en oublier un seul. Et pourtant, un matin, Martine se réveille aux urgences."
- **Primeiros segundos:** 0 s — corredor de hospital, paciente de camisola com bandeja de comida, enfermeira ao fundo: "Martine ?" → 1–2 s "Bonjour, Sophie." → 3 s close na enfermeira "C'est quoi, ça ?" → 5 s "Votre dossier dit : à jeun strict." → 8 s "Alors vous savez que vous n'avez…" → 12 s quarto, "Mes chiffres."
- **Estrutura:** conflito (paciente quebra jejum) → médico/enfermeira desconfiam ("Elle croit que j'ai changé", 40 s) → revelação (vizinha de leito ex-endocrinologista, 90 s "Vous êtes médecin ?") → objeção ("J'ai déjà essayé des gélules de cannelle", 180 s) → prova numérica ("5,9 ?", 270 s) → produto na mão + garantia ("Satisfaite ou remboursée", 300 s). Produto só aparece no final.
- **Estilo visual:** cinematográfico realista, luz fria hospitalar; aparência **compatível com vídeo gerado por IA** (hipótese, não confirmada).
- **CTA:** headline "Ce que sa voisine de lit lui a dit cette nuit-là" · "2 achetés = 2 offerts · satisfaite ou remboursée 30 jours" · botão *Shop Now*.
- **Evidências usadas:** narrativa de personagem, autoridade (ex-endocrinologista), contraste com metformina, "+15 000 personnes", garantia.

### L2 — Animação 3D "28 jours" (vídeo 1:28) · ID `2253175732202903`
- **Link:** https://www.facebook.com/ads/library/?id=2253175732202903 · inativo (28/07–09/11/2026) · 2 anúncios.
- **Hook:** cena noturna, idosa sentada na cama, relógio 3:00, selo "2ème fois"; legenda: "Si quelqu'un qui se lève 3 [fois par nuit] à cause de [sucre] prenait pendant 28 [jours]…" (cenário hipotético).
- **Sequência:** 5 s pacote + calendário "28" ("la metformine de…") → 8 s personagem fofo dentro de vaso sanguíneo → 15 s tela dividida ✗/✓ ("vraie cannelle de…") → 22 s "à destination" → 44 s antes/depois (cansada × sorridente, "sèche au réveil") → 66 s produto com mascotes ("l'extrait concentré 12[:1]") → 86 s "ça se prend" / "«il en reste !»".
- **Estilo:** animação 3D estilo cinema infantil, legendas karaokê (palavra-chave em ciano).
- **CTA:** "Se lever trois fois par nuit « à cause du sucre », ce n'est pas une fatalité. Voici 28 jours, jour par jour." · "1+1 offert · Garanti 30 jours" · *Shop Now*.

### L3 — UGC oferta-relâmpago (vídeo 0:17) · ID `1012844728266644`
- **Link:** https://www.facebook.com/ads/library/?id=1012844728266644 · ativo desde 17/07/2026 · 2 anúncios. Variantes do mesmo texto: `27638007069202976`, `1067214159115365`.
- **Hook visual 0–1 s:** mulher em cozinha, segurando 2 pacotes, faixa fixa "🚨OFFRE 1€/JOUR🚨" + "VITE ! SE TERMINE À MINUIT"; legenda "2 boîtes Liréa…".
- **Sequência:** "pour le prix" → "et voici comment l'avoir aujourd'hui" → 5 s mãos abrindo caixa ("cliquez simplement sur") → 13 s close na cápsula ("la livraison gratuite") → 15 s "cette offre flash".
- **Estilo:** UGC selfie, luz natural; urgência e preço como mensagem principal.
- **CTA:** "Offre flash ce soir · 1+1 offert" · *Shop Now*.

### L4 — Fundador "Alerte aux faux" (vídeo 1:06) · ID `984263778060761`
- **Link:** https://www.facebook.com/ads/library/?id=984263778060761 · ativo desde 23/10/2026. Variantes: `1744536423906305`, `1588916942987152`, `2201148774153475`.
- **Hook 0–3 s:** homem sentado em armazém, fileira de pacotes Liréa à frente, faixa azul "ALERTE AUX FAUX"; "[si vous avez] acheté Liréa sur Amazon… c'est un faux".
- **Estrutura:** alerta → "écoutez bien" → contrafações "explosent" → "pas en pharmacie ni magasin" → "c'est par le lien en dessous" → "commandez le vrai".
- **Estilo:** talking head estático, legendas com palavras em roxo.
- **CTA:** "Méfiez-vous des contrefaçons de cannelle Liréa" · *Shop Now*.

### L5 — Papel recortado "robinet" (vídeo 1:35) · ID `1952463358756102`
- **Link:** https://www.facebook.com/ads/library/?id=1952463358756102 · inativo (17/07–09/11/2026).
- **Hook:** "90 secondes en papier découpé pour comprendre ce qu'aucune consultation de quinze minutes ne prend le temps d'[expliquer]"; tela: mulher dormindo, relógio 22:00, "Vous n'avez rien mangé depuis 22h".
- **Sequência:** "et pourtant au [réveil]" → medidor de glicemia no vermelho → fígado "qui s'emballe" → torneira derramando cubos de açúcar ("plus s'arrêter") → produto com ilustração de canela ("celle du Sri Lanka") → café → cápsula → fígado sorrindo → antes/depois em papel.
- **Estilo:** estética stop-motion de papel recortado, paleta terrosa.
- **CTA:** "Il y a un robinet dans votre corps qui ne ferme plus la nuit. Le voici." · "Le mécanisme en 90 s · Garantie 30 jours" · *Shop Now*.

### L6 — Animação 3D "metformine" (vídeo 4:16) · ID `1134782529421301`
- **Link:** https://www.facebook.com/ads/library/?id=1134782529421301 · ativo desde 08/10/2026.
- **Hook 0–5 s:** idosa 3D na cozinha, caixa "Metformine" na bancada, mão na barriga: "Tu prends ta metformine tous les matins… ton taux [baisse]… et pourtant ton ventre…".
- **Sequência:** "il y a une raison" → fígado com torneira ("moins de sucre") → raio-X do tronco ("30 minutes, le comprimé") → partículas na água escura ("ne va nulle part") → nuvem sobre a cabeça ("le coup de barre") → personagem aponta para baixo ("si tu cliques").
- **Estilo:** 3D estilo animação de estúdio, tratamento em "tu".
- **CTA:** "Ce que fait ton corps dans les 3 heures après ta metformine" · *Shop Now*.

### L7–L9 — Imagens
| ID | Status / início | Imagem (descrição) | Hook | Headline / CTA |
|---|---|---|---|---|
| `1508654571040358` | ativo · 13/07/2026 | Corredor de armazém, mão segurando pacote; texto "On a produit trop de sachets Liréa ce mois-ci 😅 / Aide-nous à vider l'entrepôt / 1+1 OFFERT" | "On a sur-stocké ce mois-ci. Du coup c'est votre problème maintenant 😄" | "1+1 offert aujourd'hui seulement !" · *Shop Now* |
| `2119393105350095` | ativo · 29/10/2026 | Foto de corredor hospitalar com equipe médica enfileirada de cabeça baixa | "Un homme de 54 ans est mort mardi dernier dans les bras de sa femme." (medo/morte súbita) | "« Ça a vraiment marché, merci infiniment. » - Émilie T." · *Learn More* |
| `1737759380776286` | ativo · 24/09/2026 | Mão com luva preta escrita "N'achetez pas ça" ao lado do pacote, sala de diálise | "S'il vous plaît, n'achetez pas la cannelle de Ceylan Liréa…" (psicologia reversa; persona enfermeira de diálise) | "N'achetez surtout pas !" · "4,8/5 · +12 500 avis" · *Learn More* |

### Outros ângulos Liréa vistos só pelo texto (não abertos)
- Enfermeira 34 anos recusa metformina (`1698650378068134`, ativo; `2055936068351963` contém "TEXTE PRINCIPAL — copie tout ce qui est entre les lignes :" — aparentemente instrução interna de briefing publicada por engano; inferência).
- "Ma diabétologue m'a dit… « Vous fabriquez votre sucre la nuit »" (`1726645045421984`, vídeo 5:13).
- "La Metformine fonctionne. Mais personne ne parle de ce qui vient avec…" (vários IDs).
- Cassia × Ceylan (`1619345149609893`, `2531490143948396`).
- Preço ancorado: "Cure Complète 59,90 € au lieu de 119,80 € — 0,50 €/jour" (`2385174108558513`); "sachet à 14,95 €" (`1522964562936423`).
- Black Friday + metformina (`1682669986755731`, ativo desde 02/11/2026).
- 4 anúncios de 09–11/2026 **removidos pela Meta** por violar Padrões de Publicidade (ex.: `1575857106865202`, `3203641526502249`, `1944110046586258`, `1725925145710124`).

---

## Gentilia (Itália, italiano) — criativos efetivamente visualizados

**Formato dominante:** texto longo narrativo (história em 1ª pessoa, centenas de palavras) + foto quadrada simples (600×600) + headline "LEGGI QUESTO se hai…". **Nenhum vídeo** na amostra. Veiculados por **páginas-persona** (médicos, enfermeira, "diários") que apontam para `gentilia.it`.

| ID | Página anunciante | Status / início | Imagem | Hook | Headline / CTA |
|---|---|---|---|---|---|
| `1080649297659813` | Dott. Fabrizio Galli - Endocrinologo | ativo · 15/09/2026 | Foto do pacote "Gentilia Cannella di Ceylon" sobre mesa | "Mia moglie Carolina prendeva la cannella di Ceylon da esattamente 19 giorni quando il suo medico di base la chiamò…" | "LEGGI QUESTO se hai la glicemia alta" · *Shop Now* |
| `2253085015543875` | Il Diario della Glicemia | ativo · 27/09/2026 | Mulher caminhando em trilha na floresta | "Il mio endocrinologo mi ha dato due opzioni per il diabete di tipo 2…" | "LEGGI QUESTO se hai il diabete di tipo 2" · *Learn More* |
| `2510128156144033` | Il Diario del Colesterolo | ativo · 25/10/2026 | Homem idoso fazendo trilha | "Sono un cardiologo svizzero. Il mio LDL ha raggiunto 196…" | "LEGGI QUESTO se hai il colesterolo alto" · *Learn More* |
| `2346016919563069` | Il Diario della Glicemia | ativo · 12/10/2026 | Foto do pacote | "Se stai prendendo il brand Gentilia e hai già una routine di farmaci…" — assinado "Cristian, Cofondatore di Gentilia" | "Cannella di Ceylon 7200mg Equivalente in Olio MCT" · *Shop Now* |
| `1612780430444542` | Lucia Casali | ativo · 09/09/2026 | Foto do pacote | "Il 78% dei pazienti con glicemia alta cronica sviluppa danni vascolari irreversibili…" | "LEGGI QUESTO se hai la glicemia alta" · *Learn More* |

- **Estrutura narrativa típica:** abertura de choque/identidade → história pessoal com números de exame (HbA1c 7,1→6,4; 13,4→11,2) → tentativa frustrada com cápsulas comuns → "descoberta" do mecanismo (lipossolubilidade, "porte" das células, MCT) → resultado semana a semana → produto.
- **Ângulo colesterol:** página "Il Diario del Colesterolo" vende a **mesma canela** (texto menciona cannella). É ângulo, não outro produto.
- **Sinal regulatório:** página "Dott.ssa Paola Cipriani - Ginecologa" **desativada pela Meta** (4 anúncios, jun–jul/2026; produto não identificável); 1 anúncio removido (`3618353321652762`). Personas médicas podem ser fictícias — **não assumir que são profissionais reais**.

---

## 健然堂 Kenzendo (Japão, japonês) — criativos efetivamente visualizados

Páginas: **健然堂ポータル** (marca), **藤川 正則 医師** (persona médico; cardiologista em uma copy, nefrologista em outra), **Takahashi Kenji - 高橋健司医師** (persona; domínio `rinaya-jp.com`). Lote principal estreou em **16/11/2026** (Black Friday), "tempo total ativo: 18–19 h" na hora do acesso.

### K1 — Microdrama hospitalar (vídeo 9:56) · ID `1863077484847834`
- **Link:** https://www.facebook.com/ads/library/?id=1863077484847834 · ativo desde 16/11/2026 · página 健然堂ポータル.
- **Primeiros segundos:** 0–1 s corredor hospitalar, paciente idosa de pijama com bandeja de comida, enfermeira atrás → 2 s "あら、理恵さん。" → 3–5 s close na enfermeira → 8 s "カルテには絶飲食とあります。" (prontuário diz jejum absoluto) → 15 s paciente e enfermeira.
- **Sequência:** 149 s "全部やったの。" (fiz tudo) → 298 s explicação de mecanismo ("反応するよう信号を送ります") → 447 s pacote 健然堂 sobre a mesa → 594 s produto em primeiro plano.
- **Comparação:** **mesmo roteiro e mesma encenação** do vídeo Liréa L1 (`2183910109197467`): paciente com bandeja no corredor, enfermeira chama pelo nome, "dossier dit : à jeun strict" = "カルテには絶飲食". Produto só no final. Versão JP quase 2× mais longa.
- **Copy:** "自然の力で、健やかな血糖バランスをサポートしませんか？🌿 … ✅ 200件以上の臨床研究 ✅ 吸収をサポートするMCTオイル配合" · *Learn More* → `kenzendo.store`.

### K2 — "Viagem da cápsula" 3D (vídeo 3:26) · ID `1140487985356612`
- **Link:** https://www.facebook.com/ads/library/?id=1140487985356612 · ativo desde 16/11/2026 · página 藤川 正則 医師. Variantes: `1655501192896368` (3:26), `940230682354093` (2:29), `1700223384928451` (1:57).
- **Hook 0–3 s:** faixa fixa "本物のセイロンシナモンは血糖値にどう働く？🤔"; mão segura cápsula diante do pacote: "うっかり、本物のセイロンシナモンのソフトジェルを飲み込んでしまった。" (sem querer engoli a cápsula).
- **Sequência:** 3 s anatomia 3D do esôfago → 5 s "その後72時間、" → 15 s cápsula descendo ("食道を滑り下り") → 52 s molécula dourada ("全身の細胞に届きます") → 103 s hemácias ("動脈に、緩むよう伝える") → 155 s idoso medindo glicose ("何年も見ていなかった" [número]) → 204 s pacote em jardim japonês ("この分がなくなる前に" — escassez).
- **Estilo:** render 3D anatômico + legendas karaokê amarelas.
- **CTA:** *Learn More* → `kenzendo.store`.

### K3 — Unboxing Black Friday (vídeo 0:08) · ID `1483725747247937`
- **Link:** https://www.facebook.com/ads/library/?id=1483725747247937 · ativo desde 16/11/2026.
- **Visual:** mãos de pessoa idosa sobre mesa de madeira, pacote cai na mesa, abre, despeja cápsulas na palma. Sem legenda.
- **Copy:** "🖤 Kenzendo ブラックフライデー 🖤 … 3個ご購入で、さらに2個無料。合計5個" (compre 3, leve +2) · *See details*.

### K4–K5 — Imagens
| ID | Página | Status | Imagem | Hook | Headline / CTA |
|---|---|---|---|---|---|
| `1431133619130686` | 藤川 正則 医師 | ativo · 16/11/2026 | Arte de produto: "セイロンシナモン 高吸収型 (MCTオイル配合)", bullets 12:1 7.200 mg, MCT absorção 3×, Sri Lanka, 5 estrelas | "体調は良かったので、問題ないと思っていました…。でも実は、高い血糖値が…私の腎臓を傷つけていたのです。" (ângulo renal, persona nefrologista) | "セイロンシナモン 7,200mg相当 MCTオイル配合｜健然堂" · "90日間返金保証" · *See details* |
| `1141597035190365` | Takahashi Kenji - 高橋健司医師 | ativo · 14/10/2026 | Foto de refeição japonesa (salmão, arroz, missô, umeshu) | "私は糖尿病の療養指導をする仕事をしています。HbA1cは7.4でした。それを、わずか12週間で5.4まで下げました。" | `RINAYA-JP.COM` · "⭐️⭐️⭐️⭐️⭐️ — 8,952人以上のお客様にご愛用いただいています！" · *See details* |

- **Domínio irmão (hipótese forte):** as copies da persona Takahashi citam o produto como **"健然堂（RINAYA）"** e apontam para `rinaya-jp.com`; 3 cards da página 健然堂ポータル mencionam os dois domínios. Hipótese: `rinaya-jp.com` = domínio anterior/espelho do mesmo produto. Não verificado no site.
- **Sinal de tradução:** copy JP da persona Takahashi (`1139552701904607`) cita "CVS", "デイビッドさん", "タッカーさん" — elementos de roteiro norte-americano traduzido.
- **Fora de escopo (descartado):** páginas "午前3時の快眠研究会" (magnésio/sono) e "骨の健康と骨粗しょう症を学ぶ会" (ossos) também anunciam `kenzendo.store`, mas outro produto.

---

## Metabolae e Resilia (checagem rápida, só texto)

- **Metabolae (EUA):** 63/67 cards de canela; 62 ativos; 35 vídeos (até 17:05). Páginas: Metabolae, "Cristian - Co-Founder, Metabolae", "Caroline Moore", "John Tucker", "Sandra Keller, RN", "Dr. Matthew Walker", "Dr. Cornelius Carter", "Blood Sugar Balance Community", "Blood Sugar Support Group". Vídeos não abertos nesta rodada.
- **Resilia (EUA/UK):** apenas 6/78 cards da amostra são de canela, todos de 11/2026, em páginas tipo "Glucose Health Journal", "Healthy Insulin Report" (vídeos 5:28–9:54). Restante: outros produtos (confirma rodada 1: foco não é canela).

---

## Padrões entre marcas (copy observada; propriedade **não** confirmada)

| Template | Metabolae (EUA) | Gentilia (IT) | Liréa (FR) | Kenzendo (JP) |
|---|---|---|---|---|
| Microdrama hospitalar, jejum quebrado, produto no fim | — | — | `2183910109197467` (visto) | `1863077484847834` (visto) |
| "Cristian, cofundador" | página "Cristian - Co-Founder, Metabolae" | `2346016919563069` "Cristian, Cofondatore di Gentilia" | — | — |
| Real × falsificação da Amazon (fundador) | `2195193474687110` "real Metabolae versus the fake Amazon copycat" | — | `984263778060761` (visto) | — |
| Cardiologista, 12 anos estudando colesterol | `2002046113835829` Dr. Matthew Walker | `861986350311624` | — | `2541741866306379` (Takahashi) |
| "I don't give a f*ck if this upsets you" | `1839256067232603` Caroline Moore | `2126264544595849` "non me ne frega un c*zzo" | — | — |
| "Created for people who've tried everything" | `2218643705532853` | `1026958960370565` | — | — |
| Educador em diabetes, HbA1c 7,4 → 5,4 em 12 semanas | — | `29695334770069798` | — | `1141597035190365` |
| Enfermeira recusa metformina | página "Sandra Keller, RN" | `3468709280005340` (26 anos) | `1698650378068134` (34 anos) | — |
| Cenário hipotético "se alguém tomasse por N dias" | hook "prediabetic man with an A1C of 6.4… 30 days" (rodada 1) | `1068327646096803` "prediabetico, glicata 6,4… 30 giorni" | `2253175732202903` (28 jours, visto) | — |

- **Fato observado:** roteiros e copies são traduções/adaptações uns dos outros; produto idêntico (12:1, 7.200 mg equiv., MCT); embalagens com o mesmo layout (pacote stand-up, faixa marrom, ilustração de canela).
- **Inferência (hipótese):** mesmo playbook — operador comum, agência comum ou fornecedor white-label comum. Razões sociais no Google diferem (ACH Group/FR, ERCOWISE LLC/EUA, BAT Partners LLC), então **não afirmar dono comum**.

## Riscos e sinais regulatórios

- Personas de médicos/enfermeiros possivelmente fictícias + alegações de HbA1c, rins, LDL, contraste com metformina/estatina = **alegações médicas fortes**. Anúncios removidos pela Meta (Liréa 4, Gentilia 1) e páginas desativadas (Gentilia, Resilia) confirmam fiscalização ativa.
- Cópia de estrutura é possível; cópia de texto/personas/alegações **não** é recomendável. Qualquer adaptação exige revisão científica e jurídica no país de destino.

## Limitações desta investigação

1. Amostra = primeiros 36–78 cards por busca; universo não percorrido. Contadores "~N resultados" são da Meta, não auditados.
2. Áudio não transcrito (só legendas embutidas). Frames em resolução baixa (360×640).
3. Hipótese "vídeo gerado por IA" baseada só em aparência visual.
4. TikTok: 0 resultados podem refletir limitação de busca (nome do anunciante), não ausência real.
5. Google: criativo Gentilia oculto por restrição de idade (exigiria login; não feito).
6. Nenhum dado de gasto, alcance, vendas, CPA ou ROAS foi obtido. Liréa/Gentilia mostram "Transparência da UE" (alcance/segmentação na UE) — **não aberto** nesta rodada; é a próxima fonte para alcance.
7. Operação do navegador: o app Orca precisa ficar aberto durante toda a coleta (fechar a janela encerra o runtime).

## Capturas (não versionadas)

Frames e telas preservados localmente em `evidence-local/canela-ceilao-2026-11-17/<marca>/<ID>/` (pasta ignorada pelo Git, por cautela com direitos de terceiros). Índice versionado com URL de origem, tipo, caminho e SHA-256 de cada arquivo: [evidencias-visuais.md](evidencias-visuais.md). Origem: Meta Ad Library, `?id=<ID>` acima, 2026-11-17 ~18h20–18h45 UTC; quadros nos tempos listados em cada ficha.

> Nenhuma marca classificada como "vencedora". Volume, duração e status ativo = `sinais_de_atividade`.
