---
name: offer-mining
description: Executa uma missão de mineração de ofertas com pesquisa internacional, fontes, análise, classificação e relatório versionável. Use quando o usuário pedir para minerar ou investigar ofertas.
---

# Processo de mineração

## Entrada

País(es) de venda, problema, mecanismos de interesse, idiomas (automáticos ou explícitos), plataformas, número-alvo e profundidade.

Defaults quando não informados: 1 país de venda ou alcance mundial se pedido; até 10 ofertas **com evidências**; até 30 consultas de pesquisa; até 2 ciclos de aprofundamento por candidato; sem execução recorrente.

## Passos

1. **Capacidades:** inventariar ferramentas reais de busca, navegação, fontes de anúncios e análise de vídeo. Anotar lacunas.
2. **Plano:** solicitar ao `research-planner` (se disponível) consultas por mercado e idioma. Ler `.claude/skills/multilingual-discovery/SKILL.md`.
3. **Busca inicial:** coletar candidatos com URL real e data de inspeção. Descartar menções vagas sem produto identificável.
4. **Expansão:** pesquisar marca, domínio, ingredientes, anunciantes, páginas de venda, criativos e concorrentes; registrar caminhos de descoberta.
5. **Investigação:** aprofundar a oferta com `offer-investigator` e, havendo material visual acessível, `creative-reference-analyst`.
6. **Auditoria:** aplicar `.claude/skills/evidence-validation/SKILL.md` e solicitar crítica ao `evidence-auditor` se disponível.
7. **Escrita:** gerar `results/YYYY-MM-DD_slug/report.md` e `offers.json` seguindo `templates/offer-report.md` e `templates/offers.schema.example.json`. Gravar missão, buscas e limitações. Não gravar dados inventados.

## Critérios de parada

Encerrar quando: orçamento atingido; candidatos adequados suficientes; duas rodadas sem novos candidatos úteis; fontes inacessíveis; ou não houver evidência mínima. Explicar o motivo. Não preencher vagas com conteúdo especulativo.

## Forma de resposta

Resumo em português, lista das ofertas mais interessantes com fontes, classificação e nível de confiança, alertas e caminhos de aprofundamento. A seleção final é do usuário.
