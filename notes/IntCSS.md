# CSS
- Cascading Style Sheets ou folha de estilo em cascata
- Apresentação visual
- Estilo para HTML
- declarações
- não aceita que declarações começem com numeros
- não aceita caracteres especiáis


```css

body {
  background: black;
  color: green;
}

```
## Cascading

- cascata (quando há 2 ou mais declarações, a ultima será a mais relevante)

```css

body {
  background: red;
}

body {
  background: blue;
}

```
## Specificity

- Especificidade (cada seletor tem um peso e a soma dos pesos, será lçevada em conta para que eterminada declaração seja mais específica)

- A cascata perde prioridade quando há especificidade

```css
/* quando utilizado um id o declaração começa com # */
#unico-1 {
  color: blue;
}

/* quando utilizado uma class a declaração começa com . */
.qualquer {
  color: green;
}

/* quando declaração tras o nome da tag ela vai considerar tudo que seja referente a ela, a menos que haja especificidade como nos exemplos acima*/
p {
  color: red;
}

```

## Box Model

- Tudo são caixas
- Caixas possuem determinadas propriedades

##### comportamento padrão das tags
- display inLine - "span" "img" "a" aqui não tem quebra de linha - isso faz com que não de para aplicar no css o "margin - auto" tem que transformar em block "display - block"
- display block -  "h1", "p", div aqui existe quebra de linha

##### :hover
- aplica as modificações quando passa o mouse pra cima