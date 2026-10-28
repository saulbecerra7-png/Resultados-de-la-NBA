# Resultados NBA — PWA inicial

## Qué incluye
- Interfaz instalable como PWA cuando esté alojada en HTTPS.
- Consulta calendario de los próximos 7 días usando el endpoint público de ESPN.
- Horarios convertidos a America/Santiago.
- Actualización al abrir, al volver a la pestaña y cada 5 minutos mientras está visible.
- Caché de la interfaz para facilitar la carga de la carcasa sin conexión.

## Límites importantes
- El endpoint de ESPN es una fuente de terceros; puede cambiar, limitar solicitudes o dejar de funcionar. No se garantiza disponibilidad.
- La programación de TV/streaming en Chile se deja como “por confirmar”; requiere una fuente separada y verificable.
- La PWA no puede instalarse correctamente abriendo el HTML desde un archivo local. Debe publicarse en un alojamiento HTTPS (por ejemplo, GitHub Pages, Netlify o Cloudflare Pages).
- La caché guarda la interfaz, no promete mostrar un calendario actualizado sin internet.

## Publicación
1. Descomprime el ZIP.
2. Sube `index.html`, `manifest.webmanifest`, `sw.js` e `icon.svg` a un hosting estático HTTPS.
3. Abre la URL en Chrome para Android.
4. Menú ⋮ → “Instalar aplicación” o “Añadir a pantalla de inicio”.

Este es un primer paso funcional, no una app publicada ni una garantía de datos oficiales. Conviene probarlo desde el hosting y revisar que el endpoint responda desde el móvil.
