# Muralha de Aço

Jogo de defesa de torres feito em HTML5 Canvas, num único arquivo (`index.html`), sem dependências.

Colunas de veículos inimigos avançam pela estrada até a sua base. Monte armas ao lado do caminho para impedir que cheguem ao fim.

## Como jogar

Abra `index.html` no navegador (computador ou celular). No celular, jogue na horizontal: o jogo entra em tela cheia ao escolher a fase e o botão **Tela cheia** liga ou desliga isso. Se o dedo cair um pouco em cima da pista, a arma vai para o quadrado livre mais próximo.

- Toque na arma no painel e depois num quadrado livre ao lado da pista: a arma é instalada na hora. Os lugares livres ficam destacados enquanto a arma está selecionada.
- Toque numa arma já construída para **melhorar** (até o nível 3), mudar o **alvo** (primeiro, mais forte, mais perto) ou **vender** (devolve 70%).
- **Chamar onda** antecipa a próxima onda e dá energia extra.
- **x2 / x3** acelera o jogo; **II** pausa.
- **Ataque aéreo**: bombardeio em área que recarrega em 40 s.
- Teclado: `1`–`6` escolhem armas, `U` melhora, `N` chama a onda, `Espaço` pausa, `Esc` cancela.

## Inimigos (ficam mais fortes a cada onda)

| Veículo | Vida | Velocidade | Blindagem |
|---|---|---|---|
| Buggy | muito baixa | muito rápida | 0 |
| Carro | baixa | rápida | 0 |
| Jipe | média | rápida | 2 |
| Blindado | alta | média | 5 |
| Tanque leve | alta | lenta | 7 |
| Tanque pesado | muito alta | lenta | 13 |
| Colosso (chefe, onda 20) | enorme | muito lenta | 18 |

A blindagem é descontada de cada tiro, então metralhadoras quase não ferem tanques pesados. Mísseis perfuram parte da blindagem, e o laser e o EMP a ignoram.

## Armas

| Arma | Custo | Libera na fase | Função |
|---|---|---|---|
| Metralhadora | 50 | 1 | rajada rápida contra veículos leves |
| Canhão | 90 | 1 | dano em área |
| Pulso EMP | 70 | 1 | deixa os inimigos lentos |
| Mísseis | 150 | 2 | teleguiados, perfuram blindagem |
| Laser | 130 | 3 | feixe contínuo que esquenta e ignora blindagem |
| Artilharia | 200 | 4 | alcance muito longo, grande explosão |

## Fases

6 mapas com 20 ondas cada: Estrada do Vale, Zona Industrial, Dunas de Areia, Floresta Negra, Passo Gelado e Cinzas do Vulcão. Vencer uma fase libera a próxima. As estrelas dependem das vidas que sobraram (3 estrelas = nenhuma vida perdida). O progresso fica salvo no navegador.
