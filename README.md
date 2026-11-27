# jogos

Menu "Jogar e aprender": um botão para cada jogo ou modelo de ciência (abre em nova aba).

Publicação: GitHub Pages → https://paineis-gerenciais.github.io/jogos/

A capa que leva a este menu fica em https://paineis-gerenciais.github.io/geral/ (repositório `geral`).

## Arquivos

- `index.html` — o menu (HTML + CSS, sem JavaScript). Os botões e o símbolo são feitos em código, não em imagem.
- `favicon.svg` — ícone da aba do navegador.
- `marca/` — a marca deste menu: símbolo, assinaturas, ícones, cores e folha da marca.
- `assets/fundo.webp` — imagem de fundo.

## Adicionar ou tirar um jogo

Cada botão é um `<li>` em `index.html`.

- **Adicionar:** copie um `<li>` existente e troque quatro coisas: o endereço (`href`), a descrição lida por leitores de tela (`aria-label`), a linha de cima (`class="linha"`) e o nome (`class="nome"`).
- **Ícone:** é o desenho dentro de `<svg>`. Dá para repetir um ícone existente ou pedir um novo.
- **Tirar:** apague o `<li>` do jogo.
- **Em breve:** projeto ainda não publicado entra como um bloco `<div class="botao azul breve">`, sem endereço, com o selo "Em breve". Não tem clique. Esses botões ficam depois dos publicados.
- **Publicou um "Em breve":** apague o `<li>` dele e crie um botão normal, copiando um dos publicados e aproveitando o mesmo ícone.

Os endereços são relativos (`../quadra/`): funcionam enquanto o jogo estiver publicado na mesma conta. Para um jogo em outro endereço, use o endereço completo.

## Imagem de fundo

O fundo é a imagem `assets/fundo.webp`, com um véu marfim por cima para não disputar com os botões. O prompt que gerou a imagem está no `ARTE.md` do repositório `geral`.

- **Trocar a imagem:** salve a nova por cima de `assets/fundo.webp` (1920 px de largura, até 300 KB).
- **Clarear ou escurecer:** no alto do `index.html`, mude o último número de `--veu`. Mais perto de `1` clareia; mais perto de `0` mostra mais a imagem.
- **Tirar a imagem:** no alto do `index.html`, troque o valor de `--fundo` por `none`. O fundo volta ao marfim liso.
