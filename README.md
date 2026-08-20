# Portafolio Web – Iván Tapia Valdés

Sitio web personal desarrollado con **HTML5**, **CSS3** y **Bootstrap 5**, como parte del curso de Desarrollo Web en Coderhouse.

## 📁 Estructura del proyecto

```
├── index.html
├── css/
│   └── styles.css          # CSS compilado (NO editar a mano)
├── scss/
│   ├── main.scss           # único punto de entrada (@use)
│   ├── utilities/
│   │   ├── _variables.scss
│   │   └── _mixins.scss
│   ├── base/
│   │   ├── _base.scss
│   │   └── _tipografia.scss
│   ├── layout/
│   │   ├── _nav.scss
│   │   ├── _header.scss
│   │   └── _footer.scss
│   └── components/
│       ├── _buttons.scss
│       ├── _cards.scss
│       ├── _badges.scss
│       ├── _carousel.scss
│       ├── _forms.scss
│       └── _grids.scss
├── assets/
│   └── (imágenes: logo, carrusel, secciones)
└── pages/
    ├── sobre-mi.html
    ├── proyectos.html
    ├── servicios.html
    └── contacto.html
```

## 🎨 Arquitectura SCSS

Los estilos se escriben exclusivamente en `scss/` mediante partials (archivos con `_`) y se compilan a un único `css/styles.css`. `main.scss` es el punto de entrada y usa `@use` para importar cada módulo.

Para compilar (requiere `sass` instalado, `npm install -g sass`):

```bash
sass scss/main.scss css/styles.css --style=expanded
# o en modo watch durante desarrollo:
sass --watch scss/main.scss:css/styles.css
```

## 🚀 Tecnologías utilizadas

- HTML5 semántico
- Sass/SCSS (variables, partials, nesting, `&`, mixins, `@use`)
- Bootstrap 5.3 (navbar, cards, carousel, modal, formularios)
- Google Fonts (Poppins)
- Diseño mobile-first y responsivo

## 📱 Responsividad

- **Index**, **Sobre mí** y **Servicios/Contacto** están completamente adaptados a mobile y desktop mediante breakpoints en 768px y 1024px.
- El resto de las páginas cuenta con contenido y estilos aplicados sobre el mismo sistema de grillas.

## 🌐 Sitio desplegado

https://github.com/IvanTapiaValdes/portafolio-ivantapia

## 👤 Autor

Iván Tapia Valdés
