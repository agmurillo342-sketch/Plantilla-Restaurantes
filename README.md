# Plantilla para sitios de negocios locales

Base estática en **HTML, CSS y JavaScript vanilla**, inspirada en la estructura y el pulido visual del proyecto de Restaurante El Playón. Se limpió el contenido propio de El Playón: no quedan sus datos, menú, ubicación ni horarios. Personaliza cada sitio con el objeto `SITE` al final de `index.html`.

## Arranque rápido

1. Duplica este repositorio para cada cliente.
2. Abre `index.html` y busca `const SITE =`.
3. Sustituye todos los textos entre corchetes y los ejemplos por información confirmada con el negocio.
4. Ajusta los tokens de color, tipografía y radio al inicio del bloque `<style>`.
5. Cambia las cuatro imágenes por fotos propias aprobadas y añade el enlace de contacto correcto.
6. Abre `index.html` en un navegador y prueba navegación, filtros, búsqueda, enlaces y vista móvil.
7. Sube el proyecto a GitHub y en Vercel importa el repositorio. No hay compilación: deja el framework como **Other** y usa la raíz como directorio.

## Qué configurar

- **Identidad:** `name`, `initials`, `location`, título, descripción SEO, textos principales y CTA.
- **Diseño:** variables CSS `--ink`, `--paper`, `--surface`, `--brand`, `--accent`, `--display`, `--body` y `--radius`.
- **Imágenes:** `images.hero`, `images.story` y hasta cuatro `images.gallery`. El ejemplo carga imágenes remotas de Unsplash; para producción, usa imágenes con permiso y preferentemente optimizadas.
- **Oferta:** cambia `categories` y `items`. Puedes llamar la sección “Menú”, “Servicios”, “Tratamientos”, “Habitaciones”, etc. Cada elemento usa `category`, `name`, `description` (opcional) y `price`.
- **Contacto:** `contactUrl`, `address`, `hours`, `phone` y `mapEmbed`. Para el mapa, pega solamente el valor `src` del iframe de Google Maps; si se deja vacío, el mapa se oculta.
- **Secciones:** actualiza nombres del menú y encabezados para el rubro. Si una sección no aporta a la decisión del cliente, quita su bloque HTML y el JavaScript asociado; no dejes una sección de relleno.

## Qué conviene conservar y qué adaptar

**Conserva** el encabezado móvil, el CTA visible, la jerarquía del hero, el patrón de contenido breve, el buscador/filtros cuando la oferta sea larga, el contacto claro, metadatos básicos, estados accesibles y animaciones discretas. Son piezas funcionales que reducen fricción.

**Adapta por cliente** paleta, fuentes, forma de las imágenes, palabras, orden de secciones, argumentos de venta, categorías y CTA. Investiga el negocio y confirma datos, horarios y precios antes de publicar.

**Elimina** cualquier bloque que no tenga contenido verdadero o utilidad en ese sitio. Para un profesional de servicios quizá no se necesita menú filtrable; para un alojamiento, reemplaza productos y precios por tipos de habitación y disponibilidad; para una tienda, destaca catálogo y compra. Reutiliza la estructura, no la identidad visual completa: cambiar solo el nombre y el color hace que todos tus sitios parezcan la misma plantilla.

## Animaciones y accesibilidad

Incluye intro de marca, revelado al entrar en pantalla, transición de navegación y microinteracciones. Respeta `prefers-reduced-motion`. Mantén textos legibles, alt de imagen específico y etiquetas útiles. Quita o acorta la intro si ralentiza el acceso al contenido en equipos lentos.

## Límites

- No hay framework, proceso de build, backend, carrito, reservaciones conectadas ni CMS.
- Las fuentes e imágenes de ejemplo necesitan internet. Sustituye las imágenes de muestra antes de entregar a un cliente.
- El buscador y filtros corren en el navegador sobre los elementos escritos manualmente.
- Verifica privacidad, permisos de fotos y exactitud de la información con cada cliente.
