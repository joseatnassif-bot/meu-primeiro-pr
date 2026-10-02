# Fotos do site

Fotos reais da Santino Prime Meats usadas no `index.html`. Se um arquivo sumir, o site mostra um fundo neutro com o monograma "S" no lugar (menos nos banners do topo).

| Arquivo                               | Onde aparece                                              |
| ------------------------------------- | --------------------------------------------------------- |
| `santino-banner-loja.webp`            | Topo, banner 1 (interior da loja)                         |
| `santino-banner-area-externa.webp`    | Topo, banner 2 no computador (área externa, horizontal)   |
| `santino-area-externa-vertical.webp`  | Topo, banner 2 no celular (mesma cena, vertical)          |
| `santino-fachada.webp`                | Seção "Mais que um açougue": foto principal (a loja)      |
| `santino-area-externa-coqueiros.webp` | Seção "Mais que um açougue": foto menor (a experiência)   |
| `santino-cortes.webp`                 | Fundo da chamada "Procurando um corte específico?"        |

## Produtos (`produtos/`)

Fotos dos produtos tiradas pela loja, usadas na seção "Nossos cortes". Cada foto existe em 2 tamanhos (o número no fim do nome é a largura em pixels): o navegador escolhe o menor que fica nítido na tela (`srcset`). As fotos com dois produtos (picanhas Guidara e VPJ; hambúrguer e bacon VPJ) foram recortadas para cada produto ter seu card; a versão `-1200` inteira é a que abre ampliada.

Os dados de cada card (nome, marca, etiqueta, categoria do filtro e mensagem do WhatsApp) ficam no `index.html`, dentro de `<ul class="grid" id="productGrid">`. Para um produto novo, copie um `<li class="card">`, troque os textos e as fotos e ajuste `data-cat` (`wagyu`, `angus`, `grassfed`, `dia` ou `burger`) e o número do filtro correspondente.

Para trocar uma foto, substitua o arquivo mantendo o nome. Se o formato mudar muito (por exemplo, uma vertical no lugar de uma horizontal), ajuste também os atributos `width`/`height` e o texto `alt` no `index.html`.

Dicas:

- Fotos com luz quente e fundo escuro combinam com o visual do site.
- A fachada e a área externa são recortadas pela parte de baixo da foto: deixe a placa e a cobertura na metade de baixo.
- Os banners do topo ficam atrás do texto, do lado esquerdo; o assunto principal funciona melhor no centro ou à direita.
- Mantenha cada arquivo abaixo de ~300 KB (WebP com qualidade ~80) para a página carregar rápido.
