# Selectores en CSS



## Formas de agregar estilos al HTML

Estos son apuntes obtenidos del libro `Cookbook CSS de O'Relly`

La etiqueta basica para enlazar `css` con `html` es :

```html
<style type = "text/css" >
<!--
    Contenido css de nuestra pagina
    -->
</style>
```

 Esta etiqueta se suele colocar en el head de nuestro `html`.

### 1. Documento `index.html` con `css` embebido:

con este ejemplo mostraremos todos los selectores basicos:

```html
<html>
<head>
	<title>CSS Cookbook</title>
	<style type="text/css">
	
        	* {
				font-family: verdana, arial, sans-serif;
			}
        
			body {
				font-family: verdana, arial, sans-serif;
			}
        
        	#navigation {
				border: 1px solid black;
				padding: 40px;
			}
        	
        	.warning {
				font-weight: bold;
			}
        
        	li a {
					text-decoration: none;
			}
        
            h1 {
            	font-size: 120%;
            }
            a {
            	text-decoration: none;
            }
            p {
           		font-size: 90%;
            }
        
        	strong {
				text-decoration: underline;
			}
        
			div > strong {
				text-decoration: none;
			}
        
        	li + li {
				font-size: 200%;
			}
        	a[href="csscookbook.com"] {
				text-decoration: none;
			}
   
	</style>
    
</head>
<body>
	<h1>Title of Page</h1>
	<p>This is a sample paragraph with a
		<a href="http://csscookbook.com">link</a>.
        <em class="warning">aliquam erat volutpat</em>.
         Nothing happens to this part of the sentence because this
		<strong>strong</strong> isn't the direct child of div.
    </p>
  
    <div>
        However, this <strong>strong</strong> is the child of div.
        Therefore, it receives the style dictated in the CSS rule.
    </div>
    
    <ul id="navigation">
		<li><a href="http://csscookbook.com">Apples</a></li>
		<li><a href="http://csscookbook.com">Bananas</a></li>
		<li><a href="http://csscookbook.com">Cherries</a></li>
	</ul>
</body>
</html>
```



### 2. Enlazandro archivo css (Enlazados o importados)

```html
<link rel="stylesheet" type="text/css" href="/css/estilos.css" media="screen" />
```

Con el atributo `href= 'ruta_archivo.css` dentro de la etiqueta `link` podemos enlazar archivos externos `.css`.

Este enlace tambie se debe colocar en el `<head>`

### 3. Estilos en linea directa con html (En linea)

```html
<p style="font-color: blue">Test goes here.</p>
```



### 4. Reglas para aplicar los estilos CSS

Los siguientes son una guia para tratar de determinar como resuelve los conflictos de estilos usando las reglas de CSS:
The user’s own styles take priority over browser styles.

1. Los estilos del usuario tienen prioridad sobre los estilos del buscador que use.
2. Los estilos del autor de la pagina tienen prioridad sobre los estilos del usuario.
3. Los estilos embebidos tienen prioridad sobre los estilos enlazados o importados.
4. Lo estilos en linean tienen prioridad sobre los embebidos, enlazados o importatos. 

Con `!important` puedes forzar ciertas reglas que tomen mayor prioridad que otras.

```css
p {
	font-size: 12px !important;
}
```

# Sintaxis de los selectores

```css
selector {
    propiedad: valor ;
    property: value, value, value;
	property: value value value value;
}
```



## 1. Selector por nombre de etiqueta:

```css
h1 {
    font-size: 120%;
}

/* 
 	Los selectores son h1 y p.
	El ; al final de una propiedad es obligatorio.
*/
 p {
      font-size: 90%;
}
```

> Propiedad `font-size: 120%` se refiera a un texto mas largo o grande que el tamano por defecto.
>
> Propiedad `font-size: 90%` se refiera a un texto mas pequeno  que el tamano por defecto.

Es tipo de selector no es muy especifico, si tienes varias etiquetas `h1` todas se veran afectadas por los estulos.

## 2. Selector por ID:

```css

/* El caracter # seguido por el ID navigation es el selector*/

#navigation {
	border: 1px solid black;
	padding: 40px;
}
```

```html
<ul id="navigation">
	<!-- Elementos html dentro del ul -->
</ul>
```

El ID de un elemento html debe ser unico dentro de la estructura del DOM. Si quieres aplicar a estilos a un elemento en especifico lo puedes hacer por medio del ID.  

## 3. Selector decendente:

```css
/*Tomamos los elementos "a" que se encuentran dentro de los elementos "li" */
li a {
	text-decoration: none;
}
```

```html

<li ><a href="http://csscookbook.com">Apples</a></li>
<li><a href="http://csscookbook.com">Bananas</a></li>
<li><a href="http://csscookbook.com">Cherries</a></li>

```

En nuestro ejemplo tenemos tres elementos `<li>` que dentro tienen un elemento `<a>` cada uno. Estos serian los seleccionados para aplicarle los estilos.

## 4. Selector universal *

```css
* {
	font-family: verdana, arial, sans-serif;
}
/* 
	El selector universal se representa con un asterisco (*), significa que todos los elementos se		aplicara este estilo 
*/
```

## 5. Selectores de "padre > hijo"

```css
 
div > strong {
	text-decoration: none;
}
```

```html
 <div>
        However, this <strong>strong</strong> is the child of div.
        Therefore, it receives the style dictated in the CSS rule.
 </div>
```



## 6. Selectores de "hermano + hermano"

```css
li + li {
	font-size: 200%;
}
```

Seleccion los `li` que esten siguiente el uno al otro:

```html
<!-- Este elemento NO entra en la regla de hermanos, no tiene elementos li antes-->
<li><a href="http://csscookbook.com">Apples</a></li>

<!-- Solo estos dos elementos obtienen estilos por la regla de hermanos -->
<li><a href="http://csscookbook.com">Bananas</a></li>
<li><a href="http://csscookbook.com">Cherries</a></li>
```



## 7. Selectores por atributos

```css
a[href="csscookbook.com"] {
	text-decoration: none;
}
```

```html

<li ><a href="http://csscookbook.com">Apples</a></li>
<li><a href="http://csscookbook.com">Bananas</a></li>
<li><a href="http://csscookbook.com">Cherries</a></li>
```

Los selectores por atributos tienen varias caracteristicas interesantes que vale la pena  conocer.

```css
/* Estos selectores nos permiten encontrar coincidencias */

a[title~="tv hd digital"] {
	text-decoration: none;
}

a[title|="anti"] {
	color: red;
}

a[href^="mailto:"] {
	padding-right: 15px;
	background: url(icon-email.png) no-repeat right;
}

a[href$='.rss'], a[href$='.atom'] {
	padding-right: 15px;
	background: url(icon-rss.png) no-repeat right;
}

a[href *="username"] {
	padding-right: 15px;
	background: url(icons-star.png) no-repeat right;
}
```

La mejor forma de entender estos selectores es probandolos por ti mismo. Te recomiendo probar cada uno de estos ejemplos anteriores y ver que cambios probocan en tu pagina. 

## 8. Selectores por clase .

```css
.warning {
	font-weight: bold;
}
```

El protagonista de las clases es el punto `.` Las classes no tienen que ser unicas como los ID.  Puedes aplicar varias clases a un mismo objeto solo tienes que separarlas con espacios `class= "btn warning"` esta aplica a dos clases una `.btn` y la otra `.warning`.

```html
 <em class="warning">aliquam erat volutpat</em>
```

# HTML 5 etiquetas divisoras que replazan los `div`

> - `<header>`
> - `<nav>`
> - `<section>`
> - `<article>`
> - `<aside>`
> - `<footer>`

```css
/*Es recomendable colocar estos elementos como bloques en el estilo*/
header, section, nav, aside, footer {
	display: block;
}
```

