# 🎨 Colores de fondo · CSS Grid

_"El color no tiene fronteras, pero sí columnas."_

----------

## 📖 Descripción

Este proyecto forma parte de un ejercicio de maquetación donde el objetivo es practicar **CSS Grid** para crear diseños **responsive**.

El reto era reproducir una paleta de colores que se reorganiza de forma diferente en móvil, tablet y escritorio — sin que ninguna celda se rompa ni se salga de su sitio.

Solo con **HTML** y **CSS**, **CSS Grid** y fuentes de **Google Fonts**.

----------

## 🔍 Análisis

Antes de escribir código analicé los tres diseños para identificar qué elementos HTML necesitaba y cómo cambia el número de columnas según el dispositivo.

**Lo que veo en la imagen:**

-   Un `<h1>` con el título "Colores de fondo"
-   Un `<h2>` con el subtítulo "Colores"
-   Una `<section>` que contiene todo el grid
-   Dentro del grid, 16 celdas — cada una es un `<div>` con el nombre del color:
    -   `Colors` → siempre ocupa el ancho completo
    -   14 celdas normales de igual tamaño
    -   `green` → ocupa más espacio que el resto en desktop


**Cómo cambia el grid entre dispositivos:**

| Dispositivo | Columnas | `Colors` | `green` |
|---|---|---|---|
| 📱 Phone | 3 | span 3 — ancho completo | span 3 — ancho completo |
| 📟 Tablet | 4 | span 4 — ancho completo | span 4 — ancho completo |
| 🖥️ Desktop | 6 | span 6 — ancho completo | span 3 — mitad del grid |

----------

## 📐 Planificación

Estructura de archivos decidida antes de programar:

-   **`index.html`** — marcado semántico
-   **`styles/`** — CSS dividido por responsabilidad:
    -   `styles.css` → punto de entrada, solo `@import`
    -   `variables.css` → colores, fuentes y espaciado
    -   `base.css` → reset y estilos globales
    -   `layout.css` → contenedor principal, títulos y grid
    -   `cells.css` → color y estilo de cada celda
-   **`assets/imgs/`** — capturas del diseño de referencia

Cada archivo CSS tiene su propia rama en Git para mantener un historial limpio y ordenado.

----------


## 🎨 Prototipo

Diseño de referencia proporcionado por el bootcamp.

| 📱 Phone | 📟 Tablet | 🖥️ Desktop |
|---|---|---|
| ![Phone](imgs/01-grid-colors-phone-600.png) | ![Tablet](imgs/01-grid-colors-tablet-900.png) | ![Desktop](imgs/01-grid-colors-desktop.png) |

----------

## 📋 Planificación de commits

-   `chore`: add .gitignore
-   `docs`: rename original README to README-original.md
-   `docs`: add README
-   `feat`: add project folder structure
-   `feat`: add semantic HTML markup
-   `style`: add CSS variables and Google Fonts (Bitcount Single)
-   `style`: add base styles and reset
-   `style`: add grid layout mobile-first (3 columns)
-   `style`: add tablet layout (4 columns)
-   `style`: add desktop layout (6 columns)
-   `style`: add color cells styles
-   `docs`: add final screenshot to README

----------

## 🛠️ Tecnologías

- VS Code
- HTML5
- CSS3 — Grid, variables, media queries
- Google Fonts — Bitcount Single
- Git & GitHub

----------

## 📸 Resultado final

_Captura añadida al terminar el proyecto._

----------

## 🚀 Demo en vivo

👉 [Ver en GitHub Pages](https://jennydev-25.github.io/ex-html-css-frontend-reproduce-using-grid/)