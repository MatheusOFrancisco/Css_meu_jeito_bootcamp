# 🔵 Nível 02 — Flexbox

## 📖 Introdução

O Flexbox é um modelo de layout do CSS desenvolvido para facilitar a organização, distribuição e alinhamento de elementos dentro de um container.

Diferentemente dos modelos tradicionais de posicionamento, o Flexbox permite organizar elementos de maneira dinâmica, controlando seus tamanhos, espaçamentos e alinhamentos de acordo com o espaço disponível.

Seu principal objetivo é simplificar a construção de interfaces flexíveis, facilitando a criação de layouts que se adaptam a diferentes dimensões de tela.

Neste nível, serão exploradas as principais propriedades do Flexbox, compreendendo como cada uma influencia a organização dos elementos e como combiná-las na construção de interfaces.

---

## 📚 Conteúdos

### 1. Introdução ao Flexbox

Compreender o funcionamento do modelo Flexbox e sua importância na construção de layouts modernos.

O Flexbox trabalha com dois elementos principais:

- **Flex Container:** elemento pai que recebe a propriedade `display: flex` e controla a organização dos seus filhos diretos.
- **Flex Items:** elementos filhos diretos que são organizados de acordo com as propriedades definidas no container.

Também serão apresentados os conceitos de eixo principal (Main Axis) e eixo transversal (Cross Axis), fundamentais para compreender os alinhamentos do Flexbox.

### 2. Display Flex

A propriedade `display` define como um elemento será apresentado no layout.

Ao utilizar `display: flex`, o elemento passa a funcionar como um Flex Container, permitindo organizar seus filhos diretos utilizando as propriedades do Flexbox.

Existem dois valores principais:

- `flex`: cria um container flexível que participa do fluxo normal como um elemento block.
- `inline-flex`: cria um container flexível que se comporta externamente como um elemento inline.

### 3. Flex Direction

A propriedade `flex-direction` determina a direção do eixo principal, definindo como os elementos serão organizados dentro do container.

Principais valores:

- `row`: organiza os elementos horizontalmente, da esquerda para a direita.
- `row-reverse`: organiza horizontalmente, invertendo a ordem visual.
- `column`: organiza os elementos verticalmente, de cima para baixo.
- `column-reverse`: organiza verticalmente, invertendo a ordem visual.

Essa propriedade é importante para definir a estrutura e a direção dos layouts.

### 4. Justify Content

A propriedade `justify-content` controla a distribuição e o alinhamento dos elementos ao longo do eixo principal.

Principais valores:

- `flex-start`: posiciona os elementos no início do eixo.
- `flex-end`: posiciona os elementos no final do eixo.
- `center`: centraliza os elementos.
- `space-between`: distribui os elementos com o maior espaço possível entre eles, sem espaço nas extremidades.
- `space-around`: distribui espaços ao redor dos elementos.
- `space-evenly`: distribui espaços iguais entre os elementos e as extremidades.

### 5. Align Items

A propriedade `align-items` controla o alinhamento dos elementos ao longo do eixo transversal.

Principais valores:

- `stretch`: estica os elementos para preencher o espaço disponível, respeitando as restrições de tamanho.
- `flex-start`: alinha os elementos no início do eixo transversal.
- `flex-end`: alinha os elementos no final do eixo transversal.
- `center`: centraliza os elementos.
- `baseline`: alinha os elementos de acordo com a linha de base do texto.

É bastante utilizada para centralizar elementos vertical ou horizontalmente, dependendo da direção definida em `flex-direction`.

### 6. Align Content

A propriedade `align-content` controla a distribuição das linhas ou colunas de um container Flexbox quando existe espaço livre no eixo transversal.

Ela é especialmente útil quando os elementos estão distribuídos em múltiplas linhas por meio de `flex-wrap`.

Principais valores:

- `flex-start`: agrupa as linhas no início do eixo transversal.
- `flex-end`: agrupa as linhas no final.
- `center`: centraliza as linhas.
- `space-between`: distribui o espaço entre as linhas.
- `space-around`: distribui espaços ao redor das linhas.
- `space-evenly`: distribui espaços iguais entre as linhas.
- `stretch`: estica as linhas para ocupar o espaço disponível.

**Importante:** diferentemente de `align-items`, essa propriedade trabalha com a distribuição das linhas do Flex Container, não com o alinhamento individual dos elementos.

### 7. Flex Wrap

A propriedade `flex-wrap` determina se os elementos devem permanecer em uma única linha ou se podem ser distribuídos em múltiplas linhas quando não existe espaço suficiente.

Principais valores:

- `nowrap`: mantém todos os elementos em uma única linha.
- `wrap`: permite que os elementos que não cabem sejam transferidos para a próxima linha.
- `wrap-reverse`: permite a quebra, mas inverte a direção de formação das linhas.

Essa propriedade é especialmente importante na construção de layouts responsivos.

### 8. Gap

A propriedade `gap` define o espaçamento entre os elementos de um container Flexbox, evitando a necessidade de utilizar margens individuais para criar separações.

Principais variações:

- `gap`: define o espaçamento entre linhas e colunas.
- `row-gap`: controla o espaçamento entre as linhas.
- `column-gap`: controla o espaçamento entre as colunas.

É uma alternativa mais organizada para controlar os espaços entre os elementos.

### 9. Flex Grow, Flex Shrink e Flex Basis

Essas três propriedades controlam como os elementos flexíveis ocupam e distribuem o espaço disponível dentro do container.

**Flex Grow**

Define a capacidade de um elemento crescer para ocupar o espaço livre disponível.

- `0`: o elemento não cresce para ocupar o espaço restante.
- `1`: permite que o elemento cresça proporcionalmente aos demais itens.

**Flex Shrink**

Define a capacidade de um elemento diminuir de tamanho quando não existe espaço suficiente no container.

- `0`: impede que o elemento diminua por falta de espaço.
- `1`: permite que o elemento diminua proporcionalmente aos demais itens.

**Flex Basis**

Define o tamanho inicial de um elemento antes da distribuição do espaço livre ou da redução dos itens.

Pode receber valores como `auto`, `0`, `200px`, `30%`, entre outros.

Também será estudada a propriedade abreviada `flex`, que permite configurar os três comportamentos em uma única declaração.

### 10. Align Self

A propriedade `align-self` permite alterar individualmente o alinhamento transversal de um Flex Item, sobrescrevendo o comportamento definido pelo `align-items` do container.

Principais valores:

- `auto`: utiliza o alinhamento definido pelo container.
- `flex-start`: alinha o elemento no início do eixo transversal.
- `flex-end`: alinha no final.
- `center`: centraliza o elemento.
- `baseline`: alinha pela linha de base do texto.
- `stretch`: estica o elemento para ocupar o espaço disponível.

É útil quando um elemento específico precisa ter um alinhamento diferente dos demais.

### 11. Order

A propriedade `order` permite alterar a ordem visual dos elementos dentro de um Flex Container sem modificar a estrutura original do HTML.

Por padrão, todos os elementos possuem `order: 0`.

Elementos com valores menores aparecem antes dos elementos com valores maiores.

Essa propriedade pode ser utilizada para reorganizar visualmente componentes em diferentes tamanhos de tela.

**Importante:** alterar a ordem visual não altera necessariamente a ordem de leitura do documento ou a navegação pelo teclado.

### 12. Construção de layouts com Flexbox

Após compreender as propriedades individuais, serão exploradas suas combinações na construção de interfaces completas.

Exemplos de aplicações:

- Menus de navegação.
- Cabeçalhos e rodapés.
- Alinhamento de textos e imagens.
- Distribuição de cards.
- Centralização de elementos.
- Seções com colunas e linhas.
- Componentes responsivos.

O objetivo é compreender como combinar diferentes propriedades para solucionar problemas reais de organização e alinhamento.

---

## 🎯 Objetivo do nível

Ao concluir esta etapa, será possível compreender o funcionamento do Flexbox e utilizar suas propriedades para construir layouts flexíveis, organizados e adaptáveis.

O conhecimento adquirido permitirá desenvolver interfaces com maior controle sobre o posicionamento e a distribuição dos elementos, preparando o caminho para o próximo nível: CSS Intermediário.