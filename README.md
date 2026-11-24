# PokeAlliance (PKA)

Ferramentas e guias do PokeAlliance feitos com o Claude, num lugar só.

| Pasta | O que é | Página publicada |
|---|---|---|
| [`calculadora-boost/`](calculadora-boost/) | Tabela de custo de criação das pedras de boost (+0 a +50, 18 tipos), com craftar vs. comprar pronto | [Calculadora de Boost](https://claude.ai/code/artifact/4cb89918-7c3c-449c-af04-173395f98963) |
| [`calculadora-hazard/`](calculadora-hazard/) | Dano das duplas por Hazard: testa as 15 duplas do time, runa de ataque (0 a 5), Brute Berry e precisão | [Calculadora de Hazard](https://claude.ai/artifact/3c472z5c26wd9FakVLMiTK) |
| [`hazard-tasks/`](hazard-tasks/) | Checklist das quests de Hazard por NPC, na ordem de fazer (sozinho primeiro, hunt lv alto por último) | — |
| [`guia-atk5/`](guia-atk5/) | Plano de pokelogs até 1.600 pts (ATK 5, +10% de ATK), em seis fases | [Pokelog ATK 5](https://claude.ai/code/artifact/dd017413-268a-47e8-8168-4c50f3bcc87f) |
| — | Briefing de sprite do Comandante Zahal | [Briefing de sprite](https://claude.ai/code/artifact/309475c7-1aed-4c67-b921-94f7235a88b8) |

## Como usar

- **Calculadora de boost:** abra `calculadora-boost/index.html` no navegador. Os dados ficam salvos no navegador.
- **Calculadora de Hazard:** abra `calculadora-hazard/index.html` no navegador. Time, runa e berries ficam salvos no navegador. A tabela de dano necessário está na constante `NEED`.
- **Hazard:** o checklist está em `hazard-tasks/README.md`. Para atualizar, mude as kills em `MORTOS` (e o `True`/`False` de "missão pega" em `N`) no `gerar.py` e rode `python hazard-tasks/gerar.py`, que reescreve o README.
- **Guia ATK 5:** abra `guia-atk5/index.html` no navegador. A cópia local salva o progresso só no navegador, e a página publicada salva na sua conta do Claude. As duas não se sincronizam, então escolha uma.

## De onde veio cada coisa

| Item | Conversa original | Data |
|---|---|---|
| Calculadora de boost | Sessão na nuvem (Claude Code web) no repo `ZAHAL/Petshop`, branch `claude/pokemon-creation-cost-table-rhuwap`. Depois virou o repo `pokealliance-boost-calculator`, que agora é este. | 20/09/2026 |
| Hazard | Sessão na nuvem no repo `ZAHAL/Petshop`, branch `claude/upbeat-dirac-smbvf1` (pasta `pokealliance-hazard-tasks/`) | 22 a 28/10/2026 |
| Guia ATK 5 | Sessão local no app Claude Desktop, "Guia Pokelogs ATK 5" | 28/10/2026 |

Novas conversas sobre o PKA: abra neste repo (na nuvem) ou na pasta `C:\Users\João Victor\PKA` (local), para elas ficarem juntas.
