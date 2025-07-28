# 🛒 Página de Remates con Tarjetas – Celucenter

Este archivo HTML (`remates-tarjetas.html`) muestra dinámicamente los productos en remate, con diseño tipo tarjeta, conectando directamente con una hoja de Google Sheets.

---

## ✅ Características principales

- Diseño estilo "vitrina", tipo tarjeta moderna (como catálogo de sucursales)
- Muestra: nombre de sucursal, modelo, imagen, precio original y remate
- Botón dinámico que redirige a WhatsApp de la sucursal (desde columna `Walinks`)
- Responsive: se adapta automáticamente a 1, 2 o 3 columnas
- Conecta directo a Google Sheets vía [OpenSheet](https://opensheet.elk.sh)

---

## 📄 Estructura esperada en la pestaña `ListaRemates`

| nombre       | modelo     | imagen (URL) | precio_original | precio_remate | Walinks (wa.link) |
|--------------|------------|--------------|------------------|----------------|--------------------|
| Atequiza     | Modelo 1   | https://...  | 3799             | 2499           | https://wa.link/... |
| Tuxpan       | Modelo 3   | https://...  | 4599             | 2999           | https://wa.link/... |

> ⚠️ Asegúrate que el encabezado `modelo` esté en minúsculas, sin espacios

---

## 🛠 Configuración del archivo

- URL del catálogo (Google Sheets):  
  `https://opensheet.elk.sh/1WJ42ee790_Z_DxId96Ms6Be_s8g3XQJ_1DqBtRJlMnk/ListaRemates`
  
- El script lee directamente la columna `Walinks` para el botón WhatsApp.

- Si el `wa.link` está vacío o es “N/A”, el botón queda inactivo.

---

## 🌐 Publicación sugerida

Puedes alojar este HTML en:

- GitHub Pages (ej: `https://piztian.github.io/RematesRetails/remates-tarjetas.html`)
- Bitrix24 Sites
- Tu propio hosting web

---

## 🧠 Recomendaciones

- Usar `IFERROR(VLOOKUP(...), "N/A")` en la columna `Walinks` para traer los enlaces automáticamente desde otra pestaña.
- Verifica que las imágenes estén en formato `.jpg` o `.png` accesible públicamente (por ejemplo desde GitHub raw).
- Puedes editar los estilos para mostrar etiquetas, stock, promociones o envío gratis.

---

## ☎️ Contacto de atención

Atención general de Celucenter: `3321012446`

---

> 📌 Archivo relacionado: `walinkremates.html` para redirección rápida a WhatsApp
