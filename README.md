<div align="center">

<img src="docs/logo.svg" width="90" alt="MenosEspacioPDF logo"/>

# MenosEspacioPDF

**Menos peso. La misma calidad.**

Herramientas PDF que corren **100% en tu navegador**. Nada se sube a ningún servidor: tus archivos nunca salen de tu dispositivo.

[![Demo](https://img.shields.io/badge/🌐_Probar_ahora-Demo_en_vivo-5EEAD4?style=for-the-badge)](https://TU-USUARIO.github.io/menosespaciopdf/)
[![Licencia MIT](https://img.shields.io/badge/Licencia-MIT-38BDF8?style=flat-square)](LICENSE)
[![Sin backend](https://img.shields.io/badge/Backend-Ninguno-34D399?style=flat-square)](#-privacidad)
[![Idiomas](https://img.shields.io/badge/Idiomas-ES_·_EN_·_PT-FBBF24?style=flat-square)](#-idiomas)

*Funciona en Windows, Linux, macOS, Android y iPhone. Solo necesitas un navegador.*

</div>

---

## ✨ ¿Qué la hace diferente?

La mayoría de compresores de PDF te dan un botón de "comprimir" y ya. **MenosEspacioPDF te pregunta cuánto quieres comprimir**:

> 📄 *Tu archivo pesa 3.4 MB…*
> **¿Cuánto quieres comprimirlo?**
> · 2 MB menos → quedaría en ~1.4 MB
> · 1 MB menos → quedaría en ~2.4 MB
> · Llevar a ~900 KB *(ideal para enviar por correo)*
> · Compresión máxima

Las opciones se **adaptan al peso real del archivo** (pasos en MB para archivos grandes, en KB para pequeños). Puedes aplicar hasta 6 pasadas, y cuando técnicamente ya no hay margen, la página te lo dice con honestidad:

> ⚠️ *Ya no se puede comprimir más, el archivo está a su máximo de compresión.*

## 🧰 Herramientas

| Herramienta | Estado | Qué hace |
|---|---|---|
| 🗜️ **Comprimir PDF** | ✅ | Flujo conversacional con objetivo de peso y hasta 6 pasadas |
| 🔗 **Unir PDF** | ✅ | Combina varios PDF en uno, en el orden que elijas |
| ✂️ **Dividir PDF** | ✅ | Extrae un rango de páginas |
| 🔄 **Girar PDF** | ✅ | Rota todas las páginas 90°, 180° o 270° |
| 🖼️ **Imágenes a PDF** | ✅ | JPG/PNG/WebP → un PDF, cada imagen una página |
| 📷 **PDF a imágenes** | ✅ | Cada página como JPG en alta calidad (ZIP si hay varias) |
| 🔢 **Números de página** | ✅ | Numeración con posición y número inicial configurables |
| ✏️ Editar / 🔒 Proteger / ✍️ Firmar | 🔜 | En desarrollo |

## 🔒 Privacidad

Este proyecto **no tiene backend**. Toda la lógica (renderizado, compresión, unión, división) se ejecuta con JavaScript en tu propio dispositivo usando [pdf.js](https://mozilla.github.io/pdf.js/) y [pdf-lib](https://pdf-lib.js.org/).

- 🚫 Tus archivos **nunca** se suben a un servidor
- 🚫 Sin cuentas, sin registro, sin cookies de rastreo
- 🚫 Sin anuncios
- ✅ Código abierto: puedes leer exactamente qué hace

## 🌍 Idiomas

La interfaz detecta el idioma de tu navegador automáticamente:

- 🇪🇸 Español · 🇺🇸 English · 🇧🇷 Português

También puedes cambiarlo manualmente con el botón 🌐 de la barra superior.

## 🎨 Características de la interfaz

- Modo **oscuro / claro** con transición suave (recuerda tu preferencia)
- Diseño *futurista calmado*: azul profundo, acentos menta/cian, líneas finas
- Animaciones y micro-interacciones (pulso en la zona de carga, tarjetas con elevación)
- Totalmente **responsive**: escritorio, tablet y móvil
- Arrastrar y soltar + selector de archivos + botón para Google Drive

## 🚀 Usar / Desplegar

Es **un solo archivo** (`index.html`). No hay build, no hay dependencias que instalar.

**Localmente:** descarga `index.html` y ábrelo en tu navegador. Listo.

**Tu propia copia en GitHub Pages:**
1. Haz *fork* de este repositorio (o súbelo al tuyo)
2. Ve a **Settings → Pages → Deploy from a branch → `main` / root**
3. En 1–2 minutos tendrás tu URL pública

> Requiere internet solo para cargar las librerías (pdf.js, pdf-lib, JSZip) desde CDN la primera vez.

## 🛠️ Stack técnico

| Capa | Tecnología |
|---|---|
| UI | HTML5 + CSS3 (variables, grid, animaciones nativas) |
| Lógica | JavaScript vanilla (sin frameworks, sin build) |
| Motor PDF | pdf.js 3.11 (render) + pdf-lib 1.17 (creación/edición) |
| Empaquetado | JSZip 3.10 (PDF → imágenes múltiples) |
| Hosting | Cualquier hosting estático (GitHub Pages, Cloudflare Pages…) |

### ¿Cómo comprime?

Re-muestrea las páginas a alta resolución y re-codifica sus imágenes internas en JPEG, probando calidades de mayor a menor hasta acercarse al objetivo que elegiste. Es el método más efectivo posible 100% en navegador. Si necesitas conservar el texto seleccionable, hay un modo de compresión ligera (reduce menos, pero no rasteriza).

## 💜 Apoya el proyecto

MenosEspacioPDF es gratis y sin anuncios. Si te resultó útil, puedes apoyar al creador desde el botón **"¿Te gusta? Apóyame"** dentro de la página (PayPal, Binance, transferencia o Pago Móvil 🇻🇪).

## 📄 Licencia

[MIT](LICENSE) © Emir Romero

---

<div align="center">
<sub>Hecho en Venezuela 🇻🇪 · Si te gustó, deja una ⭐ en el repo — ayuda muchísimo</sub>
</div>
