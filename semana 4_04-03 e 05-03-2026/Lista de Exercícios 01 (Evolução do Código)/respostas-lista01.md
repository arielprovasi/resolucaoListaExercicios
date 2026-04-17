# Lista 01 - Desenvolvimento Web (HTML5)

## 1) Quais as tags principais da estrutura HTML5? Explique cada uma.

As principais tags de estrutura semântica do HTML5 são:

- `<!DOCTYPE html>`: declara que o documento usa HTML5.
- `<html>`: elemento raiz de toda a página.
- `<head>`: metadados do documento (charset, viewport, title, links de CSS, etc.).
- `<body>`: conteúdo visível da página.
- `<header>`: cabeçalho da página ou de uma seção.
- `<nav>`: bloco de navegação com links principais.
- `<main>`: conteúdo principal e único da página.
- `<section>`: seção temática do conteúdo.
- `<article>`: conteúdo independente (post, notícia, card completo).
- `<aside>`: conteúdo complementar (barra lateral, observações).
- `<footer>`: rodapé da página ou seção.

## 2) Cite e explique pelo menos seis tags removidas ou obsoletas na HTML5.

Exemplos de tags removidas/desaconselhadas:

- `<font>`: usada para cor/tamanho/fonte; substituída por CSS.
- `<center>`: centralização visual; substituída por CSS.
- `<big>`: aumentava tamanho do texto; substituída por CSS.
- `<tt>`: texto monoespaçado; substituída por CSS (`font-family`).
- `<strike>`: riscava texto de forma visual; usar CSS ou semântica adequada (`<del>` para conteúdo removido).
- `<frame>` e `<frameset>`: estrutura antiga de frames; substituídas por layout moderno e, quando necessário, `<iframe>`.
- `<acronym>`: substituída por `<abbr>`.

## 3) Estrutura básica do HTML5 (itens I, II e III)

Analise:

- I. `head: primeira linha de código do documento antes da tag HTML.` -> **Falso** (a primeira linha é o `<!DOCTYPE html>`; `head` fica dentro de `<html>`).
- II. `doctype: define uma nova seção genérica no documento.` -> **Falso** (`doctype` declara o tipo de documento, não cria seção).
- III. `body: define o corpo (conteúdo) da página.` -> **Verdadeiro**.

Resposta correta: **c) Somente o item III.**

## 4) Citar livro e definir termo técnico em um parágrafo

Exemplo:

`Segundo o livro "HTML e CSS: Projete e Construa Websites", de Jon Duckett, a semântica no HTML melhora a organização do conteúdo; por isso, SEO (Search Engine Optimization) é o conjunto de técnicas usadas para otimizar páginas e melhorar seu posicionamento nos mecanismos de busca.`

## 5) Projeto do blog (requisitos)

Foi implementado no diretório `blogFulano`, contendo:

- logo e favicon exclusivos (arquivos SVG autorais);
- imagem com `title` e `alt`;
- lista ordenada com números romanos;
- estrutura com `index.html` e `paginas/curriculo.html`.

## 6) Página `curriculo.html`

Foi criada em `blogFulano/paginas/curriculo.html` com informações de perfil, formação e habilidades, conforme o objetivo da atividade.

## 7) Identificar tags, atributos e valores

a) `<img src="logo.jpg" alt="Logomarca do blog">`

- Tag: `img`
- Atributos: `src`, `alt`
- Valores: `"logo.jpg"`, `"Logomarca do blog"`

b) `<meta charset="UTF-8">`

- Tag: `meta`
- Atributo: `charset`
- Valor: `"UTF-8"`

c) `<hr width="100%">`

- Tag: `hr`
- Atributo: `width`
- Valor: `"100%"`

d) `<link rel="short icon" href="imagens/logoFavicon.png">`

- Tag: `link`
- Atributos: `rel`, `href`
- Valores: `"short icon"`, `"imagens/logoFavicon.png"`

e) `<meta name="viewport" content="width=device-width, initial-scale=1.0">`

- Tag: `meta`
- Atributos: `name`, `content`
- Valores: `"viewport"`, `"width=device-width, initial-scale=1.0"`

## 8) Tags de formatação desaconselhadas e alternativas

Desaconselhadas por falta de semântica:

- `<b>` apenas para estilo visual
- `<i>` apenas para estilo visual
- `<u>`
- `<font>`
- `<center>`
- `<strike>`

Alternativas recomendadas:

- `<strong>` para importância semântica
- `<em>` para ênfase semântica
- `<mark>` para destaque relevante
- `<del>` e `<ins>` para alterações de conteúdo
- CSS para apresentação visual (cor, fonte, alinhamento, tamanho etc.)

## 9) Importância das tags semânticas no HTML5

Tags semânticas melhoram:

- **Acessibilidade**: leitores de tela entendem melhor a estrutura.
- **SEO**: mecanismos de busca identificam hierarquia e contexto do conteúdo.
- **Manutenção**: código fica mais legível, organizado e fácil de evoluir.
- **Interoperabilidade**: padrão mais consistente entre navegadores e ferramentas.

## 10) Atributos da tag `<img>` além de `src`

Principais atributos:

- `alt`: texto alternativo para acessibilidade e fallback quando a imagem não carrega.
- `title`: dica textual ao passar o mouse (uso complementar).
- `width` e `height`: reservam espaço e evitam layout shift.
- `loading`: controla o carregamento de imagens.
- `srcset`: lista de versões da imagem para diferentes resoluções.
- `sizes`: informa ao navegador qual tamanho de renderização será usado.
- `fetchpriority`: ajuda a priorizar download de imagens críticas.
