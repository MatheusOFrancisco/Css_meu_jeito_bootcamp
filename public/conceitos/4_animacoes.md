# 🟣 Nível 04 — Animações

## 📖 Introdução

As animações em CSS permitem adicionar movimento, transições e efeitos visuais aos elementos de uma página web, tornando as interfaces mais dinâmicas e interativas.

Por meio de propriedades específicas, é possível controlar como um elemento muda de aparência, tamanho, posição e outras características ao longo do tempo, sem necessariamente utilizar JavaScript.

Neste nível, serão explorados os principais recursos de animação do CSS, desde transições simples até animações personalizadas com Keyframes.

---

## 📚 Conteúdos

### 1. Introdução às animações CSS

Compreender como funcionam as animações em CSS e qual é sua importância na construção de interfaces.

As animações permitem modificar gradualmente determinadas propriedades de um elemento, criando efeitos visuais como movimentos, mudanças de tamanho, alterações de cores e rotações.

Existem duas ferramentas principais:

- **Transitions:** permitem criar transições suaves entre diferentes estados de um elemento.
- **Animations:** permitem criar animações personalizadas, definindo diferentes etapas e comportamentos.

### 2. Transitions

A propriedade `transition` permite criar mudanças suaves entre diferentes valores de uma propriedade CSS.

Sem ela, algumas alterações acontecem imediatamente. Com uma transição, é possível determinar quanto tempo uma mudança levará para ser concluída.

Principais propriedades:

- `transition-property`: define qual propriedade será animada.
- `transition-duration`: determina a duração da transição.
- `transition-timing-function`: controla a velocidade da transição ao longo do tempo.
- `transition-delay`: define quanto tempo a transição aguardará antes de começar.

Também é possível utilizar a propriedade `transition` como atalho para configurar todos esses valores.

### 3. Transform

A propriedade `transform` permite modificar visualmente a posição, o tamanho, a inclinação e a orientação de um elemento.

Principais funções:

- `translate()`: desloca um elemento horizontalmente ou verticalmente.
- `scale()`: aumenta ou diminui o tamanho de um elemento.
- `rotate()`: rotaciona um elemento.
- `skew()`: inclina um elemento em determinado ângulo.

Essas transformações podem ser utilizadas individualmente ou combinadas.

### 4. Keyframes

A regra `@keyframes` permite criar animações personalizadas, definindo diferentes etapas que serão executadas ao longo do tempo.

É possível determinar o estado inicial, final e até mesmo pontos intermediários de uma animação.

Existem duas formas principais de definir essas etapas:

- `from`: representa o início da animação.
- `to`: representa o final da animação.
- Porcentagens (`0%`, `50%`, `100%`): permitem definir estados específicos durante a execução.

Os Keyframes são utilizados em conjunto com a propriedade `animation`.

### 5. Animation Properties

As propriedades `animation` controlam o comportamento das animações criadas com `@keyframes`.

Principais propriedades:

- `animation-name`: define o nome da animação que será executada.
- `animation-duration`: determina quanto tempo a animação levará para completar um ciclo.
- `animation-timing-function`: controla a velocidade da animação.
- `animation-delay`: define o tempo de espera antes do início.
- `animation-iteration-count`: determina quantas vezes a animação será executada.
- `animation-direction`: define a direção em que a animação será executada.
- `animation-fill-mode`: determina como o elemento ficará antes ou depois da animação.
- `animation-play-state`: permite controlar se a animação está em execução ou pausada.

Também será estudado o atalho `animation`, que permite configurar várias dessas propriedades em uma única declaração.

### 6. Timing Functions

A propriedade `animation-timing-function` e sua equivalente em transições, `transition-timing-function`, controlam como a velocidade de uma animação ou transição varia ao longo do tempo.

Principais valores:

- `linear`: mantém uma velocidade constante.
- `ease`: começa devagar, acelera e termina devagar.
- `ease-in`: começa devagar e acelera.
- `ease-out`: começa rápido e termina devagar.
- `ease-in-out`: começa devagar, acelera no meio e desacelera no final.
- `cubic-bezier()`: permite criar curvas de velocidade personalizadas.

Essas funções ajudam a deixar os movimentos mais naturais e adequados ao comportamento desejado.

### 7. Delays e Iterations

Essas propriedades permitem controlar quando e quantas vezes uma animação será executada.

**Animation Delay**

Define um intervalo de espera antes do início da animação.

**Animation Iteration Count**

Determina quantas vezes uma animação será repetida.

Principais valores:

- `1`: executa a animação uma vez.
- `2`, `3`, etc.: executa a quantidade de vezes definida.
- `infinite`: repete a animação continuamente.

Esses recursos são úteis para controlar a repetição de movimentos e criar efeitos contínuos.

### 8. Animações de Hover

O estado `:hover` permite aplicar estilos quando o cursor está sobre determinado elemento.

Quando combinado com `transition` ou `transform`, é possível criar efeitos visuais como:

- Aumentar o tamanho de um botão.
- Alterar a cor de um elemento.
- Rotacionar um ícone.
- Deslocar um componente.
- Criar efeitos de destaque.

Esses efeitos são bastante utilizados em botões, links, cards e menus de navegação.

### 9. Microinterações

Microinterações são pequenas respostas visuais ou comportamentais que acontecem quando o usuário interage com uma interface.

Elas ajudam a fornecer feedback e tornam a navegação mais intuitiva.

Exemplos:

- Botões que mudam de aparência ao serem pressionados.
- Ícones que reagem à interação.
- Indicadores visuais de carregamento.
- Elementos que aparecem gradualmente.
- Feedback visual ao passar o cursor sobre um componente.

O objetivo é melhorar a experiência do usuário sem adicionar movimentos desnecessários.

### 10. Animações responsivas

As animações também precisam considerar diferentes dispositivos e condições de utilização.

Uma animação que funciona bem em uma tela grande pode não apresentar o mesmo resultado em dispositivos menores.

Serão explorados conceitos como:

- Ajuste de intensidade e deslocamento dos movimentos.
- Adaptação das animações a diferentes tamanhos de tela.
- Evitar movimentos excessivos.
- Considerar o desempenho durante a execução.
- Respeitar as preferências de acessibilidade do usuário.

### 11. Prefers Reduced Motion

A preferência `prefers-reduced-motion` permite identificar quando o usuário configurou seu sistema operacional para reduzir movimentos e animações.

Essa funcionalidade é importante para tornar as interfaces mais acessíveis, especialmente para pessoas que podem sentir desconforto com movimentos intensos.

Exemplo:

```css
@media (prefers-reduced-motion: reduce) {
    * {
        animation-duration: 0.01ms;
        transition-duration: 0.01ms;
    }
}
```

Dessa maneira, é possível reduzir ou desativar movimentos não essenciais, respeitando as preferências do usuário.

---

## 🎯 Objetivo do nível

Ao concluir esta etapa, será possível criar transições suaves, transformações visuais e animações personalizadas utilizando CSS.

Também será possível compreender como controlar a duração, velocidade, repetição e comportamento dos movimentos, além de aplicar esses recursos em componentes de interface.

O conhecimento adquirido permitirá desenvolver páginas mais dinâmicas, interativas e acessíveis, preparando o aprendizado para o último nível do bootcamp: CSS Avançado.