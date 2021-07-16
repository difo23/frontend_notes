---
title: "Curso frontend developer - platzi"
day: "4"
publishDate: "2021-06-19"
thumbnailImage: ""
shareText: " Description:  "
hashtags: ['learn', 'frontend', 'html', 'css']
draft: false

---

## OOCSS, BEM, SMACSS, ITCSS y Atomic Design

| Source:      | [URL Platzi](https://platzi.com/clases/1640-frontend-developer/) |
| ------------ | ------------------------------------------------------------ |
| **Course:**  | Curso frontend developer - platzi                            |
| **Teacher:** | Estefany Agilar                                              |



**OOCSS**
css orientado a objetos. Separa el diseño del contenido, así podemos reutilizar nuestro código

```css
// ejemplo, en vez de para cada elemento una clase.
.globalWidth {
	width: 100%;
}
```

**BEM**
Block Element Modifier. Separa los elementos y los modificadores

```css
.header {}  // bloque
.header__button--red {} // block, element, modifier
```

**SMACSS**
Scalable and Modular Arquitecture for CSS. Arquitectura de css escalable y modular. PAra eso se realizan cinco pasos

1. Dividir nuestro css en componentes base
2. Definir Layout. Elementos que se utilizan solo una vez. ej. Footer, Header
3. Definir Modulos. Componentes que se usan mas de una vez
4. Definir Estados. Estos estados definen los cambios que existen en nuestros elementos/componentes. ej. Cambio de color cuando hacen hover
5. Definir Temas. Separar los temas y sus cambios. Si tuvieras temas

**ITCSS**
Inverted Triangle CSS. Triangulo Invertido de CSS. Lo que nos indica esta metodologia es poder dividir todos nuestros archivos de css en ciertas partes para que no se mezclen.
Triangulo invertido, desde arriba hacia abajo:

- Ajustes
- Herramientas
- Generico
- Elementos
- Objetos
- Componentes
- Utilidades

Especificidad: elementos o clases con mayor peso que otros.
Magnitud
Claridad

Atomic Design
Basados en la quimica.
Atomos < Moleculas < Organismos < Templates < Paginas

La eleccion de la metodologia depende del proyecto y del equipo

Anotacion: No es tan buena practica usar !important



## ¿Qué es un componente? Analicemos nuestros diseños

StoryBooks, logra una documentación amigable y visual. Se experimenta como tener una librería de nuestros componentes.
https://storybook.js.org/docs/basics/introduction/ documentación
https://www.youtube.com/watch?v=va-JzrmaiUM cómo isntalar StoryBook

Profesor enseñando Storybook Sacha:
[STORYBOOK: LA MEJOR HERRAMIENTA PARA USAR](https://www.youtube.com/watch?v=lA-4Hz9N7qA)
[Storybook: Instalación y Primeros Pasos](https://www.youtube.com/watch?v=WgsaTWmzvFE)

## Lectures

[An Introduction To Object Oriented CSS (OOCSS)](https://www.smashingmagazine.com/2011/12/an-introduction-to-object-oriented-css-oocss/)

[Why BEM over the others?](http://getbem.com/introduction/)

[SMACSS (pronounced “smacks”) ](http://smacss.com/)

[ITCSS: Scalable and Maintainable CSS Architecture](https://www.xfive.co/blog/itcss-scalable-maintainable-css-architecture/)

[atomic design](https://bradfrost.com/blog/post/atomic-web-design/)

[Flexbox vs Grid](https://platzi.com/blog/flexbox-vs-css-grid-cual-es-la-diferencia/) 

[Flex Guide](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)

[icons](https://iconos8.es/icons/set/learning)

