# Cronograma

Dos semanas: del miércoles 25 de noviembre al martes 8 de diciembre de 2026 (14 días, con fines de semana). Equipo de cuatro integrantes. La fecha de entrega publicada en Moodle prevalece: si es anterior al 8 de diciembre, hay que recortar el plan.

## Sprints

| Sprint | Fechas | Objetivo | Historias | Hito de cierre |
|---|---|---|---|---|
| 1. Planificación y base | 25 al 28 nov | Gestión, diseño, proyecto base, cálculo e importador | HU-01 a HU-04, HU-08, HU-11, HU-15, HU-16 | La aplicación arranca, importa contenido y pasa las pruebas de cálculo |
| 2. Construcción M1 a M5 | 29 nov al 3 dic | Módulos obligatorios y contenido completo | HU-05, HU-06, HU-09, HU-10, HU-12 a HU-14, HU-17, HU-18, HU-23 | M1 a M5 integrados con las 14 partes, salvo mapa e historial |
| 3. Cierre | 4 al 8 dic | Mapa, historial, M6, M7, pruebas y entregables | HU-07, HU-19 a HU-22, HU-24 a HU-29 | Entrega |

## Día a día

Del 26 de noviembre al 3 de diciembre cada integrante dedica media jornada a sus fichas y listas (HU-23) y la otra media a la tarea de la tabla.

| Fecha | I1 Zaith | I2 Matías | I3 Alexander | I4 Andrea |
|---|---|---|---|---|
| Mié 25 nov | Reunión inicial, enunciado y plan | Diseño del modelo de datos | HU-01 | Revisión de requisitos y casos de prueba de cálculo |
| Jue 26 nov | Formato YAML y ejemplo | HU-02, con I4 | Prototipo de pantallas de la biblioteca | HU-02 (usuario y roles), con I2 |
| Vie 27 nov | HU-08 | Revisión de pull requests | HU-04 | HU-03, matriz de trazabilidad |
| Sáb 28 nov | HU-08, HU-11 | Diseño de la lista de verificación | HU-04 | HU-15, HU-16 |
| Dom 29 nov | HU-12 | Revisión de HU-12 y preparación de HU-13 | HU-09 | HU-17 con datos de prueba |
| Lun 30 nov | Pruebas del importador con contenido real | HU-13 | HU-05, HU-06 | HU-17 |
| Mar 1 dic | Revisión de introducciones | HU-13 | HU-10 | HU-17 |
| Mié 2 dic | HU-18 | HU-14 | Pruebas de M1 a M3 | Integración de HU-17 |
| Jue 3 dic | HU-18, cierre del sprint | HU-14, cierre del sprint | Correcciones, cierre del sprint | Pruebas de integración, cierre del sprint |
| Vie 4 dic | HU-22 | HU-21 | HU-07 | HU-20 |
| Sáb 5 dic | HU-27 | HU-21 | HU-24 | HU-20, HU-19 |
| Dom 6 dic | HU-27, HU-25 | HU-28 | HU-24 | HU-26 |
| Lun 7 dic | HU-27, HU-25 | Prueba de instalación con el manual | Correcciones | Informe de pruebas |
| Mar 8 dic | HU-29, acta de aceptación y entrega | HU-29 | HU-29 | HU-29 |

## Dependencias

| Historia | Necesita terminada | Fecha en que queda disponible |
|---|---|---|
| HU-02 | HU-01 | 25 nov |
| HU-03, HU-04, HU-08 | HU-02 | 26 nov |
| HU-11 | HU-03 | 27 nov |
| HU-09, HU-12 | HU-08 | 28 nov |
| HU-17 (datos de prueba) | HU-15, HU-16 | 28 nov |
| HU-13 | HU-09, HU-11, HU-12 | 29 nov |
| HU-18 e integración de HU-17 | HU-13 | 1 dic |
| HU-26 | HU-20 | 5 dic |
| HU-25 (manual técnico y mantenimiento) | HU-28 | 6 dic |

## Control

| Fecha | Actividad |
|---|---|
| 25 nov | Reunión inicial (acta N.º 1) |
| 27 nov | Validación de requisitos con el docente (IS.2.1), a cargo de Andrea |
| 28 nov | Reporte de avance 1 y respaldo del repositorio |
| 3 dic | Reporte de avance 2, respaldo y corte de M1 a M5 |
| 4 dic | Mapa (HU-07) terminado, porque es función mínima de M1 |
| 8 dic | Reporte final, acta de aceptación y etiqueta `v1.0` |

Si el 3 de diciembre M1 a M5 no están completos, quien tenga pendientes los termina antes de empezar su parte de M6 y M7.

## Referencia: cronograma sugerido por la guía

La tabla 8 propone tres fases, que aquí se comprimen en los tres sprints.

| Semana | Fase | Productos |
|---|---|---|
| 1 | Planificación y análisis | Enunciado del trabajo; Plan del proyecto; Especificación de requisitos |
| 2 | Diseño y construcción | Diseño de software; código en el repositorio; reportes de avance |
| 3 | Pruebas, entrega y cierre | Informe de pruebas; manuales; acta de aceptación; presentación |
