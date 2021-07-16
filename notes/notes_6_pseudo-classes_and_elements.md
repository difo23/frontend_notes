# Usando Pseudo-classes ":"

```css
a:link {
	color: blue;
}
a:visited {
	color: purple;
}
a:hover {
	color: red;
}
a:active {
	color: gray;
}
```

Las Pseudo-classes nos permiten crear ciertos efectos sobre nuestros elementos html. Aqui debajo te dejo una lista de los efectos que puedes estilizar con esta herramienta. Estas Pseudo-classes pueden no funcionar en ciertos navegadores, asi que ten cuidado al usarlas. 

> `:target` 
> `:enabled` 
> `:disabled` 
> `:checked` 
> `:default`
>
> ``:valid
> :invalid
> :in-range
> :out-of-range`` 
>
> `:nth-child()` 
> `:nth-last-child()` 
> `:nth-of-type()`
> `:required`
> `:root` 
> `:not()` 
> `:nth-last-of-type()`
> `:last-child`
> `:first-of-type`
> `:last-of-type`
> `:only-child`
> `:only-of-type`
> `:empty`

# Usando Pseudo- Elements "::"

Nos sirven para introducir ciertos aspectos a nuestros elementos sin agregar nuevo codigo html  como un elemento **span**.

```css
p::first-letter {
	font-size: 200%;
	font-weight: bold;
}
```

Los Pseudo-Elments son:

> - ::first-letter 
> -  ::first-line 
> -  ::before 
> -  ::after