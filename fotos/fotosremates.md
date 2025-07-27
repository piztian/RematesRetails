# 📦 Página de Remates Celucenter - Julio 2025

Esta página muestra los productos en **remate especial de fin de mes**, combinando elementos visuales atractivos con datos dinámicos desde Google Sheets.

---

## ✅ Características

- 🎨 Encabezado tipo Samsung (logo, fondo oscuro, diseño limpio)
- ⏳ Contador regresivo en vivo hasta el **31 de julio a las 23:59:59**
- 🛒 Productos en carrusel dinámico conectados a **Google Sheets** mediante OpenSheet
- 💬 Botón directo a WhatsApp y 📞 botón para llamar
- 💸 Visual con precios tachados, nuevo precio destacado y etiqueta “Remate exclusivo”
- 📱 100% responsive

---

## 📄 Requisitos

- Hoja de Google Sheets con los siguientes encabezados (pestaña `remates`):

| nombre        | imagen                            | precio_original | precio_remate |
|---------------|------------------------------------|------------------|----------------|
| Galaxy A04    | https://...jpg                     | 2899             | 1899           |

- Publicar la hoja como "cualquiera con el vínculo puede ver".
- Obtener el ID de la hoja y colocarlo en el script:

```javascript
fetch("https://opensheet.elk.sh/YOUR_SHEET_ID/remates")
  
