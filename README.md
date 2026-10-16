# Práctica: Responsive Design con CSS Grid

## Descripción del Proyecto
Esta carpeta contiene un ejemplo de diseño web responsivo utilizando CSS Grid y media queries. El objetivo es mostrar cómo adaptar la estructura de una página a diferentes dispositivos (escritorio, tablet y móvil) de manera eficiente y moderna.

## Estructura de la Carpeta
- `index.html`: Estructura HTML principal de la página.
- `css/styles.css`: Archivo de estilos donde se implementa CSS Grid y las media queries para la adaptación responsiva.

## ¿Cómo funciona el código?
El contenedor principal `.contenedor` utiliza CSS Grid para organizar las diferentes secciones de la página (`header`, `contenido`, `sidebar`, `widget-1`, `widget-2`, `footer`).

Se definen diferentes áreas de grid para cada sección y se usan media queries para modificar la disposición según el tamaño de pantalla:
- En escritorio, el layout es más complejo y aprovecha varias columnas y filas.
- En tablet, las áreas se reorganizan para mayor legibilidad y facilidad de uso.
- En móvil, cada sección ocupa el 100% del ancho y se apilan verticalmente.

## ¿Qué son las Media Queries?
Las media queries son reglas de CSS que permiten aplicar estilos diferentes según las características del dispositivo, como el ancho de la pantalla. Se usan para crear diseños responsivos que se adapten a cualquier dispositivo.

Ejemplo:
```css
@media screen and (max-width: 768px) {
  /* Estilos para tablets */
}

@media screen and (max-width: 400px) {
  /* Estilos para móviles */
}
```

### Ventajas de las Media Queries
- Permiten adaptar el diseño a cualquier dispositivo.
- Mejoran la experiencia de usuario.
- Facilitan el mantenimiento del código.

## ¿Qué es Mobile First?
Mobile First es una filosofía de diseño donde se comienza creando la versión móvil de un sitio web y luego se agregan mejoras para pantallas más grandes usando media queries. Esto asegura que la experiencia en dispositivos móviles sea óptima y que el sitio sea accesible para todos los usuarios.

### Ventajas de Mobile First
- Prioriza la velocidad y la usabilidad en móviles.
- Reduce la sobrecarga de estilos innecesarios.
- Facilita la escalabilidad del diseño.
- Mejora el SEO y la accesibilidad.

## Ejercicios para Practicar
1. **Agrega una nueva sección** llamada `noticias` y haz que solo aparezca en pantallas de escritorio.
2. **Cambia el orden** de los widgets en móvil para que `widget-2` aparezca antes que `widget-1`.
3. **Haz que el sidebar desaparezca** en pantallas menores a 500px usando media queries.
4. **Crea un layout alternativo** para tablets donde los widgets estén uno al lado del otro y el sidebar debajo del contenido.
5. **Implementa Mobile First:** Reescribe los estilos para que el diseño base sea móvil y uses media queries solo para mejorar la experiencia en pantallas más grandes.

---

**Autor:** Generado con ayuda de AI (Copilot)


