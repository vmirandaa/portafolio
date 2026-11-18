# Portafolio · Victor Miranda Araya

Sitio personal de **Victor Miranda Araya**, desarrollador front-end.
Maquetación web responsive, landing pages y SEO técnico.

Disponible en español (`/`) e inglés (`/en/`).

## Tecnologías

- HTML5 semántico y accesible
- Sitio bilingüe sin JavaScript, con `hreflang` para SEO internacional
- SCSS (variables, mixins, partials con `@use`)
- CSS Grid y Flexbox, enfoque mobile-first
- Animaciones CSS y [AOS](https://michalsnik.github.io/aos/)
- Formulario de contacto con [Formspree](https://formspree.io) (sin JavaScript propio)
- SEO on-page: meta etiquetas, Open Graph, `sitemap.xml` y `robots.txt`
- Despliegue continuo en Netlify

## Estructura

```
index.html           # versión en español
en/index.html        # versión en inglés
scss/
  main.scss          # une todos los partials
  _variables.scss    # paleta, tipografía, espaciados, breakpoints
  _mixins.scss       # media queries y contenedor
  _base.scss         # reset, botones, accesibilidad
  _header.scss  _hero.scss  _sections.scss
  _about.scss  _services.scss  _projects.scss  _contact.scss  _footer.scss
css/styles.css       # generado por Sass (no editar a mano)
img/
robots.txt
sitemap.xml
```

## Desarrollo local

Requiere [Sass](https://sass-lang.com/install):

```bash
sass --watch scss/main.scss css/styles.css
```

Luego abrir `index.html` con un servidor local (por ejemplo, Live Server en VS Code).
