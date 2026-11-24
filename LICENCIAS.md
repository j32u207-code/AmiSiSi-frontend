# Licencias y Derechos de Autor — Proyecto AmiSiSi
### Creado por Jesús Cinta Ortega — CEO de AmiSiSi

Este documento detalla la autoría, fuente original, tipo de licencia, modificaciones técnicas y métricas de optimización aplicadas a todos los recursos multimedia incluidos en el proyecto **AmiSiSi** (archivos optimizados en `src/media/` y originales en `media-bruto/`), cumpliendo estrictamente con las condiciones legales de cada licencia.

---

## 1. Fotografías e imágenes (`src/media/img/`)

| Archivo en producción | Archivo bruto original | Autor | Fuente | Licencia | Modificaciones realizadas |
| :--- | :--- | :--- | :--- | :--- | :--- |
| `cazadora.webp` | `pexels-gaith-reo-2471988-4091883.jpg` | Gaith Reo | [Pexels](https://www.pexels.com/es-es/foto/ciudad-moda-hombre-acera-4091883/) | [Pexels License](https://www.pexels.com/es-es/license/) (Uso libre gratuito) | Reescalado en GIMP, eliminación de metadatos y exportación a WebP (calidad 80). |
| `sudadera.webp` | `pexels-modelstma-20752934.jpg` | TMA Management (`@modelstma`) | [Pexels](https://www.pexels.com/photo/20752934/) | [Pexels License](https://www.pexels.com/es-es/license/) (Uso libre gratuito) | Reescalado en GIMP, eliminación de metadatos y exportación a WebP (calidad 80). |
| `pantalon.webp` | `pexels-ahcapture-29817645.jpg` | Alireza Heidarpour (`@ahcapture`) | [Pexels](https://www.pexels.com/es-es/foto/joven-con-capucha-en-entorno-urbano-29817645/) | [Pexels License](https://www.pexels.com/es-es/license/) (Uso libre gratuito) | Reescalado en GIMP, eliminación de metadatos y exportación a WebP (calidad 80). |
| `Nubes.png` | `Nubes.png` | Generada con Google Gemini | [Google Gemini](https://gemini.google.com/) | Uso libre (contenido generado por IA) | Imagen de fondo corporativa conservada como identidad visual de la marca. |

---

## 2. Iconos Vectoriales SVG (`src/media/img/`)

| Archivos optimizados | Autor | Fuente | Licencia | Modificaciones realizadas |
| :--- | :--- | :--- | :--- | :--- |
| `search.svg`, `cart2.svg`, `person.svg`, `house.svg`, `list.svg`, `box-arrow-right.svg` | The Bootstrap Authors | [Bootstrap Icons](https://icons.getbootstrap.com/) | [MIT License](https://github.com/twbs/icons/blob/main/LICENSE) | Limpieza y minificación de código SVG con SVGOMG. |

---

## 3. Audio (`src/media/audio/`)

| Archivo optimizado | Archivo bruto original | Título y Autor | Fuente | Licencia | Modificaciones realizadas |
| :--- | :--- | :--- | :--- | :--- | :--- |
| `jazz-fondo.mp3` | `564001__migfus20__jazz-background-music-loop.mp3` | *Jazz Background Music Loop* — **Migfus20** (Schwarzenegger Belonio) | [Freesound](https://freesound.org/people/Migfus20/sounds/564001/) | [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) (Reconocimiento 4.0 Internacional) | Recorte a 45 s en Audacity, normalización a -3,0 dB, desvanecimiento de entrada/salida y exportación a MP3 Estéreo (96 kbps, 44100 Hz). |
| `click-teclado.mp3` | `766639__stavsounds__keyboard_tactile_8.ogg` | *Keyboard_Tactile_8* — **StavSounds** | [Freesound](https://freesound.org/people/StavSounds/sounds/766639/) | [CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/) (Dominio Público) | Normalización a -1,0 dB en Audacity y exportación a MP3 Mono (96 kbps, 44100 Hz). |

---

## 4. Vídeo (`src/media/video/`)

| Archivo optimizado | Archivo bruto original | Autor | Fuente | Licencia | Modificaciones realizadas |
| :--- | :--- | :--- | :--- | :--- | :--- |
| `promo-amisisi.mp4` | `10352446-uhd_4096_2160_25fps.mp4` | **cottonbro studio** | [Pexels](https://www.pexels.com/video/10352446/) | [Pexels License](https://www.pexels.com/es-es/license/) (Uso libre gratuito) | Reducción de 4K a 1080p (25 FPS constantes), codificación H.264 (x264) multipase a 1500 kbps y optimización para web en HandBrake. |

---

## 5. Comparativa de optimización (Antes y Después)

| Categoría | Archivo bruto (`media-bruto/`) | Peso bruto | Archivo optimizado (`src/media/`) | Peso final | Ahorro | Optimización aplicada |
| :--- | :--- | :---: | :--- | :---: | :---: | :--- |
| **Foto** | `pexels-gaith-reo-2471988-4091883.jpg` | 4,02 MB | `cazadora.webp` | 26,2 KB | **-99,4 %** | Reescalado en GIMP, sin metadatos, WebP calidad 80 |
| **Foto** | `pexels-modelstma-20752934.jpg` | 1,62 MB | `sudadera.webp` | 37,9 KB | **-97,7 %** | Reescalado en GIMP, sin metadatos, WebP calidad 80 |
| **Foto** | `pexels-ahcapture-29817645.jpg` | 690 KB | `pantalon.webp` | 15,7 KB | **-97,7 %** | Reescalado en GIMP, sin metadatos, WebP calidad 80 |
| **Iconos (×6)** | `box-arrow-right`, `cart2`, `house`, `list`, `person`, `search` (.svg) | 2.446 B (2,39 KB) | Mismos 6 archivos `.svg` | 2.419 B (2,36 KB) | **-1,1 %** | Minificación con SVGOMG |
| **Audio (música)** | `564001__migfus20__jazz-background-music-loop.mp3` (1:31) | 2,09 MB | `jazz-fondo.mp3` (0:45) | 528 KB | **-75,3 %** | Recorte a 45 s, normalizado -3 dB, fade in/out, MP3 Estéreo 96 kbps |
| **Audio (UI)** | `766639__stavsounds__keyboard_tactile_8.ogg` | 13,8 KB | `click-teclado.mp3` | 3,36 KB | **-75,7 %** | Normalizado -1 dB, conversión a MP3 Mono 96 kbps |
| **Vídeo** | `10352446-uhd_4096_2160_25fps.mp4` (4K, 24 s) | 40,0 MB | `promo-amisisi.mp4` (1080p, 24 s) | 4,37 MB | **-89,1 %** | 4K → 1080p, 25 FPS constantes, H.264 2 pasadas 1500 kbps, Web Optimized |
| **TOTAL (12 assets)** | **Carpeta `media-bruto/`** | **48,42 MB** | **Assets optimizados en `src/media/`** | **4,97 MB** | **-89,7 %** | **Reducción neta de 43,45 MB** |

### Resumen de ahorro por tipo de recurso
* **Fotografías:** de 6,31 MB a 79,8 KB (**-98,8 %**), todas muy por debajo del límite de 150 KB.
* **Audio:** de 2,10 MB a 531,4 KB (**-75,3 %**).
* **Vídeo:** de 40,0 MB a 4,37 MB (**-89,1 %**).
* **Iconos SVG:** 2,36 KB en total para los 6 iconos vectoriales, escalables sin pérdida de nitidez.
* *Nota:* El fondo corporativo `Nubes.png` (1,36 MB) se mantiene aparte como recurso de identidad visual heredado del diseño original de la marca.

---

## Notas legales
* **Atribución CC BY 4.0:** La pista *Jazz Background Music Loop* de **Migfus20** se utiliza bajo licencia [Creative Commons Attribution 4.0](https://creativecommons.org/licenses/by/4.0/), acreditando al autor original e indicando expresamente las modificaciones de recorte, normalización y compresión aplicadas.
* **Dominio Público (CC0) y Licencias Libres:** El efecto de teclado de **StavSounds** está liberado en dominio público (CC0 1.0), los iconos vectoriales de **The Bootstrap Authors** se usan bajo licencia libre MIT, las fotografías y el vídeo de **Pexels** se emplean conforme a la Pexels License (uso y edición gratuitos sin restricciones comerciales) y el fondo `Nubes.png` es una imagen generada con Google Gemini para el proyecto.