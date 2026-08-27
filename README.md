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

## Final comparison update
- Added a three-way report selector: Player 1 / Comparison / Player 2.
- Added mirrored football-style comparison bars.
- Added objective impact metrics:
  - Positive relevance = Winners
  - Negative relevance = Unforced errors + Return errors + Double faults
  - Net impact = Positive relevance - Negative relevance
- Risk is based only on Ficha attempts and their outcomes.
- Smash remains a separate technical statistic and is not included in the risk metric.

## V4 TEST - marcador
- Al pulsar Fin de juego se obliga a seleccionar quién ganó: Jugador 1 + Jugador 2 o Pareja contraria.
- El marcador de juegos se actualiza automáticamente.
- Los sets estándar se detectan automáticamente (6-x con 2 de diferencia, 7-5 y 7-6).
- El reporte muestra sets ganados y parciales de cada set.
- Deshacer puede revertir el último juego asignado.

## V8 TEST
- Contadores visibles reiniciados automáticamente por juego; los datos completos se conservan.
- Nuevo registro Error forzado.
- Colores coherentes entre botones y dashboard; Doble falta en amarillo.
- Eliminado KPI Fichas/Smash del bloque principal.
- Secuencia de golpes con divisores visuales de juego y set.
- Gráfico radar comparativo.
- Índice de Impacto 0–100 ponderado: 45% puntos, 30% consistencia, 15% Fichas, 10% contexto competitivo.
- Resumen automático del jugador con mayor impacto positivo.
- Borrado de partidos desde Historial con confirmación.
