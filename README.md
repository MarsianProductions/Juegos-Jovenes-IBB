# 📋 Historial de Cambios

## [2.0.0] - 2026-10-14
### ⚡ Nuevo: Sistema de Desempate («Duelo Decisivo»)
- Botón automático «⚡ Desempate» al registrar empate en rondas o juego final.
- Modal exclusivo que aísla solo a los equipos empatados con contadores dedicados (+ / −) desde 0.
- Opciones ante persistencia de empate: «Dejar en empate» o «Volver a decidir (reiniciar)».

### 👥 Distribución Geométrica de Equipos (Desktop y Tablet)
- Reorganización visual a un máximo de 3 equipos por fila:
  - 6 equipos: 2 filas ordenadas de 3 equipos.
  - 5 equipos: Fila de 3 arriba y 2 equipos abajo centrados en los intersticios.
  - 4 equipos: Fila de 3 arriba y el equipo 4 centrado debajo del equipo 2.
  - 3 equipos: Fila completa de 3 equipos.
  - 2 equipos: Tarjetas equilibradas y centradas.
- En celulares (pantallas ≤ 680px) se mantiene la vista de 1 columna vertical.

### 🎨 Contraste, Tipografía y Espaciado
- Texto de ideas y opciones en blanco puro (`#ffffff`), tamaño grande (`1.08rem`) y negrita (`800`) con sombra suave.
- Aumento de contraste global en textos secundarios (`#c9d5f0`, ratio > 9:1).
- Mayor espaciado vertical en el banner del juego, tarjetas de equipos y randomizador.

### 🛠️ Correcciones y Seguridad
- Persistencia de 6 equipos y colores únicos en `localStorage` (evita borrado o reinicio de nombres al cambiar la cantidad de equipos).
- Botón «↩ Deshacer» para revertir puntuaciones erróneas.
- Diálogos de confirmación al finalizar rondas y al reiniciar todo.

### 🔊 Audio procedural y Animaciones
- Alerta sonora triple (Web Audio API) al terminar el temporizador.
- Animación de ruleta y barra de carga sincronizada a 1.5s en el sorteo de palabras.
- Animación de puntos flotantes (`+1`, `-1`) centrada en cada equipo.
