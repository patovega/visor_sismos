# 🌋 Secuencia Sísmica — II Región de Antofagasta · Mayo 2026

Visualización interactiva de la secuencia sísmica desencadenada por el terremoto principal **M6.9 Mww** del 25 de mayo de 2026 a las 17:52 hora local, en la zona de Calama, Región de Antofagasta, Chile.

---

## 🚀 Uso

Descarga `sismos.html` y ábrelo con doble clic en tu navegador.

**No requiere servidor, no requiere instalación, no requiere conexión a internet** para los datos — el JSON está embebido directamente en el HTML. Sí necesita conexión para cargar los tiles del mapa (OpenStreetMap).

---

## 📊 Datos

- **65 eventos** registrados entre el 25/05/2026 06:27 y el 26/05/2026 08:30 (hora local)
- Sismo principal: **M6.9 Mww** · 25 mayo 2026 · 17:52 local · Prof. 114 km · 20 km al NE de Calama
- Fuente: [Centro Sismológico Nacional (CSN)](https://www.sismologia.cl), Universidad de Chile
  - https://www.sismologia.cl/sismicidad/catalogo/2026/05/20260525.html
  - https://www.sismologia.cl/sismicidad/catalogo/2026/05/20260526.html

### Zonas cubiertas
| Zona | Eventos |
|------|---------|
| Calama y alrededores | 54 |
| Pica / Pozo Almonte | 5 |
| Mina Collahuasi | 4 |
| Sierra Gorda | 1 |
| Mina La Escondida | 1 |

---

## ✨ Características

- 🗺 Mapa base **OpenStreetMap** via Leaflet.js — sin API key
- 🔵 Burbujas escaladas y coloreadas por magnitud, con el valor impreso dentro
- ▶ Animación cronológica con **play / pausa / repetir**
- 🎞 Slider para navegar manualmente por la secuencia
- ⌨ Atajos de teclado: `Espacio` play/pause · `←` `→` evento a evento
- 💬 Popup con detalle completo al hacer clic en cada sismo (lugar, hora, profundidad, coordenadas, zona)
- 📦 **JSON embebido en el HTML** — un solo archivo, sin fetch, sin CORS, sin servidor

---

## 🎨 Paleta de magnitudes

| Rango | Color |
|-------|-------|
| 2.5 – 3.0 | 🟢 Verde |
| 3.0 – 4.0 | 🔵 Azul |
| 4.0 – 5.0 | 🟠 Naranja |
| 5.0 – 6.0 | 🟩 Verde neón |
| > 6.0 | 🟤 Cobre |

El tamaño de cada burbuja también es proporcional a la magnitud. El sismo principal (M6.9) pulsa con animación al aparecer en la secuencia.

---

## 📁 Archivos

| Archivo | Descripción |
|---------|-------------|
| `sismos.html` | Visualización completa — standalone, sin dependencias locales |
| `sismos_2_region_2026.json` | Datos sísmicos estructurados (65 eventos, con metadata CSN) |
| `README.md` | Este archivo |

---

## 🛠 Tecnologías

- [Leaflet.js](https://leafletjs.com) 1.9.4
- [OpenStreetMap](https://openstreetmap.org) · tiles via CDN
- Vanilla JavaScript · HTML5 · CSS3
- Sin frameworks, sin build tools, sin dependencias locales

---

## 🤖 Créditos

Desarrollado con la asistencia de **[Claude](https://claude.ai)** (Anthropic).  
El análisis del catálogo sísmico, la estructuración del JSON, el código HTML/JS/CSS y la visualización completa fueron generados en conversación con Claude Sonnet a través de [claude.ai](https://claude.ai).

[![Built with Claude](https://img.shields.io/badge/Built%20with-Claude%20AI-D97706?style=flat&logo=anthropic&logoColor=white)](https://claude.ai)

---

## 📜 Licencia

- Datos sísmicos © [Centro Sismológico Nacional](https://www.sismologia.cl), Universidad de Chile
- Mapa © [OpenStreetMap](https://openstreetmap.org) contributors — licencia [ODbL](https://opendatacommons.org/licenses/odbl/)
- Código: MIT
