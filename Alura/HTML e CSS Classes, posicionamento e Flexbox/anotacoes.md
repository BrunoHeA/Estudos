# Anotações referente ao curso "HTML e CSS: Classes, posicionamento e Flexbox" - **Em Atualização!!!**
Objetivo do curso: Aprender mais sobre CSS.

---
## Aula 01 - Seletores e posicionamento

Classes no CSS servem para definir um conteudo especifico para alterar em vez da tag em geral:

```HTML
--------------------------------------------------------
Sem usar classes:

CSS:

p {
    color: blue;
}

HTML:

<p>Sem o uso de clase esse texto</p>
<p>e esse, ficam completamente azuis</p>
--------------------------------------------------------
Usando classes:

CSS:

.texto-azul {
    color: blue;
}

HTML

<p class="texto-azul">Com o uso de classes esse texto fica em azul</p>
<p>mas esse aqui continua na cor padrão</p>
--------------------------------------------------------
```
<br>
Box model:

<img src="box model.png">

Por padrão coisas como por exemplo a margem ja são pré feitos, então um bom costume é sempre resetar esses numeros com o seguinte codigo:
```CSS
* {
    margin: 0;
    padding: 0;
}
```
O simbolo "*" significa que estou puxando **TODAS** as tag e alterando todas ao mesmo tempo.

---

## Aula 02 - Posicionando mais elemetos

Height (Altura)
```CSS
body {
    height: 100vh;
} 
```
Faz com que a altura do Body seja equivalente a 100% da altura da view port (tamanho da tela)
<br>
VH = view height (altura da view port)
<br>
<br>
Box-sizing:
<br>
Imagem representa o conteudo dentro do "pai"
<img src="box-sizing01.png">
Exemplo de tag "pai" e "filho":
```HTML
<body>
    <p>Nesse Exemplo o "body" é a tag pai da tag "p"</p>
</body>
```
Nessa imagem o conteudo de uma tag "filho" esta saindo de dentro da tag "pai"
<img src="box-sizing02.png">
Porém, usando "border-box" em vez de "content-box" vemos que o tamanho do conteudo é reduzido automaticamente, para ficar dentro da tag "pai"
<img src="box-sizing03.png">