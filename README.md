# Offer Miner — laboratório de pesquisa internacional

Repositório de **contexto, procedimentos, agentes e resultados** para executar missões de mineração de ofertas no **Orca usando Claude Code**.

Este **não** é um aplicativo web. Não há frontend, backend, banco de dados nem processamento autônomo fora das sessões do Claude Code. O Orca organiza as sessões/worktrees; o Claude segue as instruções deste repositório e usa as ferramentas de pesquisa que estiverem realmente disponíveis.

## Início rápido

1. Crie um repositório GitHub privado (sugestão: `offer-miner`) e publique nele estes arquivos.
2. Clone o repositório para sua máquina.
3. No Orca, use **Add Repo** e selecione o diretório local clonado.
4. Abra uma sessão com **Claude Code**, na raiz do projeto. O arquivo `CLAUDE.md` é o contexto principal.
5. Verifique se a sessão tem ferramentas de busca web e navegação. Se não tiver, configure os acessos antes de exigir coleta real de informações. Um arquivo Markdown ou um agente não concede acesso web por si só.
6. Envie a missão de exemplo abaixo. Revise o plano e os resultados antes de integrar alterações à branch principal.

### Primeira missão no Orca

> Execute a skill `offer-mining` para uma missão exploratória: país-alvo Estados Unidos; problema dificuldade para dormir; mecanismos cortisol, melatonina e relaxamento; idiomas inglês e espanhol, com expansão apenas quando relevante; profundidade inicial 1; até 5 ofertas documentadas; máximo de 30 consultas de busca. Registre URL, data e evidência de cada afirmação. Não trate anúncios ativos como vendas comprovadas. Grave o resultado em `results/` seguindo os templates e mostre limitações de acesso.

## Organização

- `CLAUDE.md` — regras permanentes do projeto
- `.claude/agents/` — papéis delegáveis de pesquisa, investigação e auditoria
- `.claude/skills/` — processos reutilizáveis de mineração, busca multilíngue e validação
- `docs/` — padrões de evidência e ferramentas
- `missions/` — missões de exemplo/briefings
- `templates/` — formatos de saída
- `results/` — relatórios gerados nas sessões (não versionar arquivos brutos protegidos sem direito de uso)

## Limite da primeira versão

- Pesquisa feita **sob demanda**, em sessão do Orca.
- Relatórios Markdown + JSON local, com referências rastreáveis.
- Sem promessas de dados de vendas/ROAS de concorrentes; esses dados geralmente não são públicos.
- Sem publicação automática de anúncios, sem criação de criativos e sem modificação de sistemas externos.
- Pesquisas em suplementos são **análise de mercado**, não orientação de saúde; qualquer alegação exige verificação científica e regulatória no mercado de destino.

## Próximas evoluções, somente depois de testar

Adicionar provedores de busca com acesso permitido; análise de vídeos com FFmpeg/ferramentas compatíveis; resumos por país; comparador de ofertas; eventualmente exportação estruturada. Evitar criar aplicativo ou banco de dados prematuramente.
