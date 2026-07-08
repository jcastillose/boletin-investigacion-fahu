# Boletín Vicedecanato de Investigación y Postgrado — Facultad de Humanidades USACH

Versión web del Boletín «Cuenta Pública 2024–2026 · Investigación», lista para publicar en un sistema web asociado a GitHub (por ejemplo, **GitHub Pages**).

## Contenido de esta carpeta

```
boletin-fahu-web/
├── index.html        ← el boletín (página principal)
├── support.js        ← runtime que renderiza la página
├── image-slot.js     ← componente de imágenes arrastrables
├── assets/
│   └── logo-fahu.png ← logotipo de la Facultad
└── .nojekyll         ← evita el procesamiento Jekyll de GitHub Pages
```

Todas las rutas son **relativas**, por lo que el sitio funciona tal cual al servirse desde cualquier subcarpeta de un repositorio.

## Cómo publicarlo en GitHub Pages

1. Crea un repositorio en GitHub (por ejemplo, `boletin-investigacion`).
2. Sube el **contenido** de esta carpeta a la raíz del repositorio (o a una carpeta `/docs`).
3. En el repositorio: **Settings → Pages**.
4. En *Build and deployment*, elige *Deploy from a branch*, rama `main` y carpeta `/root` (o `/docs` si lo pusiste ahí).
5. Guarda. En un par de minutos el boletín estará disponible en
   `https://<usuario>.github.io/<repositorio>/`.

## Notas

- **Conexión a internet**: la página carga tipografías (Google Fonts) y el motor de render desde CDN. GitHub Pages sirve el sitio online, así que funciona sin pasos extra.
- **Versión impresa / PDF**: usa el botón «Imprimir / PDF» (arriba a la derecha) o `Ctrl/Cmd + P`. La maquetación de impresión oculta la navegación y muestra los datos en tablas estáticas, legibles sin desplazamiento.
- **Imágenes**: los marcos de imagen del boletín son editables dentro del entorno de diseño; en el sitio publicado se muestran como marcadores hasta que se incrusten las imágenes definitivas.
- **Actualizar**: cada vez que quieras sincronizar cambios, vuelve a exportar esta carpeta y súbela al repositorio (commit + push).
