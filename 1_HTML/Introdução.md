# Introdução ao HTML


### Índice

- [Dicas](#dicas)
- [Titulos](#titulos)
- [Paragrafos](#paragrafos)
- [Tags sem conteudo](#tags-sem-conteudo)
- [Comentarios](#comentarios)
- [Atributos](#atributos)
- [Imagens](#imagens)
- [Listas](#listas)
- [Tabelas](#tabelas)
- [Div](#div)

### O que é HTML?

HTML é uma linguagem de marcação que é usada para desenvolver páginas web. É a base de todas as páginas web e é usada para criar a estrutura de uma página web. HTML significa Hyper Text Markup Language.

> [!NOTE]
> Você pode criar uma estrutura HTML rapidamente usando ! + Tab no seu editor de código


### Estrutura de um documento HTML

```html
<!DOCTYPE html>
<html>
<head>
	<title>Titulo da Página</title>
</head>
<body>
	<h1>Meu Primeiro Site</h1>
	<p>Esse é um paragrafo</p>
</body>
</html>
```



### Titulos

```html
<h1> Titulo Grande </h1>
<h2> Titulo Medio </h2>
<h3> Titulo </h3>
<h4> Subtitulo </h4>
<h5> Subtitulo Menor </h5>
<h6> Subtitulo Pequeno </h6>
```

### *Paragrafos*

```html
<p> Aqui jas um paragrafo </p> 
```

### Tags sem conteudo

```html
<br /> <!-- Quebra uma linha -->
<hr /> <!-- Cria uma linha -->
```

### Comentarios

```html
<!-- Esse é um comentarios -->
```

### Atributos

```html
<!-- Link -->
<a hred="https://www.google.com">Google</a> 
<!-- style -->
<body style="padding-bottom:500px" />
<!-- Abrindo link em nova aba -->
<a hred="https://www.google.com" target="_blank">Google</a>
```

### Imagens

```html
<img src="img/city.jpg" />

<!-- Atributo alt descreve a imagem -->
<!-- Ajuda o Google a rankear melhor sua imagem -->
<img src="img/nature.jpg" alt="Noite na floresta"/>
```

### Listas

```html
<!-- Lista não Ordenadas -->
<ul>
		<li> Carro </li>
		<li> Avião </li>
		<li> Caminhão </li>
</ul>

<!-- Lista Ordenadas -->
<ol>
		<li> Carro </li>
		<li> Avião </li>
		<li> Caminhão </li>
</ol>
```

### Tabelas

```html
<!-- 11 - Tabelas -->

<table>
		<tr>
				<th>ID:</th>
				<th>Nome:</th>
				<th>Profissão:</th>
		</tr>
		<tr>
				<td>1</td>
				<td>Anna</td>
				<td>Programadora</td>
		</tr>
		<tr>
				<td>2</td>
				<td>Alex</td>
				<td>Cozinheiro</td>
		</tr>
		<tr>
				<td>3</td>
				<td>Luana</td>
				<td>Editor de video</td>
		</tr>
<table>
```

### Div

```html
<div>
    <h2>Titulo</h2>
    <p>Paragrafo</p>
    <a href="#">Saber Mais</a>
</div>
```