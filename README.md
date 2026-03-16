# ◈ GameVault — Catálogo de Videojuegos

Un catálogo web de videojuegos construido con **Astro**. Permite explorar juegos, filtrar por género y buscar títulos específicos.

## Descripción

GameVault es una página web estática que muestra un catálogo de videojuegos destacados. El usuario puede:

- Ver todos los juegos en una grilla responsive
- Filtrar juegos por género (Acción, RPG, Puzzle, etc.)
- Buscar juegos por nombre en tiempo real
- Ver el juego mejor puntuado en la sección "Destacados"

## Herramientas usadas

| Herramienta | Para qué se usó |
|---|---|
| [Astro](https://astro.build/) | Framework principal del sitio |
| HTML semántico | Estructura (`<header>`, `<nav>`, `<section>`, `<article>`, `<footer>`) |
| CSS personalizado | Variables CSS, Grid, Flexbox, responsive design |
| JavaScript vanilla | Filtrado de juegos, búsqueda en tiempo real, menú mobile |
| Google Fonts | Tipografías Syne y DM Sans |

## Estructura del proyecto

```
game-catalog/
├── public/
│   └── favicon.svg
├── src/
│   ├── components/
│   │   ├── Header.astro      # Barra de navegación con menú mobile
│   │   ├── GameCard.astro    # Tarjeta reutilizable para cada juego
│   │   └── Footer.astro      # Pie de página
│   ├── layouts/
│   │   └── Layout.astro      # Layout base con <head> y fuentes
│   ├── pages/
│   │   └── index.astro       # Página principal
│   └── styles/
│       └── global.css        # Estilos globales y variables CSS
├── astro.config.mjs
├── package.json
└── README.md
```

## Instrucciones para ejecutarlo

### Requisitos previos

- [Node.js](https://nodejs.org/) versión 18 o superior

### Pasos

1. **Clonar el repositorio**
   ```bash
   git clone https://github.com/tu-usuario/game-catalog.git
   cd game-catalog
   ```

2. **Instalar dependencias**
   ```bash
   npm install
   ```

3. **Iniciar el servidor de desarrollo**
   ```bash
   npm run dev
   ```
   El sitio estará disponible en `http://localhost:4321`

4. **Generar la versión de producción** (opcional)
   ```bash
   npm run build
   npm run preview
   ```

## Características

- **Responsive**: Funciona en celular, tablet y desktop
- **Filtrado por género**: Botones interactivos que muestran solo los juegos del género seleccionado
- **Búsqueda en tiempo real**: El campo de búsqueda filtra los juegos mientras escribís
- **Componentes reutilizables**: `GameCard` se puede usar para cualquier juego solo pasándole los datos
- **HTML semántico**: Uso correcto de `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<footer>`
