# Diferentes tipos de estilos por pantalla



```css


/*Con @media  podemos poner los distintos estilo en un mismo archivo */
/* print*/
@media print {
	body {
		font: 10pt Times, Georgia, serif;
	}
}

/*screen:*/
@media screen {
	body {
		font: 12pt Verdana, Arial, sans-serif;
	}
}

/* projection:*/
@media projection {
	body {
		font-size: 14pt;
	}
}
```

O en archivos diferentes

```css
/* print.css:*/ 
body {
font: 10pt Times, Georgia, serif;
line-height: 120%;
}

/* screen.css:*/
body {
	font: 12px verdana, arial, sans-serif;
	line-height: 120%;
}

/* projection.css: */
body {
	font: 14px;
	line-height: 120%;
}
```



``` html 
<!-- En el header -->
<link rel="stylesheet" type="text/css" href="/css/print.css" media="print" />
<link rel="stylesheet" type="text/css" href="/css/screen.css" media="screen" />
<link rel="stylesheet" type="text/css" href="/css/projection.css" media="projection" />

```



## Lista de media types

| Media type | Dispositivo                    |
| ---------- | ------------------------------ |
| all        | All devices                    |
| aural      | Speech and  sound synthesizers |
| braille    | Braille                        |
| embossed   | Print Braille                  |
| handheld   | PDA and Smartphone             |
| print      | printers and print previews    |
| projection | projected presentations        |
| screen     | colors monitors                |
| tty        | terminals, teletypes           |
| tv         | televisions and web TV         |

# Organizacion de una hoja de estilo



```css
/* Typography & Colors
------------------------------------ */
[css code ]
/* Structure
------------------------------------ */
[css code ]
/* Headers
------------------------------------ */
[css code ]
/* Images
------------------------------------ */
[css code ]
/* Lists
------------------------------------ */
[css code ]
/* Form Elements
------------------------------------ */
[css code ]
/* Comments
------------------------------------ */
[css code ]
/* Sidebar
------------------------------------ */
[css code ]
/* Common Elements
------------------------------------ */
[css code ]
```

# Hojas de estilo arternativas

```html
<link href="default.css" rel="stylesheet" title="default styles" type="text/css" media="screen" />
<link href="green.css" rel="stylesheet" title="green style" type="text/css" media="screen" />
<link href="blue.css" rel="stylesheet" title="blue style" type="text/css" media="screen" /
```

