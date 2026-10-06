# TRAB 2026 · Módulo 5 · Datasets para ANOVA

Este paquete contiene 10 conjuntos de datos sintéticos para actividades por equipo.

## Estructura
Cada archivo contiene entre 120 y 190 observaciones y tres grupos: `A`, `B`, `C`.

Columnas:
- `participant_id`: identificador de la observación.
- `group`: condición experimental (`A`, `B`, `C`).
- `hours`: tiempo de exposición.
- `measurement_before`: medición inicial.
- `measurement_after`: medición posterior.
- `change`: diferencia `measurement_after - measurement_before`.

## Pregunta de investigación sugerida
**¿El cambio observado difiere entre las tres condiciones experimentales?**

Hipótesis nula:
`H0: mu_A = mu_B = mu_C`

## Uso pedagógico
1. Explorar los datos.
2. Visualizar `change` por `group`.
3. Comparar medias y variabilidad.
4. Ejecutar un ANOVA de una vía.
5. Interpretar el resultado sin confundir significancia estadística, causalidad e importancia práctica.
6. Construir una historia científica apropiada para paper, propuesta, reporte o presentación.

## Importante
Los datos son completamente sintéticos y fueron creados con fines docentes. No representan personas, experimentos ni resultados reales.

`dataset_validation_summary.csv` contiene resultados de control para el instructor. No es necesario entregarlo a los participantes.
