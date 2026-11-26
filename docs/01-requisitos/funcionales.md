# Requisitos funcionales

El texto y la prioridad vienen de la tabla 2 de la guía. La columna de criterios de aceptación es una propuesta del equipo y debe validarse.

| Código | Requisito | Prioridad | Módulo | Criterios de aceptación (propuestos) |
|---|---|---|---|---|
| RF-01 | Listar todas las partes de la familia ISO/IEC 29110 agrupadas por tipo de documento: visión general, perfiles, evaluación y certificación, y guías. | Alta | M1 | Las 14 partes aparecen en uno de los cuatro grupos. |
| RF-02 | Mostrar, para cada parte, una introducción redactada por el equipo con sus propias palabras y las fuentes consultadas. | Alta | M2 | Ninguna ficha queda sin introducción ni sin fuente. |
| RF-03 | Mostrar el mapa gráfico de la familia y permitir navegar desde él hacia la ficha de cada parte. | Media | M1 | Cada nodo abre su ficha, también con teclado. |
| RF-04 | Incluir en cada ficha un botón para descargar o consultar el documento oficial de la norma. | Alta | M3 | El botón indica acceso gratuito, de pago o institucional y su enlace está verificado. |
| RF-05 | Registrar organizaciones o proyectos a evaluar, con nombre, tamaño del equipo y perfil objetivo. | Alta | M4 | Los tres campos son obligatorios. |
| RF-06 | Presentar la lista de verificación de cada parte, organizada por proceso, actividad y tarea cuando corresponda. | Alta | M4 | La jerarquía se ve en pantalla y cada parte tiene su lista. |
| RF-07 | Permitir marcar cada ítem como Cumple, Cumple parcialmente, No cumple o No aplica. | Alta | M4 | El valor queda guardado y puede cambiarse. |
| RF-08 | Adjuntar evidencias por ítem (archivo o enlace) y registrar observaciones, responsable y fecha. | Media | M4 | Un ítem admite varias evidencias de ambos tipos. |
| RF-09 | Calcular automáticamente el porcentaje de cumplimiento por norma, por proceso y por organización. | Alta | M5 | Cumple la [fórmula](reglas-de-negocio.md) y se actualiza al cambiar una respuesta. |
| RF-10 | Asignar el estado de aplicación de cada norma según las reglas de la tabla 4. | Alta | M5 | Pasan los casos del [plan de pruebas](../07-pruebas/plan-pruebas.md). |
| RF-11 | Mostrar un tablero con indicadores y gráficos del avance de cada norma. | Alta | M5 | Muestra porcentaje, estado y al menos un gráfico por organización. |
| RF-12 | Listar las brechas, es decir, los ítems con No cumple o Cumple parcialmente, con su acción de mejora. | Media | M5 | La acción de mejora se puede registrar y editar. |
| RF-13 | Exportar reportes de estado a PDF o a hoja de cálculo. | Media | M6 | El archivo incluye estado por norma, fecha y responsable. |
| RF-14 | Guardar el historial de evaluaciones para comparar el avance en el tiempo. | Media | M5 | Se comparan dos evaluaciones de la misma norma y organización. |
| RF-15 | Administrar normas, apartados, ítems y usuarios con control de acceso por rol. | Media | M7 | Alta, edición y eliminación; solo el administrador accede. |

## Funciones mínimas por módulo que no tienen código RF

La tabla 1 de la guía pide además estas funciones. Se controlan en el [backlog](../05-backlog/backlog.md).

| Módulo | Función |
|---|---|
| M1 | Índice general, navegación por capítulos y buscador por palabra clave |
| M2 | Ficha con código, título, edición vigente, propósito, introducción, audiencia, perfiles relacionados, contenido principal y normas vinculadas |
