# Listagem Pokémon

Página com cartões de dez Pokémon, cada um com imagem animada, descrição e tipos, e alternância entre tema claro e escuro.

**Online:** https://ygos-96.github.io/listagem-pokemon/

Projeto de estudo de HTML, CSS e JavaScript, feito para praticar layout em grade, estados de interação (`hover`) e manipulação do DOM.

## O que faz

- Exibe 10 cartões com GIF, nome, descrição e tipos do Pokémon.
- Leve ampliação ao passar o mouse sobre cada cartão e sobre os botões do cabeçalho.
- **Botão de tema:** alterna entre modo claro e escuro e troca o ícone (sol e lua).
- Barra de rolagem personalizada para a lista.

## Como está organizado

```
index.html
src/css/   reset.css, estilos gerais (estilos.css) e scrollbar.css
src/js/    index.js (troca de tema)
src/imagens/   GIFs dos Pokémon e ícones do tema
```

O modo escuro é uma classe (`modo-escuro`) aplicada ao `body`. Todo o restante é decidido no CSS a partir dela, então o JavaScript só alterna a classe e o ícone.

## Tecnologias

HTML5, CSS3 (Flexbox, Grid, pseudoclasses) e JavaScript puro.

## Rodar localmente

Abra o `index.html` no navegador, ou use qualquer servidor estático:

```bash
npx serve .
```

## Limitações conhecidas

- Os dados dos Pokémon estão escritos direto no HTML. Uma evolução natural seria buscar da PokéAPI e gerar os cartões por JavaScript.
- O tema escolhido não é salvo entre visitas.
