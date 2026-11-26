# Plan de pruebas

## Niveles

| Nivel | Alcance | Herramienta |
|---|---|---|
| Unitarias | Cálculo, estados, brechas, permisos | pytest |
| Integración | Importador, evaluación completa, exportación | pytest-django |
| Funcionales | Un caso por requisito funcional | Manual con registro |
| No funcionales | RNF-01 a RNF-07 | Según [criterios](../01-requisitos/no-funcionales.md) |
| Aceptación | Recorrido con el cliente | Acta de aceptación |

## Casos unitarios de cálculo y estado

Los casos PU-06, PU-09, PU-10 y PU-11 prueban los casos límite de [RN-02](../01-requisitos/reglas-de-negocio.md). PU-05 y PU-08 suponen evidencias adjuntas; sin ellas el estado esperado es Casi conforme.

| ID | C | P | NC | NA | Sin respuesta | % esperado | Estado esperado |
|---|---|---|---|---|---|---|---|
| PU-01 | 0 | 0 | 0 | 0 | 10 | 0 | No iniciado |
| PU-02 | 1 | 0 | 9 | 0 | 0 | 10 | En inicio |
| PU-03 | 3 | 2 | 5 | 0 | 0 | 40 | En progreso |
| PU-04 | 7 | 2 | 1 | 0 | 0 | 80 | Casi conforme |
| PU-05 | 10 | 0 | 0 | 0 | 0 | 100 | Conforme (con evidencias) |
| PU-06 | 0 | 0 | 10 | 0 | 0 | 0 | En inicio |
| PU-07 | 4 | 1 | 3 | 2 | 0 | 56,25 | En progreso |
| PU-08 | 8 | 0 | 0 | 2 | 0 | 100 | Conforme (con evidencias) |
| PU-09 | 79 | 1 | 120 | 0 | 0 | 39,75 | En inicio |
| PU-10 | 199 | 1 | 0 | 0 | 0 | 99,75 | Casi conforme |
| PU-11 | 0 | 0 | 0 | 10 | 0 | Sin valor | Sin ítems aplicables |
| PU-12 | 5 | 0 | 0 | 0 | 5 | 50 | En progreso |

## Casos funcionales

| ID | Requisito | Caso | Resultado | Fecha |
|---|---|---|---|---|
| PF-01 | RF-01 | Las 14 partes aparecen agrupadas | | |
| PF-02 | RF-02 | Cada ficha muestra introducción y fuentes | | |
| PF-03 | RF-03 | Cada nodo del mapa abre su ficha | | |
| PF-04 | RF-04 | Cada botón abre su enlace y muestra el tipo de acceso | | |
| PF-05 | RF-05 | Registrar organización; rechazar campos vacíos | | |
| PF-06 | RF-06 | Lista con jerarquía de proceso, actividad y tarea | | |
| PF-07 | RF-07 | Marcar y cambiar los cuatro valores | | |
| PF-08 | RF-08 | Adjuntar archivo y enlace; guardar observación, responsable y fecha | | |
| PF-09 | RF-11 | Tablero muestra indicadores y gráficos correctos | | |
| PF-10 | RF-12 | Brechas incluyen solo NC y P, con acción de mejora | | |
| PF-11 | RF-13 | Exportar PDF y hoja de cálculo con fecha y responsable | | |
| PF-12 | RF-14 | Comparar dos evaluaciones | | |
| PF-13 | RF-15 | Cada rol accede solo a lo permitido | | |

## Informe de pruebas

Registrar fecha, versión (commit), casos ejecutados, fallos, correcciones y resultado final. Se entrega en la [carpeta de evidencias](../08-gestion-29110/README.md).
