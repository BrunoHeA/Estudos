# Anotações referente ao curso "HTML e CSS: responsividade com mobile-first" - **Finalizado**

Projeto refente ao seguinte repositorio: [Repositorio](https://github.com/BrunoHeA/projeto-alurabooks)

---
## Aula 01 - Aplicando a metodologia mobile-first

nada de novo, só iniciando o site mesmo.

---
## Aula 02 - Criando Header, Flexbox e @import

### **Label**

O Label serve para associar, um elemento a outro pelo ID, como por exemplo:

```HTML
<input type="checkbox" id="menu">
<label for="menu">
    <span></span>
</label>
```
Aqui ele faz com que o input tambem funcione apertando no span, por que os 2 estão associados graças ao label.

### **Position**

O position: relative libera a opção de colocar outros atributos como top, left, right e bottom. ja o position: absolute permite que você movimente o elemento de acordo com outro que venha antes ou seja o pai, mas eles precisam ser diferente de static que é o padrão.

---
## Aula 03 - Integrando o Carrossel com o SwiperJS

### **SwiperJS**

SwiperJS é uma api em que é possivel importar no projeto HTML, ele mexe um pouco com o JavaScript mas não sendo nenhum pouco aprofundado, então até mesmo eu que não sei nada sobre JavaScript posso usar. O SwiperJs serve para criar um carrossel de imagens, é basicamente um facilitador, pois, é possivel cirar um carrossel com o html mas é muito complexo e com o SwiperJS tudo se torna muito mais simples. Para mais informações sobre a API basta acessar o site official [AQUI](https://swiperjs.com/).

### **Wrap**

flex-wrap: wrap é uma estilização utilizada junto com o flex-box para que o conteudo ao chegar no limite da tela, ele faça uma quebra de linha oa invéz de tentar esticar a tela como ele faz por padrão.

---
## Aula 04 - Selecionando Media Queries

nada de novo, apenas usando das mesmas coisas só que com o media queries para estilizar em outro tamanho de tela.

---
## Aula 05 - Produzindo CSS no desktop

### **Combinadores CSS**

"~" - Procura outro elemento que esteja abaixo dele("irmão"), como por exemplo:

```CSS
/* Nesse exemplo ele procura a classe .container-rotulo que esteja embaixo da classe .container-botao */
.container-botao:checked ~ .container-rotulo {
    background: var(--azul-degrade);
}
```

">" - Procura outro elemento que esteja dentro(filho) do elemento anterior, como por exemplo:

```CSS
/* Nesse exemplo ele procura a classe .cabecalho-menu-h que esteja dentro da classe .container-rotulo */
.container-botao:checked ~ .container-rotulo > .cabecalho-menu-h {
    background-image: url("../assets/Menu Aberto.svg");
}
```

"+" - Procura outro elemento que esteja abaixo dele("irmão") mas esse precisa necessariamente estar logo abaixo grudado com a classe, como por exemplo.

```CSS
/* Nesse exemplo ele procura a classe .container-rotulo que esteja embaixo da classe .container-botao mas a classe .container botão tem que estar grudada com a .container-rotulo no HTML */
.container-botao:checked ~ .container-rotulo {
    background: var(--azul-degrade);
}
```

---
## Aula 06 - Publicando o projeto

nada novo, só publicação do projeto.