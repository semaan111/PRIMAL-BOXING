# PRIMAL Boxing Club — GitHub Pages

Aplicación bilingüe de entrenamiento de boxeo con 114 combinaciones, video vertical con superposiciones, cronómetro y música de YouTube.

## Actualización de identidad

- Marca: **PRIMAL**.
- Símbolo: `primal.png`, imagen proporcionada por el usuario; también `primal-favicon.png`.
- Botón «Inicio»: se oculta cuando ya estás en la pantalla de inicio.
- YouTube: reproductor visible oficial de 200 × 200 píxeles dentro del flujo de la página, **no flotante**. De este modo no tapa ningún componente. El reproductor puede exigir pulsar Play.

## Prioridad: voz

Se desactivó la voz robótica MP3 para **escuchar** instrucciones en vivo. La app vuelve a utilizar la síntesis de voz nativa del dispositivo, disponible en Ajustar > Voz del dispositivo, con selección de voces español/inglés. Puede elegir otras voces instaladas (por ejemplo, mejoradas en iOS). Suena **la misma voz del dispositivo** en la sesión normal y durante la captura. No se puede garantizar una voz natural en todos los dispositivos: depende de las voces del sistema.

**Limitación técnica importante:** las voces `speechSynthesis` no exponen un audio capturable directamente por `MediaRecorder`. Para conservar una pista de voz grabada, el video sigue utilizando los fragmentos MP3 sintéticos anteriores **solo dentro del archivo exportado**; la persona oye en vivo la voz nativa. Para que suenen exactamente igual en el video y en vivo, se necesitan grabaciones de voz natural (por ejemplo, audios generados o grabados profesionalmente) y sustituir el banco de voz. No se afirma que el problema de naturalidad del archivo exportado esté resuelto.

**YouTube:** debido a las restricciones del reproductor incrustado, este debe permanecer visible y ocupar al menos 200×200 px. Está situado debajo de las funciones principales, sin posición flotante. Durante la grabación se pausa YouTube para evitar mantener un reproductor oculto bajo el video. La app no extrae ni descarga el audio de YouTube.

## Instalación

1. Descomprime el ZIP.
2. Abre tu repositorio GitHub, **Add file → Upload files**.
3. Sube el contenido de la carpeta, incluido `coach-audio/` y `.nojekyll` (si tu interfaz lo permite).
4. Haz Commit. La página funcionará como sitio estático en GitHub Pages.
5. Prueba primero en tu iPhone una sesión de 10–15 segundos y una grabación.

No se ha probado audio real en un iPhone desde este entorno. El formato de video y el comportamiento de `speechSynthesis` pueden variar en Safari.
