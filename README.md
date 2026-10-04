# Plantilla Ixbal · Negocio local

Plantilla madre para negocios locales y de servicios: plomeros, estéticas, talleres, consultorios, despachos.

**Incluye:** hero con llamada a WhatsApp, servicios, nosotros, opiniones, preguntas frecuentes, horario con indicador de “Abierto ahora”, mapa, botón flotante de WhatsApp y datos estructurados para Google.

## Uso

```bash
npm run dev     # servidor local en http://localhost:4321
npm run check   # valida el sitio (sin dependencias)
```

También puedes abrir `index.html` con cualquier servidor estático. No requiere compilación.

## Personalizar

1. **Identidad:** colores y tipografía en `assets/css/tokens.css`.
2. **Contenido:** textos en `index.html`, organizado por secciones.
3. **Imágenes:** reemplaza los archivos de `assets/img/`.

Las reglas de arquitectura y la lista de datos que se repiten están en [AGENTS.md](AGENTS.md).

## Publicar

Es un sitio estático: sirve la raíz del repositorio en GitHub Pages, Netlify, Vercel o AWS Amplify.

> Antes de publicar, convierte `assets/img/og-image.svg` a PNG de 1200 × 630 y usa una URL absoluta en `og:image`: WhatsApp y Facebook no muestran vistas previas en SVG.
