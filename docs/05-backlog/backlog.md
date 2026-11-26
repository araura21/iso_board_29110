# Backlog

Plazo: 25 de noviembre al 8 de diciembre de 2026. Fechas por día y dependencias en el [cronograma](cronograma.md); I1 es Zaith Manangón, I2 Matías Lugmaña, I3 Alexander Villacres e I4 Andrea Raura ([roles](../08-gestion-29110/02-plan-del-proyecto.md)).

Puntos: estimación relativa (1, 2, 3, 5, 8). Responsable y estado se actualizan durante el proyecto.

Definición de terminado: código en `main` mediante pull request revisado por otro integrante, pruebas en verde, criterios de aceptación cumplidos y [trazabilidad](../01-requisitos/trazabilidad.md) actualizada.

## E0. Base del proyecto

| ID | Historia o tarea | Criterios de aceptación | Pts | Resp. | Sprint | Fecha límite | Estado |
|---|---|---|---|---|---|---|---|
| HU-01 | Crear proyecto, repositorio en GitHub y README de instalación | Otro integrante lo ejecuta siguiendo el README | 2 | I3 | 1 | 25 nov | Pendiente |
| HU-02 | Crear el modelo de datos y las migraciones (I4 apoya con usuario y roles) | Incluye todas las entidades y campos del [modelo](../03-base-de-datos/modelo-datos.md), con usuario personalizado en la primera migración; los datos persisten | 5 | I2 | 1 | 26 nov | Pendiente |
| HU-03 | Como usuario quiero iniciar sesión según mi rol | Contraseña cifrada; el consultor no puede editar | 3 | I4 | 1 | 27 nov | Pendiente |

## M1. Biblioteca

| ID | Historia | Criterios de aceptación | Pts | Resp. | Sprint | Fecha límite | Estado |
|---|---|---|---|---|---|---|---|
| HU-04 | Ver las partes agrupadas por tipo de documento | RF-01 | 3 | I3 | 1 | 28 nov | Pendiente |
| HU-05 | Recorrer la guía por capítulos desde un índice general | Índice, anterior y siguiente | 3 | I3 | 2 | 30 nov | Pendiente |
| HU-06 | Buscar normas por palabra clave | Busca en código, título e introducción | 2 | I3 | 2 | 30 nov | Pendiente |
| HU-07 | Navegar desde el mapa gráfico a cada ficha | RF-03 | 5 | I3 | 3 | 4 dic | Pendiente |

## M2 y M3. Fichas y acceso

| ID | Historia | Criterios de aceptación | Pts | Resp. | Sprint | Fecha límite | Estado |
|---|---|---|---|---|---|---|---|
| HU-08 | Importar el contenido de las normas desde YAML | Cumple las [reglas del importador](../03-base-de-datos/carga-contenido.md) | 5 | I1 | 1 | 28 nov | Pendiente |
| HU-09 | Consultar la ficha completa de una norma | Todos los campos de M2 y fuentes; espacio para el enlace a la lista | 3 | I3 | 2 | 29 nov | Pendiente |
| HU-23 | Investigar y redactar las 14 fichas y listas | [Tabla de carga](../04-contenido/familia-29110.md) completa | 8 | Todos | 1 y 2 | 3 dic | Pendiente |
| HU-10 | Descargar o consultar el documento oficial | RF-04 | 2 | I3 | 2 | 1 dic | Pendiente |

Reparto de HU-23. Las introducciones se entregan el 1 de diciembre y las listas el 3. I4 tiene menos partes porque la lista de 5-1-2 debe incluir todas las tareas de la norma.

| Integrante | Partes | Cantidad |
|---|---|---|
| I1 | 1-1, 1-2, 2-1, 3-1 | 4 |
| I2 | 3-2, 4-1, 5-1-1, 5-1-3 | 4 |
| I3 | 5-1-4, 5-3, 5-4, 5-6-1 | 4 |
| I4 | 5-1-2, 5-6-2 | 2 |

## M4. Lista de verificación

| ID | Historia | Criterios de aceptación | Pts | Resp. | Sprint | Fecha límite | Estado |
|---|---|---|---|---|---|---|---|
| HU-11 | Registrar una organización o proyecto | RF-05 | 2 | I1 | 1 | 28 nov | Pendiente |
| HU-12 | Ver la lista de una norma por proceso, actividad y tarea | RF-06 | 3 | I1 | 2 | 29 nov | Pendiente |
| HU-13 | Marcar cada ítem desde la ficha | RF-07 y RNF-01 | 5 | I2 | 2 | 1 dic | Pendiente |
| HU-14 | Adjuntar evidencias, observación, responsable y fecha | RF-08 | 5 | I2 | 2 | 3 dic | Pendiente |

## M5. Tablero

| ID | Historia | Criterios de aceptación | Pts | Resp. | Sprint | Fecha límite | Estado |
|---|---|---|---|---|---|---|---|
| HU-15 | Calcular el porcentaje por norma, proceso y organización | RN-01, pruebas unitarias | 3 | I4 | 1 | 28 nov | Pendiente |
| HU-16 | Asignar el estado de aplicación | RN-02, pruebas unitarias | 2 | I4 | 1 | 28 nov | Pendiente |
| HU-17 | Ver tablero con indicadores y gráficos | RF-11; integrado con respuestas reales | 5 | I4 | 2 | 2 dic | Pendiente |
| HU-18 | Listar brechas y registrar acciones de mejora | RF-12 | 3 | I1 | 2 | 3 dic | Pendiente |
| HU-19 | Comparar evaluaciones en el tiempo | RF-14 | 3 | I4 | 3 | 5 dic | Pendiente |

## M6 y M7. Reportes y administración

| ID | Historia | Criterios de aceptación | Pts | Resp. | Sprint | Fecha límite | Estado |
|---|---|---|---|---|---|---|---|
| HU-20 | Exportar el estado a PDF y hoja de cálculo | Incluye fecha y responsable | 5 | I4 | 3 | 5 dic | Pendiente |
| HU-21 | Administrar familias, normas, apartados e ítems | Se registra una familia nueva sin tocar código | 5 | I2 | 3 | 5 dic | Pendiente |
| HU-22 | Administrar usuarios y roles | Solo el administrador | 2 | I1 | 3 | 4 dic | Pendiente |

## Cierre

| ID | Tarea | Criterios de aceptación | Pts | Resp. | Sprint | Fecha límite | Estado |
|---|---|---|---|---|---|---|---|
| HU-24 | Verificar rendimiento y accesibilidad | RNF-04 y RNF-07 | 3 | I3 | 3 | 6 dic | Pendiente |
| HU-25 | Manuales de usuario y técnico y [documento de mantenimiento](../09-entrega/documento-mantenimiento.md) (I2 revisa la parte técnica); instalación en otro equipo | RNF-06, IS.6.1 | 3 | I1 | 3 | 7 dic | Pendiente |
| HU-26 | Evaluar una organización de ejemplo y generar su reporte | Entregable 6 | 2 | I4 | 3 | 6 dic | Pendiente |
| HU-27 | Informe técnico APA 7 | Entregable 3 | 5 | I1 | 3 | 7 dic | Pendiente |
| HU-28 | Desplegar en una URL con almacenamiento persistente y crear el usuario de prueba para el docente | Entregable 2 | 3 | I2 | 3 | 6 dic | Pendiente |
| HU-29 | Carpeta de evidencias y presentación de 10 minutos | Entregables 4 y 7 | 3 | Todos | 3 | 8 dic | Pendiente |

## Carga por integrante

| Responsable | Sprint 1 | Sprint 2 | Sprint 3 | Puntos propios |
|---|---|---|---|---|
| I1 | 7 | 6 | 10 | 23 |
| I2 | 5 | 10 | 8 | 23 |
| I3 | 5 | 10 | 8 | 23 |
| I4 | 8 | 5 | 10 | 23 |

Los 11 puntos compartidos (HU-23 y HU-29) se reparten entre los cuatro. Total del backlog: 103.
