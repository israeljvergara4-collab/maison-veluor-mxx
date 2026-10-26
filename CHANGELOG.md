# Changelog
Formato: [Keep a Changelog](https://keepachangelog.com/es-ES/1.1.0/) · Versionado: [SemVer](https://semver.org/lang/es/)

## [1.0.2] - 2026-10-25
### Corregido
- Las rutas ahora son relativas: el sitio se ve al abrir `index.html` directo, en cualquier servidor o subcarpeta (antes se perdían estilos e imágenes).
- Imágenes sin carga diferida (más fiable en celulares).

## [1.0.1] - 2026-10-25
### Corregido
- Celular: la tarjeta del hero se salía de la pantalla; el botón de WhatsApp tapaba texto (ahora es circular); el carrito se encimaba con el selector Imagen/Pares; la promoción se rompía en varias líneas.

## [1.0.0] - 2026-10-25
### Añadido
- Build de producción: HTML/CSS/JS minificados, sin source maps, archivos con hash de contenido.
- Imágenes extraídas de base64 a archivos `.webp` cacheables, con carga diferida.
- Cabeceras de seguridad (CSP estricta, HSTS, etc.) y política de caché por tipo de archivo.
- Aviso de privacidad (LFPDPPP), política de cookies, términos y envíos/devoluciones.
- Base de datos Supabase con RLS, función `place_order` y Edge Function `create-order`.
- CI/CD con GitHub Actions hacia Cloudflare Pages y Supabase.
