# Plantilla Ixbal · Negocio local

Plantilla para negocios locales y de servicios del hogar: plomeros, electricistas, impermeabilizadores, talleres y cualquier negocio que atiende a domicilio. El ejemplo es Taller Arce, reparaciones del hogar en la Ciudad de México.

**Incluye:** barra de urgencias, hero con foto y llamada a WhatsApp, garantías, seis servicios con foto y precio de referencia, banda de urgencias 24 h, cómo trabajamos, trabajos recientes, nosotros, zonas de servicio, opiniones, preguntas frecuentes, formulario de cotización por WhatsApp, horario con indicador de “Abierto ahora”, mapa, botón flotante de WhatsApp y datos estructurados para Google.

## Uso

```bash
npm run dev     # servidor local en http://localhost:4321
npm run check   # valida el sitio (sin dependencias)
```

También puedes abrir `index.html` con cualquier servidor estático. No requiere compilación.

## Personalizar

1. **Identidad:** colores y tipografía en `assets/css/tokens.css`.
2. **Contenido:** textos en `index.html`, organizado por secciones.
3. **Imágenes:** cada foto tiene un espacio listado en `imageSlots` de `template.json`; mientras no tenga foto real, muestra una etiqueta con lo que va ahí. Ver [AGENTS.md](AGENTS.md#espacios-de-imagen).

Las reglas de arquitectura y la lista de datos que se repiten están en [AGENTS.md](AGENTS.md).

## Publicar

Es un sitio estático: sirve la raíz del repositorio en GitHub Pages, Netlify, Vercel o AWS Amplify.

> Antes de publicar, convierte `assets/img/og-image.svg` a PNG de 1200 × 630 y usa una URL absoluta en `og:image`: WhatsApp y Facebook no muestran vistas previas en SVG.
