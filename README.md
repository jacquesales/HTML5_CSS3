# HTML5 & CSS3
Website codificado com a linguagem de marcação HTML versão 5, juntamente com  estilo CSS versão 3.

![](https://i.imgur.com/bWZsb8e.png)



### Projeto Jobs

- [Home Page](https://jacquesales.github.io/ "Home Page")
- [Encontrar vaga](https://jacquesales.github.io/findjobs.html "Encontrar vaga")
- [Modelo de vaga](https://jacquesales.github.io/job.html "Modelo de vaga")
- [Enviar vaga](https://jacquesales.github.io/sendjobs.html "Enviar vaga")
- [Contato](https://jacquesales.github.io/contact.html "Contato")



###### HTML
```html
<!DOCTYPE html>
<html lang="pt-br">
<head>
	<title>Jobs</title>
	<meta charset="utf-8">
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<link rel="stylesheet" type="text/css" href="css_projeto_jobs.css">
	<link href="https://fonts.googleapis.com/css2?family=Cairo:wght@300&family=Open+Sans+Condensed&display=swap" rel="stylesheet">
	<link href="https://fonts.googleapis.com/css2?family=Comic+Neue&display=swap" rel="stylesheet">
	<link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.8.2/css/all.css" integrity="sha384-oS3vJWv+0UjzBfQzYUhtDYW+Pj2yciDJxpsK1OYPAYjqT085Qq/1cq5FLXAZQ7Ay" crossorigin="anonymous">
</head>
```
###### CSS
```css
*{
	margin: 0;
	padding: 0;
	box-sizing: border-box;
}
nav{
	position: fixed;
	top: 0;
	left: 0;
	height: 100px;
	width: 100%;
	z-index: 1;
	background-color: #FFF;
	border-bottom: 1px solid #CCC;
}
nav:after {
	clear: both;
	content: "";
	display: block;
}
.maqescrever{
	animation: blinkCursor 500ms steps(40) infinite, 
	typingText 5s steps(35) 1s normal both;
	animation-iteration-count: infinite;
}
@keyframes blinkCursor{
	from{border-right-color: #BEBEBE;}
	to{border-right-color: transparent;}
}
@keyframes typingText{
	from{width: 0;}
	to{width: 27em;}
}
```
###### Site Responsivo
```css
/*Versão tablet*/
@media screen and (max-width: 768px){
	#logo{
		position: absolute;
		left: 50px;
	}
	.nav-container ul{
		float: none;
		text-align: center;	
		margin-left: 15%;	
		padding: 0;
	}

/*Versão mobile*/	
@media screen and (max-width: 425px){
	.nav-container .btn-menumobile{
		display: block !important;
	.btn-menumobile{
		display: block;
		font-size: 1.75em;
		color: #CCC;
		position: absolute;
		right: 1.5em;
		top: 0.75em;
	}	
	.nav-container ul{
		position: relative;
		top: 4em;
		height: 3em;
		line-height: 3em;
		display: none;
	}
```
