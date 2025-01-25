
# Índice

- [Formas de usar o CSS](#formas-de-usar-o-css)
  - [Inline CSS](#inline-css)
  - [Internal CSS](#internal-css)
  - [External CSS](#external-css)
- [Seletores](#seletores)
  - [Classes](#classes)
  - [ID](#id)
- [Cores](#cores)
- [Background](#background)
  - [Imagem](#imagem)
- [Text](#text)
  - [Alinhamento de textos](#alinhamento-de-textos)
  - [Decoração de texto](#decoração-de-texto)
  - [Transformação de texto](#transformação-de-texto)
  - [Espaçamento de letras](#espaçamento-de-letras)
- [Fontes](#fontes)
  - [Estilo de Fonte](#estilo-de-fonte)
  - [Font Weight](#font-weight)
  - [Font Size](#font-size)
- [Box Model](#box-model)
  - [Padding](#padding)
  - [Margin](#margin)
  - [shorthand](#shorthand)
  - [Border](#border)
- [Display](#display)
  - [Inline](#inline)
  - [Block](#block)
  - [Hidden](#hidden)
- [Position](#position)
  - [Position Static](#position-static)
  - [Position Relative](#position-relative)
  - [Position Absolute](#position-absolute)
  - [Position Relative com Absolute](#position-relative-com-absolute)
  - [Position Fixed](#position-fixed)
  - [Position Sticky](#position-sticky)
  - [Z-index](#z-index)


# Formas de usar o CSS

- ***Inline CSS:*** Usa o atributo **`style`** direto no elemento [não Recomendado]
- *Internal CSS: Usa a tag* `<style>`  dentro do head
- *External CSS: Usa a tag <link /> para linkar um arrquivo externo de CSS*
- *Frameworks: Bootstrap, Materialize, Bulma, Tailwind CSS e outros*
- *Pré-processadores: SASS, LESS, Styled Components e outros*
- *CSS in JS: Styled Components, Emotion e outros*

### ***Inline CSS***

```html
<h1 
		style="color: blueviolet; font-size: 50px;"
		> Mudar cor e tamanho da fonte
</h1>
```

### *Internal CSS*

```html
<style>
	  h1 {
	    color: purple;
	  }
	  p {
	    color: gold;
	    font-size: 20px;
	    }
</style>
```

### *External CSS*

- Podem ser adicionados multiplos arquivos

```html
<link rel="stylesheet" href="css/Style.css" />
```

# Seletores

- Precedencia: `ID` > `Class` > `Tag`
- Pode ter ID e Class ao mesmo tempo

### Classes

- Usa o ponto (.) para identificar
- Pode ser usado várias vezes

```html
<p class="paragraph">Eu sou um parágrafo</p>
```

```css
.paragraph {
  color: orange;
}
```

### *ID*

- Usa o jogo da velha (#) para identificar
- Pode ser usado apenas uma vez

```html
<h1 id="exclusive-title">Eu sou um título com ID</h1>
```

```css
#exclusive-title {
  color: yellow;
  background-color: purple;
  padding: 10px;
}
```

## Cores

```css
/* Pelo nome */
color: crimson;

/* Pelo Hexadecimal */
color: #4b1b57;
color: #275;

/* RGB */
color: rgb(110, 0, 0);
color: rgb(199, 161, 114);

/* RGBA */
color: rgba(197, 183, 51, 0.4);

/* HSL */
color: hsl(286, 80%, 35%);
```

# Background


```css
/* Cor do fundo */
background-color: lightblue;

/* Opacidade */
opacity: 0.5;
```

### Imagem

```css
/* Size */
height: 400px;
width: 500px;

/* Fundo com imagem */
background-image: url(../img/image.png);

/* Centralizando */
background-position: center;
background-size: cover;
```

# Text

### Alinhamento de textos

- Pode ser usado em uma div com `center` para alinhar todos os componentes

```css
/* top, bottom, left, right */
text-align: right;

/* start , center , end */
text-align: center;

/* justify, inherit, initial, unset */
text-align: justify-center;
```

### Decoração de texto

```css
/* Removendo underline */
text-decoration: none;
```

### Transformação de texto

```css
/* Uppercase */
text-transform: uppercase;

/* Lowercase */
text-transform: lowercase;

/* Capitalize */
text-transform: capitalize;
```

### Espaçamento de letras

```css
letter-spacing: 14px;
```

## Fontes

- Serif, Sans-serif,  Monospace, Cursive e Fantasy estão disponiveis
- Pode-se adicionar fontes externas com o Google Fonts

```css
/* Alterando a fonte */
font-family: Georgia; /* Serifada */
font-family: Helvetica; /* Sans-serif */
font-family: "Courier New"; /* Monospace */
font-family: cursive;
font-family: fantasy; 
```

### Estilo de Fonte

- Nomal, italic, Oblique

```css
/* italic */
font-style: italic;

/* oblique */
font-style: oblique;
```

### Font Weight

- Cuidado: Algumas fontes não possuem todas as variações
- Podem ser
    - valores de 100 a 900
    - Palavras bold(600)

```css
/* Thin */
font-weight: 100;
font-weight: lighter;

/* bold */
font-weight: 600;
font-weight: bold;

/* Bolder */
font-weight: 900;
font-weight: bolder;
```

### Font Size

```css
font-size: 78px;
```

# Box Model

- Altura e Largura, Padding, Border, Margin;
- Alguns elementos possuem padding e margin por padrão

### Padding

- Espaço interno

```css
padding: 20px;
padding-bottom: 20px; /* também pode ser top, left, right */
```

### Margin

- Espaço externo

```css
margin: 10px;
margin-top: 10px; /* tb pode ser bottom, left, right */
```

### shorthand

- 1 valor: Todos os lados
- 2 valores: Top e Base, Esquerda e Direita
- 3 valores: Top, Esquerda e Direita
- 4 valores: Top, Esquerda, Base e Direita

```css
padding: 20px 10px 30px 5px;
margin: 10px 5px 20px 0px;
padding: 20px 0px;
```

### Border

```css
border: 5px solid #4b1b57;
border-bottom: 5px solid #4b1b57; /* tb pode ser top, left, right */

/* Arredondando a borda */
border-radius: 17px;
```

# Display


### Inline

```css
<div class="inline-box">a</div>
<div class="inline-box">b</div>
<div class="inline-box">c</div>
```

```css
.inline-box{
		display: inline-Block
		
		/* So pra ajudar na visualização */
		width: 50px;
		height: 50px;
		margin: 10px;
		background-color: green;
}
```

### Block

- Span por default é inline

```css
<span class"block">Teste 1</span>
<span class"block">Teste 2</span>
```

```css
.block{
	display: block;
	
	/* So pra ajudar na visualização */
	background-color: #333;
	margin 10px
}
```

### Hidden

Esconde elementos

```css
display: none;
```

# Position

### Position Static

é o valor padrão

### Position Relative

Não é muito usado, pois pode causar sobreposição entre elementos que vem em seguida.

```css
position: relative;
top: 200px;
left: 40px;
```

### Position Absolute

Posiciona em qualquer canto da tela, isso poode ser uma solução ou um problema

```css
position: absolute;
top: 2px;
right: 2px;
```

### Position Relative com Absolute

podemos resolver o problema de absolute com um container relativo

```html
<div class="relative-container">
		<div class="absolute-1"></div>
		<div class="absolute-2"></div>
</div>
```

```css
.relative-container {
	width: 300px;
	height: 300px;
	border 1px solid red;
	position: relative;
}

.absolute-1,
.absolute-2 {
	width: 50px;
	height: 50px;
	background-color: #422;
	position: absolute;
}

.absolute-1 {
	top: 10px;
	left: 10px;
}
.absolute-2 {
	bottom: 10px;
	right: 10px;
}
```

### Position Fixed

Sempre aparece independente do scroll.

```css
position: fixed;
top: 50px;
right: 50px;
```

### Position Sticky

```css
position: sticky;
top: 10px;
```

### Z-index

quanto maior o numero mais pra cima fica na pagina.

```css
z-index: 3;
```