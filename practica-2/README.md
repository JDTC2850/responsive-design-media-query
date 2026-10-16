# Práctica: Distribución de cajas con CSS Grid

## Descripción del proyecto

Este ejercicio muestra cómo organizar ocho cajas numeradas en una cuadrícula usando CSS Grid. Algunas cajas se posicionan explícitamente y se extienden por varias filas o columnas; las demás se acomodan en las posiciones disponibles.

## Estructura de la carpeta

- `index.html`: contiene las ocho cajas y enlaza la hoja de estilos.
- `css/styles.css`: define la cuadrícula, la apariencia de las cajas y la posición de algunos elementos.

## Configuración de la cuadrícula

La clase `.grid-container` activa CSS Grid y define tres columnas de 200 px, cuatro filas de 100 px y una separación de 10 px:

```css
.grid-container {
  display: grid;
  grid-template-columns: repeat(3, 200px);
  grid-template-rows: repeat(4, 100px);
  gap: 10px;
  width: 620px;
}
```

- `display: grid` convierte el contenedor en una cuadrícula.
- `grid-template-columns` y `grid-template-rows` establecen el número y tamaño de las columnas y filas.
- `gap` determina el espacio entre las cajas.

## Posicionamiento de las cajas

En `index.html`, cada elemento tiene una clase de la `a` a la `h`. La hoja de estilos usa estas clases para indicar posiciones y expansiones:

```css
.a {
  grid-row: 1 / 3;
}

.b {
  grid-row: 1 / 3;
}

.c {
  grid-row: 2;
  grid-column: 1;
}

.d {
  grid-column: 2 / 4;
}

.g {
  grid-row: 3 / 5;
  grid-column: 3;
}

.h {
  grid-row: 4;
  grid-column: 1 / 3;
}
```

- `.a` ocupa las dos primeras filas.
- `.b` también ocupa las dos primeras filas y se coloca en una columna disponible.
- `.c` se ubica en la primera columna de la segunda fila.
- `.d` se extiende por las columnas segunda y tercera.
- `.g` ocupa la tercera columna en las filas tercera y cuarta.
- `.h` se extiende por las dos primeras columnas de la cuarta fila.
- Las cajas sin coordenadas explícitas se ubican automáticamente en los espacios disponibles, siguiendo el orden del HTML.

La clase `.box` usa Flexbox para centrar el número horizontal y verticalmente dentro de cada caja.

## Cómo probar la práctica

Abre `index.html` en un navegador. Después, modifica las propiedades `grid-row` y `grid-column` en `css/styles.css` para cambiar la distribución y observa el resultado.

## Ejercicios para practicar

1. Cambia el tamaño de las columnas y las filas.
2. Haz que la caja `.a` ocupe una columna completa.
3. Intercambia la ubicación de las cajas `.g` y `.h`.
4. Agrega una caja y observa cómo CSS Grid la acomoda automáticamente.
5. Prueba `grid-template-areas` para definir una distribución alternativa.

### Recursos

- [Guía de CSS Grid en MDN](https://developer.mozilla.org/es/docs/Web/CSS/CSS_grid_layout)
- [CSS Tricks: A Complete Guide to Grid](https://css-tricks.com/snippets/css/complete-guide-grid/)

---

**Autor:** Generado con ayuda de AI (Copilot)