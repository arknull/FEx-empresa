# FEx-empresa

Este proyecto es la maquetación de una página de una empresa usando html y css.

Se establece la guía para mantener y escalar el proyecto.

## Layout

Es un Layout tradicional, se construye siguiendo el flujo de la página. Se divide en Header, hero, services y contact.

- Header: contiene los links a las secciones del sitio. Es una barra de navegación horizontal.
- hero: tiene el titulo de la página.
- services: contiene card con los servicios que ofrece la empresa.
- contact: contiene informacion adicional de la empresa, como el blog y más servicios.

Se compone a partir de componentes flexibles.

## Variables

Para tener mayor control sobre los colores, los tipos de fuente y el espaciado, se declaran estas propiedades como variables al comienzo del documento CSS dentro de :root

```css
:root {
  /* colors */
  --background-color: #f3f3f3;
  --main-color: #db522f;
  --dark-color: #4c4c4c;
  --text-color: #888889;
  --blue-color: #54708d;
  --green-color: #63a19b;
  --yellow-color: #d7af78;
  /* fonts  */
  --font-family: "Sanchez", serif;
  /* borders  */
  --border-section: 1px solid var(--text-color);
}
```

Para llamar las variables se debe asignar a la propiedad el valor:
`var(--main-font)`

**Todos las propiedades referenciadas deben llamarse por variables.**

## Guía de estilo del código

#### HTML

Se usan etiquetas sintácticas para nombrar los elementos principales: header, main, aside.
Se cuida la indentación y el orden de los elementos siguiendo el flujo de la página.

#### CSS

Las clases se llaman usando la metodología BEM.
`bloque__elemento--modificador`
Las declaraciones se estructuran en el siguiente orden:

- Propiedades del modelo de caja
- Posicionameniento
- Tipografía
- Decoración

```css
.example-element {
  display: block;
  width: 220px;
  height: 40px;
  position: relative;
  font-family: var(--main-font);
  text-transform: uppercase;
  background-color: #333333;
}
```
