# Salón Aurora — terminado

Sitio estático de cuatro páginas: index.html, espacios.html, paquetes.html y contacto.html. Abrir index.html o servir con `python3 -m http.server 8000`.

## Entrega
- Identidad navy/champagne, tipografía editorial, fotos amplias y bokeh CSS con pausa y reduced-motion.
- Responsive, menú móvil con Escape, FAQ nativa y formulario que arma una consulta de WhatsApp al +54 11 5555-1010. El usuario revisa y envía en WhatsApp; no hay backend ni almacenamiento de datos.
- Cinco imágenes generadas con la herramienta integrada imagegen: assets/hero-salon.png, assets/pista.png, assets/candybar.png, assets/jardin.png y assets/mesa.png. Versiones WebP para carga ligera y fallback PNG. Prompts en assets/PROMPTS.md.
- Demo explicitada; sin precios, aforo, dirección, horarios ni servicios garantizados inventados.
- Meta noindex/nofollow en todas las páginas. _headers configura X-Robots-Tag en alojamientos compatibles; el servidor local simple no procesa _headers. robots.txt permite leer la meta noindex.
- Skills leídas: anti-generico, frontend-design, imagegen y web-review. Dirección y referencias en spec.md.

## Verificación realizada
Playwright/Chromium a 390 y 1280 px: ocho recorridos de página, todos sin desborde horizontal, sin imágenes rotas, con un h1 y noindex. Sin errores JavaScript. Capturas en qa/.

Probado: menú móvil, cierre con Escape y retorno de foco; pausa de luces; selección de Quince desde enlace y generación de mensaje de WhatsApp con nombre e invitados. `node --check app.js` correcto.

Revisión visual de inicio en móvil/escritorio y espacios en móvil. Foco visible, etiquetas de campos, enlace de salto y reduced-motion incluidos. No se afirma auditoría exhaustiva de accesibilidad ni entrega efectiva del mensaje al número demo. Fuentes externas de Google con alternativas locales. Sin despliegue y sin operaciones git.
