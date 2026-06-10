# 🎙️📺 Te Lo Cuento - Producción Pro

**Crea reportajes, notas periodísticas y videos profesionales con mezclador de 3 pistas, visualizadores de audio y gráficos de noticiero directamente desde tu navegador.**  
Sin servidores, sin marcas de agua, sin límites. Todo el procesamiento de audio y video se realiza de forma local, segura y en tiempo real en tu dispositivo.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Web Audio API](https://img.shields.io/badge/Web_Audio_API-FF9800?style=for-the-badge&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

---

## 🌟 Características Principales

### 🎛️ Mezcla de Audio de Nivel Profesional (3 Pistas)
* **Audio Principal (Voz):** Fijo al 100%. Es el protagonista y el único que activa los efectos visuales.
* **Audio del Video (Entrevista/Ambiente):** Volumen independiente (ej. 30%). Se mantiene estable durante todo el reporte, sin subidas bruscas al final, respetando el flujo periodístico.
* **Cortina Musical (Opcional):** Volumen independiente (ej. 20%). Con control preciso de inicio (slider y saltos) y bucle inteligente si es más corta que el video.
* **Limitador Anti-Clipping:** Compresor dinámico (`DynamicsCompressor`) integrado que evita distorsiones y saturación al mezclar las 3 pistas.

### 📺 Gráficos de Noticiero (Lower & Upper Third)
* **Titular Principal (Lower Third):** Franja de color en la parte **inferior** (Rojo, Cian o Negro) para garantizar que los rostros y el video de fondo nunca queden tapados.
* **Fecha, Hora y Lugar (Upper Third):** Texto discreto en la parte superior con sombra suave para máxima legibilidad. Incluye botón **"🔄 Auto"** que rellena automáticamente con la ubicación predeterminada (*Apóstoles*) y la fecha/hora actual.
* **Badge "🔴 EN VIVO":** Indicador opcional en la esquina superior para mayor impacto visual.

### 🎨 Visualización Reactiva Inteligente
* **4 Efectos Visuales:** Barras de Frecuencia, Onda Suave, Círculos Concéntricos y Partículas Reactivas.
* **Comportamiento Limpio:** Los efectos **solo** reaccionan a la voz. Durante la intro visual o cuando la voz termina, el canvas se limpia automáticamente, dejando el video de fondo y los gráficos perfectamente visibles sin artefactos.

### ⚡ Rendimiento y Compatibilidad Móvil
* **100% Cliente (Client-Side):** Tus archivos nunca salen de tu dispositivo. Privacidad y velocidad garantizadas.
* **Exportación Inteligente:** Soporte nativo para `.mp4` (iOS) y `.webm` (Android/Desktop).
* **Sistema de Rescate Móvil:** Utiliza la `Web Share API` nativa del celular. Si el navegador bloquea la descarga, aparece un modal con el video listo para que lo guardes con un toque o lo compartas directo a WhatsApp/Instagram.

---

## 🚀 Cómo usarlo

1. **Clona el repositorio** o descarga el archivo `index.html`.
2. Abre el archivo en un navegador moderno (Se recomienda **Google Chrome**, **Edge** o **Brave** para el mejor soporte de `MediaRecorder` y `Web Audio API`).
3. **Carga tus archivos:**
   * **1. Fondo:** Video del reportaje o entrevista (acepta también imágenes).
   * **2. Audio Principal:** Tu grabación de voz o locución.
   * **3. Cortina Musical:** (Opcional) Música ambiental de fondo.
4. **Edita y Marca:** Usa los paneles de preview para marcar el segundo exacto de inicio del video y de la música.
5. **Configura:** 
   * Ajusta los volúmenes (Recomendado: Video 30%, Cortina 20%).
   * Activa los **Gráficos de Noticiero** y usa el botón "Auto" para la fecha/lugar.
   * Elige la **Orientación** (16:9 o 9:16) y el **Efecto Visual**.
   * Define el **Retraso de la voz** (Intro visual de 2s recomendado) y la **Duración máxima**.
6. **Exporta:** Haz clic en `💾 Exportar`. El video se procesará y se descargará o compartirá automáticamente al finalizar.

---

## 📋 Flujos de Trabajo Recomendados

### 📱 Para Estados de WhatsApp (Máx. 90s)
```text
Intro visual: 2 segundos
Tiempo extra: 10 segundos
Duración máxima: 90 segundos (WhatsApp)
Gráficos: Titular + Fecha/Lugar (Auto)
