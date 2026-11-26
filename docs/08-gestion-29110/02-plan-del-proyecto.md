# Plan del proyecto

Versión: 0.1 (borrador). Aprobado por: ____ Fecha: ____

## Equipo y roles (GP.1)

| ID | Integrante | Roles | Responsabilidades |
|---|---|---|---|
| I1 | Zaith Manangón | GP, PR | Planificar y controlar el proyecto, calendario y cambios; reuniones y actas; coordinar la aceptación con el cliente. Programa importador, organizaciones, brechas y usuarios; manuales e informe |
| I2 | Matías Lugmaña | LT, PR | Arquitectura y decisiones técnicas, modelo de datos, revisión de código, GitHub y despliegue. Programa lista de verificación, evidencias y administración de contenido |
| I3 | Alexander Villacres | DIS, PR | Diseño detallado, prototipos e interfaces, navegación, usabilidad y accesibilidad. Programa proyecto base, biblioteca, fichas y acceso |
| I4 | Andrea Raura | AN, PR | Especificar y validar requisitos con el cliente, trazabilidad; coordinar pruebas y corrección de defectos. Programa acceso por rol, cálculo, tablero y reportes |
| CL | Ing. Diego Gamboa Mgtr. | CL | Validar requisitos, aprobar cambios, aceptar y calificar el proyecto |

Los cuatro integrantes forman además el equipo de trabajo (ET), redactan fichas y prueban lo que programan. Cada uno demuestra su aporte con commits y participación en la exposición. Ningún integrante es el único revisor de su propio trabajo.

## Ciclo de vida

Ágil con tres sprints entre el 25 de noviembre y el 8 de diciembre de 2026.

## Tareas, estimaciones y calendario

Ver [backlog](../05-backlog/backlog.md) y [cronograma](../05-backlog/cronograma.md).

## Recursos

Equipos de los integrantes, equipo de laboratorio para pruebas de rendimiento, GitHub, fuentes oficiales de ISO.

## Riesgos

| Riesgo | Prob. | Impacto | Respuesta |
|---|---|---|---|
| Plazo de dos semanas insuficiente | Alta | Alto | Terminar M1 a M5 antes de M6 y M7 |
| No tener acceso al texto de las normas para completar las listas, sobre todo 5-1-2 | Alta | Alto | Consultar PAS y copia institucional en los primeros dos días |
| La investigación de 14 fichas retrasa la construcción | Media | Alto | Repartir desde el día 1 y trabajar en YAML en paralelo |
| Enlaces rotos al entregar | Media | Medio | Verificarlos y fecharlos antes del cierre |
| Copia textual de documentos ISO | Baja | Alto | Paráfrasis, cita y revisión cruzada |
| Instalación falla en otro equipo | Media | Medio | Probar el manual antes del último día |

## Control de versiones

- Rama `main` siempre ejecutable; una rama por historia (`feature/HU-13-marcar-items`).
- Pull request revisado por otro integrante.
- Mensajes de commit con el ID de la historia.
- Solo I2 integra migraciones de la app `evaluaciones`, para evitar conflictos.
- La plantilla de la ficha es de I3. Las plantillas de la lista son de I1 hasta cerrar HU-12 y después de I2.
- Etiqueta `v1.0` en la entrega.

## Respaldo

Repositorio en GitHub y una copia periódica adicional (por ejemplo, ZIP o `git bundle`) registrada en los [reportes de avance](04-reportes-de-avance.md).
