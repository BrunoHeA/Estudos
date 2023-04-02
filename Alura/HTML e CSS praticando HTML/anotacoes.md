# Anotações referente ao curso "HTML e CSS: praticando HTML/CSS" - **Finalizado**

Projeto refente ao seguinte repositorio: [Repositorio](https://github.com/BrunoHeA/Projeto-HTML-e-CSS-01)

---
## Aula 01 - Iniciando o projeto

### **Classes**

É possivel colocar dois nomes para a mesma tag no HTML, da seguinte forma:

```HTML
<section class="principal apresentacao">
    <h1>Titulo</h1>
</section>
```
Assim a tag section tem a classe "principal" e a classe "apresentacao"

### **Background**

para colocar uma imagem de fundo, usamos o seguinte codigo no CSS:

```CSS
body {
    background-image: url("./assets/background.png");
}
```
e para que a imagem não se repita diversas vezes a fim de preencher todo o espaço vazio, utilizamos o seguinte codigo:

```CSS
body {
    background-repeat: no-repeat;
}
```

e para que a imagem use todo o espaço utilizamos o seguinte codigo:

```CSS
body {
    background-size: contain;
}
```
Ele usa o tamanho da tag pai para distinguir qual o tamanho maximo.

---
## Aula 02 - A dupla HTML e CSS

### **Medida em**

A medida relativa em significa literalmente o tamanho da font do navegador, então ele pega o tamanho padrão da fonte no navegador e coloca na medida em, como por exemplo:

```CSS
body {
    padding: 1em;
}
```
Digamos que o padrão do navegador é 16px de tamanho. <br>
Nesse caso 1em = 16px e 2em = 32px

### **Tag a e button**

Essas 2 tags são muito parecidas mas não iguais, elas podem confundir pois com a estilização, elas podem ser identicas visualmente, porém, por trás elas não são iguais, sendo a tag button mais recomendada na hora de executar uma função, como por exemplo apagar um formulario, geralmente algo envolvendo o JavaScript, ja a tag a é mais usada para redirecionamentos ou coisas mais simples.

**Grid**

Usando o grid como display, ele tenta separar os conteudos filhos em grid, usando o "grid-template-columns" da para definir o tamanho da coluna e quantas colunas havera na pagina como por exemplo:

```CSS
body {
    grid-template-columns: 50% 50%;
}
```
assim terá 2 colunas cada uma ocupando 50% do espaço da tag body.

---
## Aula 03 - Posicionando elementos

### **Margem e Padding**

A diferença da margem para o padding é que o padding ele aumenta o tamanho do elemento, e a margem ela aumenta o espaço em branco em volta, como por exemplo em um quadro com moldura, ele tendo uma margem de 10px é a mesma coisa que colocar um papel branco de 10px em volta da moldura, ja o padding é a mesma coisa que esticar a moldura para que ela chegue nesses 10px.

### **Align-itens**

Quando usado junto com o display grid, basicamente faz os itens irem para o centro da grid, como no projeto eu utilizei a coluna os itens acabam indo para o centro da coluna na qual eles estão dentro.

### **Text-align**

O text-align não alinha apenas textos, mas sim tudo que esta contido dentro do bloco, até imagens.

---
## Aula 04 - Finalizando nossa pagina

### **UL e LI**

Listas no html sáo muito simples na teoria, por que é so adicionar a tag UL para sinalizar o inicio de uma lista, e colocar dentro da tag LI os objetos da lista, sendo cada LI apenas 1 dessa lista, sendo possivel adicionar varios LI dentro de um UL como por exemplo:

```HTML
<ul class="dispositivos-lista">
    <li>
        <img src="./assets/tv.png" alt="icone de uma tv">
        <h3 class="lista-item">TV</h3>
    </li>
    <li>
        <img src="./assets/computador.png" alt="icone de um computador">
        <h3 class="lista-item">Computadores</h3>
    </li>
    <li>
        <img src="./assets/celular.png" alt="icone de um celular">
        <h3 class="lista-item">Celulares e tablets</h3>
    </li>
</ul>
```
### **PseudoClasses**

Nada mais que classes ja integradas no CSS como por exemplo:

:focus: é aplicada quando um elemento está em foco, pode ser pelo clique do mouse ou seleção pelo teclado. Um exemplo é quando os campos de escrita em formulários estão selecionados para o usuário escrever.

:hover: detecta quando um usuário está com o mouse em cima do elemento, sem necessariamente estar clicando.

:active: detecta quando o elemento está ativo, quando há uma interação, por exemplo: o link "a" está sendo clicado.

:visited: detecta quando o link a já foi visitado, ou seja, se você já clicou anteriormente naquele link.

:link: detecta quando é um link "a" que nunca foi clicado antes.

Exemplo de como são utilizados na pratica:

```CSS
/* 

seletor:pseudo-classe {
  propriedade: valor;
}

*/

a:hover {
    color: white;
}
a:active {
    color: purple;
}
```

---
## Aula 05 - Compartilhando o projeto

Nada de novo nessa aula somente explicação sobre como criar e o que é repositórios.