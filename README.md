# Padel Tracker PWA

Primera versión funcional de una web-app móvil para registrar estadísticas de dos jugadores de pádel.

## Uso
1. Sube estos archivos a un hosting HTTPS (por ejemplo GitHub Pages).
2. Abre la URL desde Safari en iPhone.
3. Pulsa Compartir > Añadir a pantalla de inicio.

## Datos
Los partidos se guardan localmente en el navegador mediante localStorage.
No requiere servidor ni base de datos para esta V1.


## V2
- Winner y ficha cuentan como golpes sin error en el porcentaje de consistencia.
- Dashboard rediseñado con selector de jugador, barras por categoría, donut de consistencia y secuencia de eventos.


## V2.1
- Corregida la caché del Service Worker para que las nuevas versiones de GitHub Pages se actualicen correctamente.
- Añadido indicador visible v2.1.

## V3
- Ficha deja de contar como golpe independiente.
- Ficha actúa como etiqueta de riesgo: tras pulsarla hay que clasificar el resultado como Bola dentro, Error no forzado o Winner.
- Nuevo modificador Smash con la misma lógica.
- Dashboard con desglose de Fichas y Smash: intentos, entran, falladas, winners, % éxito y % winner.
