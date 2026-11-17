# Índice de evidências visuais — canela-do-Ceilão (2026-11-17)

Relaciona cada captura local com o anúncio de origem. **Os arquivos de mídia ficam em `evidence-local/` (ignorado pelo Git) e não são versionados**; este índice e os hashes, sim.

- **Coleta:** 2026-11-17, ~18h10–18h50 UTC, navegador embutido do Orca (`orca-ide` 1.4.253), Meta Ad Library sem login.
- **Método:** vídeos — player ampliado localmente via CSS, `currentTime` ajustado e captura de tela por quadro (nenhum arquivo de vídeo baixado); imagens — captura de tela do card do anúncio; `_card.txt` — texto do card extraído da página.
- **Integridade:** arquivos copiados do diretório temporário com `cp -p`, SHA-256 e tamanho conferidos origem × destino (147/147 idênticos) antes de apagar as cópias temporárias. Nenhum arquivo de mídia foi alterado depois da captura.
- **Tratamento de pranchas:** `sheet_*.png` de vídeos = montagem de quadros gerada com FFmpeg na hora da coleta; `sheet_*.png` de imagens = captura de tela inteira do card. `contact_*.png` e `imgs.png` = montagens. São derivados, não o criativo original.
- **Verificar (na raiz do repositório):**
  ```bash
  grep -oE '`evidence-local/[^`]+` \| [^|]+ \| `[0-9a-f]{64}`' knowledge/referencias/canela-ceilao-2026-11-17/evidencias-visuais.md \
    | sed -E 's/^`([^`]+)` \| [^|]+ \| `([0-9a-f]{64})`/\2  \1/' | sha256sum -c --quiet && echo OK
  ```
- **Uso:** material de terceiros, só para pesquisa interna. Não republicar. Análise detalhada de cada anúncio: [anuncios-criativos.md](anuncios-criativos.md).

## Anúncios

| Marca | Produto | ID do anúncio | URL original | Tipo de criativo | Pasta local | Arquivos | Observações |
|---|---|---|---|---|---|---|---|
| Liréa | Cannelle de Ceylan 12:1 + huile MCT | `2183910109197467` | https://www.facebook.com/ads/library/?id=2183910109197467 | Vídeo 9:16, 5:06 — microdrama hospitalar realista | `evidence-local/canela-ceilao-2026-11-17/lirea/2183910109197467/` | 15 | Ativo, início 04/11/2026. Frames 0–300 s. Produto só no final. Mesmo roteiro do Kenzendo 1863077484847834. Aparência compatível com IA (hipótese). |
| Liréa | Cannelle de Ceylan 12:1 + huile MCT | `2253175732202903` | https://www.facebook.com/ads/library/?id=2253175732202903 | Vídeo 9:16, 1:28 — animação 3D | `evidence-local/canela-ceilao-2026-11-17/lirea/2253175732202903/` | 13 | Inativo (28/07–09/11/2026). Hook de cenário hipotético "28 jours". |
| Liréa | Cannelle de Ceylan 12:1 + huile MCT | `1012844728266644` | https://www.facebook.com/ads/library/?id=1012844728266644 | Vídeo 9:16, 0:17 — UGC oferta-relâmpago | `evidence-local/canela-ceilao-2026-11-17/lirea/1012844728266644/` | 13 | Ativo desde 17/07/2026. Faixa fixa "OFFRE 1€/JOUR". |
| Liréa | Cannelle de Ceylan 12:1 + huile MCT | `984263778060761` | https://www.facebook.com/ads/library/?id=984263778060761 | Vídeo 9:16, 1:06 — fundador talking head | `evidence-local/canela-ceilao-2026-11-17/lirea/984263778060761/` | 13 | Ativo desde 23/10/2026. "ALERTE AUX FAUX" (Amazon). |
| Liréa | Cannelle de Ceylan 12:1 + huile MCT | `1952463358756102` | https://www.facebook.com/ads/library/?id=1952463358756102 | Vídeo 9:16, 1:35 — papel recortado | `evidence-local/canela-ceilao-2026-11-17/lirea/1952463358756102/` | 13 | Inativo (17/07–09/11/2026). Metáfora "robinet" (fígado). |
| Liréa | Cannelle de Ceylan 12:1 + huile MCT | `1134782529421301` | https://www.facebook.com/ads/library/?id=1134782529421301 | Vídeo 9:16, 4:16 — animação 3D | `evidence-local/canela-ceilao-2026-11-17/lirea/1134782529421301/` | 13 | Ativo desde 08/10/2026. Ângulo metformina, tratamento "tu". |
| Liréa | Cannelle de Ceylan 12:1 + huile MCT | `1508654571040358` | https://www.facebook.com/ads/library/?id=1508654571040358 | Imagem 338×600 — armazém / 1+1 offert | `evidence-local/canela-ceilao-2026-11-17/lirea/1508654571040358/` | 2 | Ativo desde 13/07/2026. |
| Liréa | Cannelle de Ceylan 12:1 + huile MCT | `2119393105350095` | https://www.facebook.com/ads/library/?id=2119393105350095 | Imagem 452×600 — corredor hospitalar | `evidence-local/canela-ceilao-2026-11-17/lirea/2119393105350095/` | 2 | Ativo desde 29/10/2026. Hook de morte súbita. |
| Liréa | Cannelle de Ceylan 12:1 + huile MCT | `1737759380776286` | https://www.facebook.com/ads/library/?id=1737759380776286 | Imagem 600×600 — luva "N'achetez pas ça" | `evidence-local/canela-ceilao-2026-11-17/lirea/1737759380776286/` | 2 | Ativo desde 24/09/2026. Psicologia reversa, persona enfermeira de diálise. |
| Gentilia | Cannella di Ceylon 7200mg equivalente in olio MCT | `1080649297659813` | https://www.facebook.com/ads/library/?id=1080649297659813 | Imagem 600×600 + texto longo — persona endocrinologista | `evidence-local/canela-ceilao-2026-11-17/gentilia/1080649297659813/` | 2 | Ativo desde 15/09/2026. Página "Dott. Fabrizio Galli - Endocrinologo". |
| Gentilia | Cannella di Ceylon 7200mg equivalente in olio MCT | `2253085015543875` | https://www.facebook.com/ads/library/?id=2253085015543875 | Imagem 600×600 + texto longo | `evidence-local/canela-ceilao-2026-11-17/gentilia/2253085015543875/` | 2 | Ativo desde 27/09/2026. Página "Il Diario della Glicemia". |
| Gentilia | Cannella di Ceylon 7200mg equivalente in olio MCT | `2510128156144033` | https://www.facebook.com/ads/library/?id=2510128156144033 | Imagem 600×600 + texto longo — ângulo colesterol | `evidence-local/canela-ceilao-2026-11-17/gentilia/2510128156144033/` | 2 | Ativo desde 25/10/2026. Página "Il Diario del Colesterolo". |
| Gentilia | Cannella di Ceylon 7200mg equivalente in olio MCT | `2346016919563069` | https://www.facebook.com/ads/library/?id=2346016919563069 | Imagem 600×600 + texto — "Cristian, cofondatore" | `evidence-local/canela-ceilao-2026-11-17/gentilia/2346016919563069/` | 2 | Ativo desde 12/10/2026. Mesma persona da Metabolae (EUA). |
| Gentilia | Cannella di Ceylon 7200mg equivalente in olio MCT | `1612780430444542` | https://www.facebook.com/ads/library/?id=1612780430444542 | Imagem 600×600 + texto longo | `evidence-local/canela-ceilao-2026-11-17/gentilia/1612780430444542/` | 2 | Ativo desde 09/09/2026. Página "Lucia Casali". |
| 健然堂 Kenzendo | セイロンシナモン 7,200mg相当 MCTオイル配合 | `1863077484847834` | https://www.facebook.com/ads/library/?id=1863077484847834 | Vídeo 9:16, 9:56 — microdrama hospitalar | `evidence-local/canela-ceilao-2026-11-17/kenzendo/1863077484847834/` | 13 | Ativo desde 16/11/2026. Mesmo roteiro do Liréa 2183910109197467. |
| 健然堂 Kenzendo | セイロンシナモン 7,200mg相当 MCTオイル配合 | `1140487985356612` | https://www.facebook.com/ads/library/?id=1140487985356612 | Vídeo 9:16, 3:26 — 3D "viagem da cápsula" | `evidence-local/canela-ceilao-2026-11-17/kenzendo/1140487985356612/` | 13 | Ativo desde 16/11/2026. Página "藤川 正則 医師". |
| 健然堂 Kenzendo | セイロンシナモン 7,200mg相当 MCTオイル配合 | `1483725747247937` | https://www.facebook.com/ads/library/?id=1483725747247937 | Vídeo 9:16, 0:08 — unboxing | `evidence-local/canela-ceilao-2026-11-17/kenzendo/1483725747247937/` | 13 | Ativo desde 16/11/2026. Black Friday 3+2. Sem legenda. |
| 健然堂 Kenzendo | セイロンシナモン 7,200mg相当 MCTオイル配合 | `1431133619130686` | https://www.facebook.com/ads/library/?id=1431133619130686 | Imagem 600×600 — arte de produto + texto (ângulo renal) | `evidence-local/canela-ceilao-2026-11-17/kenzendo/1431133619130686/` | 2 | Ativo desde 16/11/2026. Persona nefrologista. |
| 健然堂 Kenzendo | セイロンシナモン 7,200mg相当 MCTオイル配合 | `1141597035190365` | https://www.facebook.com/ads/library/?id=1141597035190365 | Imagem 600×600 — refeição japonesa + texto | `evidence-local/canela-ceilao-2026-11-17/kenzendo/1141597035190365/` | 2 | Ativo desde 14/10/2026. Persona "Takahashi Kenji"; destino rinaya-jp.com (domínio irmão, hipótese). |

Capturas do Google Ads Transparency por domínio ficam em `<marca>/google-ads-transparency/` (Liréa e Gentilia).

Composições por marca (`_composicoes/`): `imgs.png` (imagens da marca lado a lado) e `index.txt` (log de captura). Não pertencem a um único anúncio.

## Manifesto SHA-256 (por arquivo)

Caminhos relativos à raiz do repositório. Data da coleta de todos: 2026-11-17.

### Liréa — FR / francês

| ID do anúncio | Arquivo | Conteúdo | SHA-256 |
|---|---|---|---|
| `1012844728266644` | `evidence-local/canela-ceilao-2026-11-17/lirea/1012844728266644/1012844728266644_card.txt` | texto do card (copy, datas, headline, CTA) | `627959cf41245bef2d8f2bab18b61af216919a1285e1b80b9f40ace1771430cb` |
| `1012844728266644` | `evidence-local/canela-ceilao-2026-11-17/lirea/1012844728266644/1012844728266644_f00000.0.png` | quadro do vídeo em 0 s | `700ad2d662347fbfda013c20807e6306115100588baf28918323d5de4aff950a` |
| `1012844728266644` | `evidence-local/canela-ceilao-2026-11-17/lirea/1012844728266644/1012844728266644_f00001.0.png` | quadro do vídeo em 1 s | `e237dfd7265d47ba960196d22c97e791cafcff8364a8c2f77020d5724b49880a` |
| `1012844728266644` | `evidence-local/canela-ceilao-2026-11-17/lirea/1012844728266644/1012844728266644_f00002.0.png` | quadro do vídeo em 2 s | `8095826b5fe52eaaee4f0afc533e33a285f8c62b0627a86061ce5560c2c24704` |
| `1012844728266644` | `evidence-local/canela-ceilao-2026-11-17/lirea/1012844728266644/1012844728266644_f00003.0.png` | quadro do vídeo em 3 s | `ed77baea1188f7cd05bbf3662b49f110af06d409370d09dd77473340c278f369` |
| `1012844728266644` | `evidence-local/canela-ceilao-2026-11-17/lirea/1012844728266644/1012844728266644_f00004.3.png` | quadro do vídeo em 4.3 s | `363dc50d68ca48ce27cdb063b0c59a5c2f07a99ea3bb8fe37f7da9b0233d3e98` |
| `1012844728266644` | `evidence-local/canela-ceilao-2026-11-17/lirea/1012844728266644/1012844728266644_f00005.0.png` | quadro do vídeo em 5 s | `3e2300cf1800220e07e189df02ae4ae7c0e4c7602418d2821b79ee37ab78b50d` |
| `1012844728266644` | `evidence-local/canela-ceilao-2026-11-17/lirea/1012844728266644/1012844728266644_f00008.0.png` | quadro do vídeo em 8 s | `bdca7a8318ffb7efe0dd5d4c6906d40341cf0e4d026169e41cdd5173685e1573` |
| `1012844728266644` | `evidence-local/canela-ceilao-2026-11-17/lirea/1012844728266644/1012844728266644_f00008.7.png` | quadro do vídeo em 8.7 s | `9bc783ec8b4d1f415cceba60383af888ea7f1b583e919720f600dd7c8b1d4895` |
| `1012844728266644` | `evidence-local/canela-ceilao-2026-11-17/lirea/1012844728266644/1012844728266644_f00013.0.png` | quadro do vídeo em 13 s | `bbdd19a2505a9ef4a2eecce74457cd460bb313ba9d3e529f4f39f1a6c7fbc1a3` |
| `1012844728266644` | `evidence-local/canela-ceilao-2026-11-17/lirea/1012844728266644/1012844728266644_f00015.0.png` | quadro do vídeo em 15 s | `f91d62bba38dd8d67283655e644a405bf90671300ba4d56ac5188299506f549e` |
| `1012844728266644` | `evidence-local/canela-ceilao-2026-11-17/lirea/1012844728266644/1012844728266644_f00015.4.png` | quadro do vídeo em 15.4 s | `23282b34b38f6066b8fb5e9ecc6bfdfcf90f0a4b4d266cdb2d051c1647d50a4c` |
| `1012844728266644` | `evidence-local/canela-ceilao-2026-11-17/lirea/1012844728266644/sheet_1012844728266644.png` | prancha de quadros / captura do card | `13466f3ddc4a151a1e02b46716deb2bcd5790b0ffba215dd63f1aabf07692908` |
| `1134782529421301` | `evidence-local/canela-ceilao-2026-11-17/lirea/1134782529421301/1134782529421301_card.txt` | texto do card (copy, datas, headline, CTA) | `fdd95a38c7a2acb8a92675e7e2ac4d1f94c1a78af399dc1f4524e830e93ae26c` |
| `1134782529421301` | `evidence-local/canela-ceilao-2026-11-17/lirea/1134782529421301/1134782529421301_f00000.0.png` | quadro do vídeo em 0 s | `99df81b11883f653c5d6b7598f570e8293b30e4162e43197c3180583f9381783` |
| `1134782529421301` | `evidence-local/canela-ceilao-2026-11-17/lirea/1134782529421301/1134782529421301_f00001.0.png` | quadro do vídeo em 1 s | `29ad59693f0180e97f067357c7dc59d79276f5ad4e9359c4785950458e6c02c8` |
| `1134782529421301` | `evidence-local/canela-ceilao-2026-11-17/lirea/1134782529421301/1134782529421301_f00002.0.png` | quadro do vídeo em 2 s | `8bb6fe7e3cf6077bec588ebf345f4d366ca71eb2b9d4cf865a8fc1012e3086a0` |
| `1134782529421301` | `evidence-local/canela-ceilao-2026-11-17/lirea/1134782529421301/1134782529421301_f00003.0.png` | quadro do vídeo em 3 s | `2e78bee0cf47604f4ad5e75efc95335056ae95acf15d0950a711ddd8cbce44d8` |
| `1134782529421301` | `evidence-local/canela-ceilao-2026-11-17/lirea/1134782529421301/1134782529421301_f00005.0.png` | quadro do vídeo em 5 s | `497038888fd603f044c3c5ed83bbf2cd1fcd013133a7c04a43c1fe4b15735056` |
| `1134782529421301` | `evidence-local/canela-ceilao-2026-11-17/lirea/1134782529421301/1134782529421301_f00008.0.png` | quadro do vídeo em 8 s | `91c9a22dcae68c5af359cc250620e697227139ed027ed9a7014a5dcc4d9b135a` |
| `1134782529421301` | `evidence-local/canela-ceilao-2026-11-17/lirea/1134782529421301/1134782529421301_f00015.0.png` | quadro do vídeo em 15 s | `fc1a1faeecb65171a994282ca0429fc288dcef0b9afbf3552df8818fcd0c64d8` |
| `1134782529421301` | `evidence-local/canela-ceilao-2026-11-17/lirea/1134782529421301/1134782529421301_f00064.0.png` | quadro do vídeo em 64 s | `1a902569aceda239e73cd7c5d956e2149a7d2de5d6f0c58bfbb59a81b6fd7057` |
| `1134782529421301` | `evidence-local/canela-ceilao-2026-11-17/lirea/1134782529421301/1134782529421301_f00128.1.png` | quadro do vídeo em 128.1 s | `5013f6eaaf5afba0d6212f3b8294cc1cde370f88aae2c219e043f4b491469faf` |
| `1134782529421301` | `evidence-local/canela-ceilao-2026-11-17/lirea/1134782529421301/1134782529421301_f00192.1.png` | quadro do vídeo em 192.1 s | `3e89687281ea98909a94fd099f21e0b8f905c3dbf0058db7fb1d1b988184c1f3` |
| `1134782529421301` | `evidence-local/canela-ceilao-2026-11-17/lirea/1134782529421301/1134782529421301_f00254.1.png` | quadro do vídeo em 254.1 s | `bd029b35be409c25b6dd3e5b012997aafdb039eaf3143ba1f679f21cce5ee264` |
| `1134782529421301` | `evidence-local/canela-ceilao-2026-11-17/lirea/1134782529421301/sheet_1134782529421301.png` | prancha de quadros / captura do card | `8d447418f5268c49f59fd4bab4a10627a23b30a9666abfc471bb7f0838398859` |
| `1508654571040358` | `evidence-local/canela-ceilao-2026-11-17/lirea/1508654571040358/1508654571040358_card.txt` | texto do card (copy, datas, headline, CTA) | `40d97ed4cd499b6eac8c2005fe7fe359d1ce178c1b6ed3bd7d8631fe22164045` |
| `1508654571040358` | `evidence-local/canela-ceilao-2026-11-17/lirea/1508654571040358/sheet_1508654571040358.png` | prancha de quadros / captura do card | `9aaf3c0fa33eb52d068de7caa54a5b7dc5c053cafb8d0212fb014860797452eb` |
| `1737759380776286` | `evidence-local/canela-ceilao-2026-11-17/lirea/1737759380776286/1737759380776286_card.txt` | texto do card (copy, datas, headline, CTA) | `88f42e85daafd9a61c1d2dc8b08a6d25feaa39fb4110e20c330240983a523daa` |
| `1737759380776286` | `evidence-local/canela-ceilao-2026-11-17/lirea/1737759380776286/sheet_1737759380776286.png` | prancha de quadros / captura do card | `2f5325a387a58e7570008a71fc8b571e9c0ade4f8fec3406016265b2249e982d` |
| `1952463358756102` | `evidence-local/canela-ceilao-2026-11-17/lirea/1952463358756102/1952463358756102_card.txt` | texto do card (copy, datas, headline, CTA) | `e16e5f1e66699b6fad28ec539cfef21c426644f063901ca3a025beed6567c69a` |
| `1952463358756102` | `evidence-local/canela-ceilao-2026-11-17/lirea/1952463358756102/1952463358756102_f00000.0.png` | quadro do vídeo em 0 s | `537311c443c4b6106082b70a650abb400f733a45efdbaff854b2e3d3038d82e2` |
| `1952463358756102` | `evidence-local/canela-ceilao-2026-11-17/lirea/1952463358756102/1952463358756102_f00001.0.png` | quadro do vídeo em 1 s | `e141198018c3205b31d4b47cb00ddd4bab59fdf8a59be186c1d7690d52d9a042` |
| `1952463358756102` | `evidence-local/canela-ceilao-2026-11-17/lirea/1952463358756102/1952463358756102_f00002.0.png` | quadro do vídeo em 2 s | `2c169acf0820415f7eba370de5e3e0a584e01f45976f35c841fbf827b7a59cbe` |
| `1952463358756102` | `evidence-local/canela-ceilao-2026-11-17/lirea/1952463358756102/1952463358756102_f00003.0.png` | quadro do vídeo em 3 s | `98d5ccba6f5714da77a72f85322c38f8d8e45a00d816429219ff42beb5b816e8` |
| `1952463358756102` | `evidence-local/canela-ceilao-2026-11-17/lirea/1952463358756102/1952463358756102_f00005.0.png` | quadro do vídeo em 5 s | `e3118111a9ab8a28ffb3ade52ed40e7d22ee08e9eea13da4528515d25cf94947` |
| `1952463358756102` | `evidence-local/canela-ceilao-2026-11-17/lirea/1952463358756102/1952463358756102_f00008.0.png` | quadro do vídeo em 8 s | `a92d0d3ba4bd108bb72affd2a25da81a79d735870b11de117fc45007a545b05b` |
| `1952463358756102` | `evidence-local/canela-ceilao-2026-11-17/lirea/1952463358756102/1952463358756102_f00015.0.png` | quadro do vídeo em 15 s | `5cfc0ef542ebff09895238af38db32a6ce0011eb0f63628f6da3abf5fac9561c` |
| `1952463358756102` | `evidence-local/canela-ceilao-2026-11-17/lirea/1952463358756102/1952463358756102_f00023.8.png` | quadro do vídeo em 23.8 s | `7b0a6306a7000cb3a5fb7d90a0a3f5870cc448c4e3522eb39344f40508191592` |
| `1952463358756102` | `evidence-local/canela-ceilao-2026-11-17/lirea/1952463358756102/1952463358756102_f00047.5.png` | quadro do vídeo em 47.5 s | `09c2770b1fd240c6df6719264d7316237c98ed740d181799ccb13bcb30b40170` |
| `1952463358756102` | `evidence-local/canela-ceilao-2026-11-17/lirea/1952463358756102/1952463358756102_f00071.3.png` | quadro do vídeo em 71.3 s | `4344936825db0f0a2a76495fec43153afcafde592a472891d7e4df49141bf0df` |
| `1952463358756102` | `evidence-local/canela-ceilao-2026-11-17/lirea/1952463358756102/1952463358756102_f00093.1.png` | quadro do vídeo em 93.1 s | `084e913012beb22aabab39b96ea35d9b589af3707960afcf512e8e23179ff631` |
| `1952463358756102` | `evidence-local/canela-ceilao-2026-11-17/lirea/1952463358756102/sheet_1952463358756102.png` | prancha de quadros / captura do card | `f4684b052c5722f3d0781408391d1f225c074917792deb5cb0a7ae3be5f63cf9` |
| `2119393105350095` | `evidence-local/canela-ceilao-2026-11-17/lirea/2119393105350095/2119393105350095_card.txt` | texto do card (copy, datas, headline, CTA) | `ff7eb010664901c36932291597fce05369bb303afe8ff7d1a7ccdc7e2d4f845a` |
| `2119393105350095` | `evidence-local/canela-ceilao-2026-11-17/lirea/2119393105350095/sheet_2119393105350095.png` | prancha de quadros / captura do card | `7802009c9c052866cc8f3831873b341601219191160a0dd7c2c753234284107b` |
| `2183910109197467` | `evidence-local/canela-ceilao-2026-11-17/lirea/2183910109197467/2183910109197467_t0000,0.png` | quadro do vídeo em 0 s | `bb361a3ff0bec5339c1e7ec322ae87e28bcf39ab3cd23e9366f25614110cceb3` |
| `2183910109197467` | `evidence-local/canela-ceilao-2026-11-17/lirea/2183910109197467/2183910109197467_t0001,0.png` | quadro do vídeo em 1 s | `fe3764c0b0ae7c6b940e3775605c865fe19e2ddf9e5b7e5f954a137814525ce4` |
| `2183910109197467` | `evidence-local/canela-ceilao-2026-11-17/lirea/2183910109197467/2183910109197467_t0002,0.png` | quadro do vídeo em 2 s | `9fa1961a04bd86f7a1086538ec28a2e986785273d3b454ab1242edc5a3e39098` |
| `2183910109197467` | `evidence-local/canela-ceilao-2026-11-17/lirea/2183910109197467/2183910109197467_t0003,0.png` | quadro do vídeo em 3 s | `2c7e637019be38695109f2965c056dbdfdc21c6bdf1871c107e7d1927e80931c` |
| `2183910109197467` | `evidence-local/canela-ceilao-2026-11-17/lirea/2183910109197467/2183910109197467_t0005,0.png` | quadro do vídeo em 5 s | `c6f644af7a3194b2057e3f07fd8aaa139edbde6b31c07d5e51442b2b9e0baa79` |
| `2183910109197467` | `evidence-local/canela-ceilao-2026-11-17/lirea/2183910109197467/2183910109197467_t0008,0.png` | quadro do vídeo em 8 s | `e24a3f97793b744953f5a60ef3847e77a2ce3d7cabf81166f874f57cbeafcd5e` |
| `2183910109197467` | `evidence-local/canela-ceilao-2026-11-17/lirea/2183910109197467/2183910109197467_t0012,0.png` | quadro do vídeo em 12 s | `37910d5fa92191386f6ac8ebfad6ed0dd55304979a7debcb12cf53e18fb1dd32` |
| `2183910109197467` | `evidence-local/canela-ceilao-2026-11-17/lirea/2183910109197467/2183910109197467_t0020,0.png` | quadro do vídeo em 20 s | `a2a29ee07fbaa42d33c032be36ff95d397c96b035fa32731a39429f6b82ba130` |
| `2183910109197467` | `evidence-local/canela-ceilao-2026-11-17/lirea/2183910109197467/2183910109197467_t0040,0.png` | quadro do vídeo em 40 s | `23dd5a05fa78e9e0f22c80154c78042b0276ce3cc0687e3d826f56f411496cdf` |
| `2183910109197467` | `evidence-local/canela-ceilao-2026-11-17/lirea/2183910109197467/2183910109197467_t0090,0.png` | quadro do vídeo em 90 s | `206b00e8ba5d1fe94c9b7c35110453d3a05e8768e29215aa29df7cfcbff54cfe` |
| `2183910109197467` | `evidence-local/canela-ceilao-2026-11-17/lirea/2183910109197467/2183910109197467_t0180,0.png` | quadro do vídeo em 180 s | `d79b733983f1a90894dd4e230e3efee347c6fb0afc7fdd9aea4323ae91072546` |
| `2183910109197467` | `evidence-local/canela-ceilao-2026-11-17/lirea/2183910109197467/2183910109197467_t0270,0.png` | quadro do vídeo em 270 s | `fd43f54dd372905f02a69112b1e0060b1a0db05ab9f9e0b7fbdf2e9de4e26307` |
| `2183910109197467` | `evidence-local/canela-ceilao-2026-11-17/lirea/2183910109197467/2183910109197467_t0300,0.png` | quadro do vídeo em 300 s | `a305ee49da3e9adba23427892f1882361608862da9cb454ab5c0fee5741ed34d` |
| `2183910109197467` | `evidence-local/canela-ceilao-2026-11-17/lirea/2183910109197467/95f34f70-617c-49e6-88c4-9e064347cdc3-screenshot.png` | captura de tela do card (modal "Link para o anúncio") | `92c52e29a2180dd39ec2668bc1c7798c3cae5e3701d934fc59e0d59fd4279e9c` |
| `2183910109197467` | `evidence-local/canela-ceilao-2026-11-17/lirea/2183910109197467/contact_2183910109197467.png` | prancha de quadros (montagem) | `90e7b1d15f8be23b5fcde34b1220e674a371fa2b65ce6aa8a6ac2db6dd610aed` |
| `2253175732202903` | `evidence-local/canela-ceilao-2026-11-17/lirea/2253175732202903/2253175732202903_card.txt` | texto do card (copy, datas, headline, CTA) | `1cd4d52440624002a86005c4db7fee26b09402974cb3dd19411e5a44d9098dcc` |
| `2253175732202903` | `evidence-local/canela-ceilao-2026-11-17/lirea/2253175732202903/2253175732202903_f00000.0.png` | quadro do vídeo em 0 s | `4ac2bd7051428a89aca5974e180f8cdfec98b4f606148eccc8701a071b5d2d47` |
| `2253175732202903` | `evidence-local/canela-ceilao-2026-11-17/lirea/2253175732202903/2253175732202903_f00001.0.png` | quadro do vídeo em 1 s | `7b92eaf4b5cb8b227cfaa71a018e1c5d54eee124661d5c8cb57e29f08f19f37d` |
| `2253175732202903` | `evidence-local/canela-ceilao-2026-11-17/lirea/2253175732202903/2253175732202903_f00002.0.png` | quadro do vídeo em 2 s | `df7c8f360075c77fb8ee2bfdf547532c082cc5bf8e926d10ad476fd494b97f23` |
| `2253175732202903` | `evidence-local/canela-ceilao-2026-11-17/lirea/2253175732202903/2253175732202903_f00003.0.png` | quadro do vídeo em 3 s | `5af740b4614523f38dbe83e6b10f3c4a82276cd2346a0f816e19e0148236f009` |
| `2253175732202903` | `evidence-local/canela-ceilao-2026-11-17/lirea/2253175732202903/2253175732202903_f00005.0.png` | quadro do vídeo em 5 s | `fbae6586bcd0efa4262710b6a711fe5d882f651f706fdf460f1b1a60a7ec800b` |
| `2253175732202903` | `evidence-local/canela-ceilao-2026-11-17/lirea/2253175732202903/2253175732202903_f00008.0.png` | quadro do vídeo em 8 s | `a15bc00798aeee551a28ed711ce612b993a816abcec8dfdff7695edea5c478bd` |
| `2253175732202903` | `evidence-local/canela-ceilao-2026-11-17/lirea/2253175732202903/2253175732202903_f00015.0.png` | quadro do vídeo em 15 s | `eaec25ace63b6fe7ecca1d612d4ee8d84974c814c8d1f6b715c6645dfac4cf0a` |
| `2253175732202903` | `evidence-local/canela-ceilao-2026-11-17/lirea/2253175732202903/2253175732202903_f00021.9.png` | quadro do vídeo em 21.9 s | `9f1638202dfd31a444a42d555af6722fc7e2d14f93497e4404cf3c8907379ac7` |
| `2253175732202903` | `evidence-local/canela-ceilao-2026-11-17/lirea/2253175732202903/2253175732202903_f00043.8.png` | quadro do vídeo em 43.8 s | `26ba1d9f21a0bb87d82373ebd849ad37d8df51009e17969e557ed30f113c34c1` |
| `2253175732202903` | `evidence-local/canela-ceilao-2026-11-17/lirea/2253175732202903/2253175732202903_f00065.7.png` | quadro do vídeo em 65.7 s | `6f594834ccfd1126c720581f91e767b0f85959775b39c309240a0e1ba0725f2d` |
| `2253175732202903` | `evidence-local/canela-ceilao-2026-11-17/lirea/2253175732202903/2253175732202903_f00085.7.png` | quadro do vídeo em 85.7 s | `7d7272f21062c4381f4f13b44f4f56201cca6fb1c14a4c962538db52731ba4f4` |
| `2253175732202903` | `evidence-local/canela-ceilao-2026-11-17/lirea/2253175732202903/sheet_2253175732202903.png` | prancha de quadros / captura do card | `9aa72e1058d281ba7ebeb7fa745e7735523fd88b0aa12ec1d9a79630aa6b1191` |
| `984263778060761` | `evidence-local/canela-ceilao-2026-11-17/lirea/984263778060761/984263778060761_card.txt` | texto do card (copy, datas, headline, CTA) | `cdc1acafd4f3f88acc812b89270925cb60a8eff8a375e784432ef9666fe6952c` |
| `984263778060761` | `evidence-local/canela-ceilao-2026-11-17/lirea/984263778060761/984263778060761_f00000.0.png` | quadro do vídeo em 0 s | `b920f97a7e27ba5747a63bcc10c76efdff4741b330427a6ec4cddf5b5aa49ebb` |
| `984263778060761` | `evidence-local/canela-ceilao-2026-11-17/lirea/984263778060761/984263778060761_f00001.0.png` | quadro do vídeo em 1 s | `95323d57bc7cf3b6f0dda44d61a4fbed2f899b58932d704d32ed86bc3724afc1` |
| `984263778060761` | `evidence-local/canela-ceilao-2026-11-17/lirea/984263778060761/984263778060761_f00002.0.png` | quadro do vídeo em 2 s | `c2b4b6d545d91fed473b0d9ed018c7c59877577e102fd8e05ee5e37cb406d93e` |
| `984263778060761` | `evidence-local/canela-ceilao-2026-11-17/lirea/984263778060761/984263778060761_f00003.0.png` | quadro do vídeo em 3 s | `2735a4d5be8d286d99af02c4d600023b87f80a5e541cedb83b1ae5221690c5ac` |
| `984263778060761` | `evidence-local/canela-ceilao-2026-11-17/lirea/984263778060761/984263778060761_f00005.0.png` | quadro do vídeo em 5 s | `660a95b4e2ed5da77f13f0ef2e84c3370add8d8c4b26625e83cabda7fe98b710` |
| `984263778060761` | `evidence-local/canela-ceilao-2026-11-17/lirea/984263778060761/984263778060761_f00008.0.png` | quadro do vídeo em 8 s | `16aef625d54f6564c55e92c4b5842fa055db2901d20c785f4019012b7c1aac6c` |
| `984263778060761` | `evidence-local/canela-ceilao-2026-11-17/lirea/984263778060761/984263778060761_f00015.0.png` | quadro do vídeo em 15 s | `f982f4edb8f53477261fbe8fb2ec8f699a4e762e54559434e8fcc8314c3df22e` |
| `984263778060761` | `evidence-local/canela-ceilao-2026-11-17/lirea/984263778060761/984263778060761_f00016.5.png` | quadro do vídeo em 16.5 s | `13e9b6f5d8a6064ca58e9567c616f0f340392e268cc39c5b110474109199474b` |
| `984263778060761` | `evidence-local/canela-ceilao-2026-11-17/lirea/984263778060761/984263778060761_f00032.9.png` | quadro do vídeo em 32.9 s | `7d811d1076c577aa30ee432b84ae3cf16d12f657fefbd5e2888d419fbd927e91` |
| `984263778060761` | `evidence-local/canela-ceilao-2026-11-17/lirea/984263778060761/984263778060761_f00049.4.png` | quadro do vídeo em 49.4 s | `dd40a6515b55fc5c22a8415a57c3eaa509ac7d2a60b67f436de1eca5d8939139` |
| `984263778060761` | `evidence-local/canela-ceilao-2026-11-17/lirea/984263778060761/984263778060761_f00063.8.png` | quadro do vídeo em 63.8 s | `39773adb135f1e0fe5092299b2a33500fc2b70531acc509b79d69edd941aa721` |
| `984263778060761` | `evidence-local/canela-ceilao-2026-11-17/lirea/984263778060761/sheet_984263778060761.png` | prancha de quadros / captura do card | `9ee39ecc6f802af7aa487dd2ff5b44461eaa6705145c8735648e5af8c72b8a15` |
| — | `evidence-local/canela-ceilao-2026-11-17/lirea/_composicoes/imgs.png` | montagem lado a lado das imagens da marca | `d77d4db37427de95981c9211997f528712ec670e97031bae74af2ff932549d26` |
| — | `evidence-local/canela-ceilao-2026-11-17/lirea/_composicoes/index.txt` | log de captura (ID, tipo, duração, resolução) | `f1a60c1739b222033bc162a9c1ab8fb9af8f430de224476e0aab3480b08d0dde` |
| — | `evidence-local/canela-ceilao-2026-11-17/lirea/google-ads-transparency/google_lireaofficiel.com.png` | Google Ads Transparency, domínio lireaofficiel.com (6 anúncios, ACH Group) — https://adstransparency.google.com/?region=anywhere&domain=lireaofficiel.com | `91f58ecb4f05a7dfcb438a680192c3bdb8ffd65b9636da8549e3783eb2193be2` |

### Gentilia — IT / italiano

| ID do anúncio | Arquivo | Conteúdo | SHA-256 |
|---|---|---|---|
| `1080649297659813` | `evidence-local/canela-ceilao-2026-11-17/gentilia/1080649297659813/1080649297659813_card.txt` | texto do card (copy, datas, headline, CTA) | `22aa8d8ea8f1c06337f54b81c3a8e5667601714a02f18d799acef4d8750f30b2` |
| `1080649297659813` | `evidence-local/canela-ceilao-2026-11-17/gentilia/1080649297659813/sheet_1080649297659813.png` | prancha de quadros / captura do card | `2e7c3a1dfbe776786e0a9d74f821a8c14237cfd609d0a995979105139babf004` |
| `1612780430444542` | `evidence-local/canela-ceilao-2026-11-17/gentilia/1612780430444542/1612780430444542_card.txt` | texto do card (copy, datas, headline, CTA) | `eb93105b5700db40975e747c56f58fc95a94d4db0ad05ca0e9ad08e1d9dfc798` |
| `1612780430444542` | `evidence-local/canela-ceilao-2026-11-17/gentilia/1612780430444542/sheet_1612780430444542.png` | prancha de quadros / captura do card | `7acedee661b21e80c31327b85b92ccf520037b8737851b457fc13ad3e5c5426d` |
| `2253085015543875` | `evidence-local/canela-ceilao-2026-11-17/gentilia/2253085015543875/2253085015543875_card.txt` | texto do card (copy, datas, headline, CTA) | `47793e3cb73756b0f62c406019253ec2ea94a08708e7a7fccef9429fb54524c4` |
| `2253085015543875` | `evidence-local/canela-ceilao-2026-11-17/gentilia/2253085015543875/sheet_2253085015543875.png` | prancha de quadros / captura do card | `2744b6ccfb9993bd5987e16e6c962ae630145c1bd56380d3e00a1337d9e2f38d` |
| `2346016919563069` | `evidence-local/canela-ceilao-2026-11-17/gentilia/2346016919563069/2346016919563069_card.txt` | texto do card (copy, datas, headline, CTA) | `36a7864553a153c4e44341853f848e73b8c68404012ab7dec0c623274a58d30d` |
| `2346016919563069` | `evidence-local/canela-ceilao-2026-11-17/gentilia/2346016919563069/sheet_2346016919563069.png` | prancha de quadros / captura do card | `26c63a889e201ee6f3d45c4a645406636c58c191560fcab2072de7d55587bf49` |
| `2510128156144033` | `evidence-local/canela-ceilao-2026-11-17/gentilia/2510128156144033/2510128156144033_card.txt` | texto do card (copy, datas, headline, CTA) | `13dd370c4c5c0f533ba1bc79626db4d150de406b01001793645e52ff39ea326b` |
| `2510128156144033` | `evidence-local/canela-ceilao-2026-11-17/gentilia/2510128156144033/sheet_2510128156144033.png` | prancha de quadros / captura do card | `4a44066ab6dc85120f53e07da7c4c89d7956e3d0ebd279ac0f3394edbbfea50e` |
| — | `evidence-local/canela-ceilao-2026-11-17/gentilia/_composicoes/imgs.png` | montagem lado a lado das imagens da marca | `4b8f47375d449bc7262b76e585830cd7256cae72f978deae019ebdd4b1c7031d` |
| — | `evidence-local/canela-ceilao-2026-11-17/gentilia/_composicoes/index.txt` | log de captura (ID, tipo, duração, resolução) | `743969dc3fb1ee05cd7f2c9a195a8ca5a709d82d216b2afb6e056e6450365175` |
| — | `evidence-local/canela-ceilao-2026-11-17/gentilia/google-ads-transparency/google_gentilia.it.png` | Google Ads Transparency, domínio gentilia.it (1 anúncio, ERCOWISE LLC) — https://adstransparency.google.com/?region=anywhere&domain=gentilia.it | `223d1923ef7cbcf4fb9ac2d4093edb6f3e9c96805eefd6aa02a290d3cde0f40a` |

### 健然堂 Kenzendo — JP / japonês

| ID do anúncio | Arquivo | Conteúdo | SHA-256 |
|---|---|---|---|
| `1140487985356612` | `evidence-local/canela-ceilao-2026-11-17/kenzendo/1140487985356612/1140487985356612_card.txt` | texto do card (copy, datas, headline, CTA) | `1b8b36fdc8d34dcc770a162d09e5faff61574c908b3e03928a6d34dab37799df` |
| `1140487985356612` | `evidence-local/canela-ceilao-2026-11-17/kenzendo/1140487985356612/1140487985356612_f00000.0.png` | quadro do vídeo em 0 s | `e8757e772376f2d266e0fab4c19dd10b111280f5b882517b2e0ccf22967bdac6` |
| `1140487985356612` | `evidence-local/canela-ceilao-2026-11-17/kenzendo/1140487985356612/1140487985356612_f00001.0.png` | quadro do vídeo em 1 s | `d09424449831d8d09821af40e2918a78deda86f379c52a1eb36045452e35084e` |
| `1140487985356612` | `evidence-local/canela-ceilao-2026-11-17/kenzendo/1140487985356612/1140487985356612_f00002.0.png` | quadro do vídeo em 2 s | `2810db5a4681d09223aa22a85898d165f658520c69309d588e9f98dae5ce04d6` |
| `1140487985356612` | `evidence-local/canela-ceilao-2026-11-17/kenzendo/1140487985356612/1140487985356612_f00003.0.png` | quadro do vídeo em 3 s | `cb2ce4136ca5da8f55fe0d15f5ba541ee9e76e80c6b2bbc1e3659f94a53182de` |
| `1140487985356612` | `evidence-local/canela-ceilao-2026-11-17/kenzendo/1140487985356612/1140487985356612_f00005.0.png` | quadro do vídeo em 5 s | `2f1059eedec777598b06d6d5f73c57982dfd8d633306ba86a1833721774091b5` |
| `1140487985356612` | `evidence-local/canela-ceilao-2026-11-17/kenzendo/1140487985356612/1140487985356612_f00008.0.png` | quadro do vídeo em 8 s | `cb5d15c3584c1717e2cc413899591c74bc9231bf214858f3323681f043113adc` |
| `1140487985356612` | `evidence-local/canela-ceilao-2026-11-17/kenzendo/1140487985356612/1140487985356612_f00015.0.png` | quadro do vídeo em 15 s | `8f64f71a47f495748321c644985eecd0105ff9a3dc564c35b46b4edcb27e5f81` |
| `1140487985356612` | `evidence-local/canela-ceilao-2026-11-17/kenzendo/1140487985356612/1140487985356612_f00051.6.png` | quadro do vídeo em 51.6 s | `2c59825fe9487c75c9879981934c5cb2c5d3cc6de7e4e0ae34e2f4559d8119db` |
| `1140487985356612` | `evidence-local/canela-ceilao-2026-11-17/kenzendo/1140487985356612/1140487985356612_f00103.1.png` | quadro do vídeo em 103.1 s | `6c69ffdb57390ae3070c33b564885b4c028754319ea631f3e99b5a9af74fd86d` |
| `1140487985356612` | `evidence-local/canela-ceilao-2026-11-17/kenzendo/1140487985356612/1140487985356612_f00154.7.png` | quadro do vídeo em 154.7 s | `74ec9a9125e03f1625acd6e9e7ffb71184a7e920ace2bce43440be58f7d55ab6` |
| `1140487985356612` | `evidence-local/canela-ceilao-2026-11-17/kenzendo/1140487985356612/1140487985356612_f00204.3.png` | quadro do vídeo em 204.3 s | `658fdfd08666139d69d0851b18ba156cc42b95117ac2e407eb4d3299d0367fcf` |
| `1140487985356612` | `evidence-local/canela-ceilao-2026-11-17/kenzendo/1140487985356612/sheet_1140487985356612.png` | prancha de quadros / captura do card | `502e8056295e0ec4aa17070f6fe082ede9926cde786fbbc903ca14a965b379d0` |
| `1141597035190365` | `evidence-local/canela-ceilao-2026-11-17/kenzendo/1141597035190365/1141597035190365_card.txt` | texto do card (copy, datas, headline, CTA) | `079802e33620cd00172cd2734cfecfc3b33d4baad143db3dbd914832520d43ca` |
| `1141597035190365` | `evidence-local/canela-ceilao-2026-11-17/kenzendo/1141597035190365/sheet_1141597035190365.png` | prancha de quadros / captura do card | `1fa0b9badc9c44bad356cdbe3aaa3273dd4994070c69f51e8d37b6a35812c432` |
| `1431133619130686` | `evidence-local/canela-ceilao-2026-11-17/kenzendo/1431133619130686/1431133619130686_card.txt` | texto do card (copy, datas, headline, CTA) | `a29af666bfeae9f326b759b2d0025321ff0b9c9d87dc5e4e6c59d68293e76e34` |
| `1431133619130686` | `evidence-local/canela-ceilao-2026-11-17/kenzendo/1431133619130686/sheet_1431133619130686.png` | prancha de quadros / captura do card | `0d4aa3658b56e6d63781a57bfe8195fca6d111ec4877160ade07f823a80aa9d7` |
| `1483725747247937` | `evidence-local/canela-ceilao-2026-11-17/kenzendo/1483725747247937/1483725747247937_card.txt` | texto do card (copy, datas, headline, CTA) | `fa61b1e247cdb0d49436ad0a9d3f56a4f9e7149d04eb3318df8426b23d068bcb` |
| `1483725747247937` | `evidence-local/canela-ceilao-2026-11-17/kenzendo/1483725747247937/1483725747247937_f00000.0.png` | quadro do vídeo em 0 s | `c0b26901de82741bfce8a8a9c2e3521707e60bceff2073b1cf2588ea18a889b3` |
| `1483725747247937` | `evidence-local/canela-ceilao-2026-11-17/kenzendo/1483725747247937/1483725747247937_f00001.0.png` | quadro do vídeo em 1 s | `ef90b26a6d5f9970859dec39f7d7f6b891eb193961e13bbc10910129cdf2a1f5` |
| `1483725747247937` | `evidence-local/canela-ceilao-2026-11-17/kenzendo/1483725747247937/1483725747247937_f00001.9.png` | quadro do vídeo em 1.9 s | `f912ee31b35fbf92619ed179a560b820eff1d74a995d2392d7e97cd74c69584a` |
| `1483725747247937` | `evidence-local/canela-ceilao-2026-11-17/kenzendo/1483725747247937/1483725747247937_f00002.0.png` | quadro do vídeo em 2 s | `b7cd8a74191823068f084a91d1802e2961a599c3c946372bebf7fd245e398195` |
| `1483725747247937` | `evidence-local/canela-ceilao-2026-11-17/kenzendo/1483725747247937/1483725747247937_f00003.0.png` | quadro do vídeo em 3 s | `54da1a6a2ad1036eb1783896ec5bd1587ca9716430b50c7b6ef1ecd6dca8c3cf` |
| `1483725747247937` | `evidence-local/canela-ceilao-2026-11-17/kenzendo/1483725747247937/1483725747247937_f00003.8.png` | quadro do vídeo em 3.8 s | `6f8d7dfc382abf044a86a0283785c72eb0168a809c7a641b9a3c59a8ea3c0b8b` |
| `1483725747247937` | `evidence-local/canela-ceilao-2026-11-17/kenzendo/1483725747247937/1483725747247937_f00005.0.png` | quadro do vídeo em 5 s | `2dc28dec2740589c42047a3d0aede7f45e8f9e1c64067342fd34c6d9c43783d4` |
| `1483725747247937` | `evidence-local/canela-ceilao-2026-11-17/kenzendo/1483725747247937/1483725747247937_f00005.5.png` | quadro do vídeo em 5.5 s | `46957994121b2c8fea1545ed2da0d398214f91d809086e465cdd992302a894a1` |
| `1483725747247937` | `evidence-local/canela-ceilao-2026-11-17/kenzendo/1483725747247937/1483725747247937_f00005.6.png` | quadro do vídeo em 5.6 s | `f78db9895cf38bb2a91713193fd09ff64ef3a23754f34cd5f9f6a12649c98303` |
| `1483725747247937` | `evidence-local/canela-ceilao-2026-11-17/kenzendo/1483725747247937/1483725747247937_f00008.0.png` | quadro do vídeo em 8 s | `9dd7874129b11b35497f551c6f5162fc70889829a8463c3a26c48b3b5df80c3d` |
| `1483725747247937` | `evidence-local/canela-ceilao-2026-11-17/kenzendo/1483725747247937/1483725747247937_f00015.0.png` | quadro do vídeo em 15 s | `1aabd1d993ace67629727e21f23cd493b5137678f89ef9938a3a82eb90a4e751` |
| `1483725747247937` | `evidence-local/canela-ceilao-2026-11-17/kenzendo/1483725747247937/sheet_1483725747247937.png` | prancha de quadros / captura do card | `f81386c1e07a556a3e240a49f45aa5f57541c99cc06c8130dda851f8cbd38963` |
| `1863077484847834` | `evidence-local/canela-ceilao-2026-11-17/kenzendo/1863077484847834/1863077484847834_card.txt` | texto do card (copy, datas, headline, CTA) | `1410816f045268579aefbf663d58307aad3474744958ac0ce10385d3888e3f1c` |
| `1863077484847834` | `evidence-local/canela-ceilao-2026-11-17/kenzendo/1863077484847834/1863077484847834_f00000.0.png` | quadro do vídeo em 0 s | `193f87ddb3192557fbd27b88c8bb2de6616688529d74a78d6bc148ceb3ed54ca` |
| `1863077484847834` | `evidence-local/canela-ceilao-2026-11-17/kenzendo/1863077484847834/1863077484847834_f00001.0.png` | quadro do vídeo em 1 s | `32ecd788ec7109861fa5d717564b1696904ccb681d7e5aca588e7b71b9d34c94` |
| `1863077484847834` | `evidence-local/canela-ceilao-2026-11-17/kenzendo/1863077484847834/1863077484847834_f00002.0.png` | quadro do vídeo em 2 s | `ed5ecd5eedde6708d738ffbadf4f574724bbcf686a8d70aa81e1efe0778d3098` |
| `1863077484847834` | `evidence-local/canela-ceilao-2026-11-17/kenzendo/1863077484847834/1863077484847834_f00003.0.png` | quadro do vídeo em 3 s | `312c22cf9fe964cfea074483be4f4375aa1bd3c379a8ccea2ea015e209b71c13` |
| `1863077484847834` | `evidence-local/canela-ceilao-2026-11-17/kenzendo/1863077484847834/1863077484847834_f00005.0.png` | quadro do vídeo em 5 s | `76a4219da2ef65ea9d2775a1b7688fc018de9268d32691e1437f7cdbaf9d8fad` |
| `1863077484847834` | `evidence-local/canela-ceilao-2026-11-17/kenzendo/1863077484847834/1863077484847834_f00008.0.png` | quadro do vídeo em 8 s | `6d0ba90540526bfba77d1f1bf998cddce4ed16619adcde23bc2016473814d392` |
| `1863077484847834` | `evidence-local/canela-ceilao-2026-11-17/kenzendo/1863077484847834/1863077484847834_f00015.0.png` | quadro do vídeo em 15 s | `b44006c3d8c73f6ae2bbf5ddf468362924897d0bb170c3d2b63b049645a7f56e` |
| `1863077484847834` | `evidence-local/canela-ceilao-2026-11-17/kenzendo/1863077484847834/1863077484847834_f00149.0.png` | quadro do vídeo em 149 s | `2b02a1034b1e13746be90e551c15483559cb1186259f12332274824b55dcefcf` |
| `1863077484847834` | `evidence-local/canela-ceilao-2026-11-17/kenzendo/1863077484847834/1863077484847834_f00298.1.png` | quadro do vídeo em 298.1 s | `59916829da710235cb73188297a840ffde4488f838b310f8cb32f441c77e4b73` |
| `1863077484847834` | `evidence-local/canela-ceilao-2026-11-17/kenzendo/1863077484847834/1863077484847834_f00447.1.png` | quadro do vídeo em 447.1 s | `377650dd38eabc5629d4175648cc3e8bd4d4143e866daf39545b98db9f53ee1a` |
| `1863077484847834` | `evidence-local/canela-ceilao-2026-11-17/kenzendo/1863077484847834/1863077484847834_f00594.1.png` | quadro do vídeo em 594.1 s | `1811c0bd8bb2f038d0f5c64039cdf8982b5c58f8e5a8af741d08cd96abaa335e` |
| `1863077484847834` | `evidence-local/canela-ceilao-2026-11-17/kenzendo/1863077484847834/sheet_1863077484847834.png` | prancha de quadros / captura do card | `9e220b0dac243f5ec5dae4a7087d6090753e413c0e5fe25c41576d2400edd1f8` |
| — | `evidence-local/canela-ceilao-2026-11-17/kenzendo/_composicoes/imgs.png` | montagem lado a lado das imagens da marca | `a1871df6ca8e04ff5b23512a7ba0cd43647a4cec601f54ce344f1523d643cf72` |
| — | `evidence-local/canela-ceilao-2026-11-17/kenzendo/_composicoes/index.txt` | log de captura (ID, tipo, duração, resolução) | `8acc91d17d30ec499192b22e8de5829fa43a445787b428d09ce896090670c0d1` |

