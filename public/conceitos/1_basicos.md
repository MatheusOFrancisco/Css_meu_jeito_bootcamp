# 🟢 Nível 01 — Fundamentos do CSS\

### Aqui o CSS ainda está cru, quase não da para fazer muitas coisas, apenas mudar o tamanho e cor de algumas coisas

## 📖 Introdução

### O QUE É CSS?
O CSS (Cascading Style Sheets) é uma linguagem utilizada para definir a apresentação visual de documentos HTML. Por meio dele, é possível controlar cores, fontes, espaçamentos, dimensões, posicionamento e diversos outros aspectos de uma página web.

Neste nível, serão apresentados os fundamentos da linguagem, desde sua integração com HTML até os principais conceitos utilizados na estilização de elementos.

---

## 📚 Conteúdos

### 1. Introdução ao CSS

Entender o que é CSS, sua importância no desenvolvimento web e como ele trabalha em conjunto com o HTML.

- **HTML:** responsável pela estrutura e pelo conteúdo da página.
- **CSS:** responsável pela apresentação visual e pelo layout.
- **JavaScript:** responsável pelo comportamento e pela interatividade.

### 2. Formas de adicionar CSS ao HTML

Existem três maneiras principais de aplicar estilos a um documento HTML:

- **Inline CSS:** aplicação de estilos diretamente na tag HTML por meio do atributo `style`.
- **Internal CSS:** utilização da tag `<style>` dentro do documento HTML.
- **External CSS:** criação de um arquivo `.css` separado, conectado ao HTML através da tag `<link>`.

A utilização de arquivos externos é geralmente recomendada por facilitar a organização, manutenção e reutilização dos estilos.

### 3. Seletores e especificidade

Os seletores permitem identificar quais elementos HTML receberão determinada estilização.

Principais seletores:

- **Universal (`*`):** seleciona todos os elementos.
- **Elemento (`p`, `h1`, `div`):** seleciona elementos pelo nome da tag.
- **Classe (`.classe`):** seleciona elementos que possuem determinada classe.
- **ID (`#id`):** seleciona um elemento pelo seu identificador.

A especificidade determina qual regra CSS terá prioridade quando diferentes seletores aplicarem propriedades conflitantes ao mesmo elemento.

### 4. Cores e backgrounds

O CSS oferece diferentes maneiras de trabalhar com cores e planos de fundo.

- `color`: define a cor do texto.
- `background-color`: define a cor de fundo.
- `background-image`: adiciona imagens ao fundo.
- `background-size`: controla o dimensionamento da imagem.
- `background-position`: define o posicionamento do fundo.
- `background-repeat`: controla a repetição da imagem.

As cores podem ser representadas por nomes, valores HEX, RGB, RGBA, HSL e HSLA.

### 5. Fontes e tipografia

A tipografia influencia diretamente a legibilidade e a identidade visual de uma interface.

Principais propriedades:

- `font-family`: define a família tipográfica.
- `font-size`: controla o tamanho da fonte.
- `font-weight`: define a espessura do texto.
- `font-style`: controla o estilo da fonte.
- `text-align`: define o alinhamento do texto.
- `text-decoration`: adiciona ou remove decorações.
- `line-height`: controla o espaçamento entre linhas.
- `letter-spacing`: controla o espaçamento entre caracteres.

### 6. Unidades de medida

As unidades de medida definem dimensões, espaçamentos e tamanhos dos elementos.

**Unidades absolutas:**
- `px`: pixels, unidade de referência fixa no CSS.

**Unidades relativas:**
- `%`: valor relativo ao elemento de referência, dependendo da propriedade.
- `em`: relativo ao tamanho da fonte do elemento de referência.
- `rem`: relativo ao tamanho da fonte do elemento raiz (`html`).
- `vw`: relativo à largura da viewport.
- `vh`: relativo à altura da viewport.

A escolha da unidade influencia a flexibilidade e a capacidade de adaptação do layout.

### 7. Margin e Padding

São propriedades utilizadas para controlar os espaçamentos dos elementos.

- `margin`: define o espaçamento externo, separando um elemento dos demais.
- `padding`: define o espaçamento interno, entre o conteúdo e a borda do elemento.

Ambas permitem configurações individuais para os lados superior, inferior, esquerdo e direito.

### 8. Borders e Outlines

Permitem adicionar contornos aos elementos HTML.

- `border`: define uma borda ao redor do elemento.
- `border-width`: controla a espessura.
- `border-style`: define o estilo da borda.
- `border-color`: define sua cor.
- `border-radius`: arredonda os cantos.
- `outline`: adiciona um contorno externo que não ocupa espaço no layout.

### 9. Display

A propriedade `display` determina como um elemento participa do fluxo de layout.

Principais valores:

- `block`: ocupa uma linha e, por padrão, utiliza toda a largura disponível.
- `inline`: ocupa apenas o espaço necessário ao conteúdo e não aceita todas as dimensões da mesma maneira que elementos block.
- `inline-block`: combina características dos dois modelos.
- `none`: remove o elemento da apresentação e do fluxo do documento.

### 10. Pseudo-classes

Permitem estilizar elementos em situações específicas ou partes de um elemento.

**Pseudo-classes:**
- `:hover`: quando o cursor está sobre um elemento.
- `:active`: enquanto o elemento está sendo ativado.
- `:focus`: quando o elemento recebe foco.
- `:first-child`: seleciona o primeiro filho.
- `:last-child`: seleciona o último filho.

---

## 🎯 Objetivo do nível

Ao concluir esta etapa, será possível compreender a estrutura básica do CSS, aplicar estilos a documentos HTML e controlar os principais aspectos visuais de uma página.

Esses conhecimentos servirão como base para os próximos níveis, nos quais serão exploradas técnicas mais avançadas de organização, posicionamento e estilização de interfaces.