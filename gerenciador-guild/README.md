# Gerenciador de Guild — PokeAlliance

Controle semanal da contribuição dos membros da guild (Cafe Do Psyduck): pontos de daily, valor doado, meta com verde/amarelo/vermelho, check de boss e total geral.

## Regra

- Daily normal = 1 ponto, wildscape = 2, primal = 4. O jogo já exporta a soma em `points` (nos exports antigos, `dailiesCompleted`).
- `contribution` no export é o valor em dinheiro doado para a guild. Os pontos de daily não entram nele.
- Contribuição da semana = valor doado + pontos × valor do ponto (150 por padrão).
- Meta semanal por membro, "perto a partir de (%)" e valor do ponto são campos abertos no topo da página. Verde = bateu a meta, amarelo = acima do percentual de "perto", vermelho = abaixo.
- No jogo os valores zeram toda semana, então cada export é o total de uma semana (segunda a domingo). O total geral soma as semanas importadas.

## Uso

1. No jogo, exporte os membros da guild (JSON ou CSV) no fim da semana.
2. Na página, "Importar export do jogo". A semana é deduzida da data do export e pode ser corrigida antes de confirmar. Reimportar a mesma semana troca os números e mantém as marcações de boss.
3. Marque quem participou do boss da semana. Pontos e valor doado podem ser corrigidos direto na tabela.
4. "Exportar semana (JSON)" e "Exportar tudo (JSON)" geram os valores já calculados.

A [página publicada](https://claude.ai/artifact/NHRNB1TQZpToikwrJWMDQx) guarda os dados num banco compartilhado: quem tiver acesso de Colaborador ou acima edita, quem tiver só leitura apenas vê. Abrir `index.html` direto no navegador também funciona, mas aí os dados ficam só naquele navegador e não se misturam com os da página publicada.

`exports/` guarda os exports originais do jogo já importados (06/09, 27/09 e 08/11/2026).
