# Viriatus Airsoft Store

Site da loja de airsoft Viriatus Airsoft Store (Viseu), loja parceira do Clube Airsoft Viriatus.

## O que está aqui

| Ficheiro | Para que serve |
| --- | --- |
| `index.html` | O site (montra). Abre em qualquer browser. |
| `dados.js` | Produtos, preços, contactos e categorias. **É aqui que se mudam os conteúdos.** |
| `img/` | Imagens das categorias, dos produtos e o emblema. |
| `versao-claude/loja-airsoft.html` | Versão com painel de gestão e encomendas. Só funciona dentro do Claude (usa a base de dados do Claude). Fica aqui como referência. |

## Ver o site

- No computador: descarregar o repositório e abrir `index.html` no browser.
- Online: ativar o GitHub Pages (Settings › Pages › Branch `main`, pasta `/ (root)`). O site fica em `https://<utilizador>.github.io/<repositorio>/`.

## Adicionar ou mudar um produto

1. Pôr a foto em `img/` (JPG, PNG ou SVG).
2. Em `dados.js`, na lista `"img"`, acrescentar uma linha com um código e o caminho da foto, por exemplo `"minha-aeg": "img/minha-aeg.jpg"`.
3. Em `"produtos"`, copiar um produto existente e mudar os campos: `id` (único, sem espaços), `nome`, `marca`, `categoria` (tem de existir em `cfg.categorias`), `preco`, `precoPromo` (0 se não houver), `stock`, `descricao`, `specs`, `imagens` (lista de códigos da alínea 2), `destaque`, `novidade`, `replica` (true nas armas: pede APD e 18+ no checkout) e `ativo`.
4. Guardar e recarregar o site.

## Notas

- As encomendas feitas nesta montra **não são registadas** nem pagas. A loja real vai ser montada em WordPress + WooCommerce, com MB WAY e Multibanco (ifthenpay).
- Os 12 produtos incluídos são exemplos para demonstração.
- Venda de réplicas só a maiores de 18 anos, sócios de uma APD (Lei n.º 5/2006).
