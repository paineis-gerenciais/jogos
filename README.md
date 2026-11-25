# jogos

Menu "Jogar e aprender": um botão para cada jogo ou modelo de ciência (abre em nova aba).

Publicação: GitHub Pages → https://paineis-gerenciais.github.io/jogos/

A capa que leva a este menu fica em https://paineis-gerenciais.github.io/geral/ (repositório `geral`).

## Arquivos

- `index.html` — o menu (HTML + CSS, sem JavaScript). Os botões são feitos em código, não em imagem.
- `assets/` — criar quando a arte ficar pronta (`simbolo.webp` e `fundo.webp`). Os prompts estão em `ARTE.md`, no repositório `geral`.

## Adicionar ou tirar um jogo

Cada botão é um `<li>` em `index.html`.

- **Adicionar:** copie um `<li>` existente e troque quatro coisas: o endereço (`href`), a descrição lida por leitores de tela (`aria-label`), a linha de cima (`class="linha"`) e o nome (`class="nome"`).
- **Ícone:** é o desenho dentro de `<svg>`. Dá para repetir um ícone existente ou pedir um novo.
- **Tirar:** apague o `<li>` do jogo.

Os endereços são relativos (`../quadra/`): funcionam enquanto o jogo estiver publicado na mesma conta. Para um jogo em outro endereço, use o endereço completo.

## Colocar a arte

1. Salve as imagens em `assets/simbolo.webp` (512 px de lado) e `assets/fundo.webp` (1920 px de largura).
2. No alto do `index.html`, troque `--fundo: none;` por `--fundo: url("assets/fundo.webp");`.
3. Troque o bloco `<svg class="simbolo">…</svg>` pela linha `<img>` que está no comentário logo acima dele.
