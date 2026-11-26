# Documento de mantenimiento

Versión: 0.1 (borrador). Explica cómo corregir, actualizar y ampliar iso_board_29110 después de la entrega. Respalda el ítem IS.6.1 y se completa en HU-25.

Lo marcado como "Pendiente" se escribe cuando exista el código.

## Estructura del sistema

Monolito web en capas con Python, Django y SQLite. Ver [arquitectura](../02-arquitectura/arquitectura.md), [stack](../02-arquitectura/stack.md) y [modelo de datos](../03-base-de-datos/modelo-datos.md).

## Entorno de desarrollo

- Python 3.12 (Django 5.2 necesita 3.10 o superior).
- Dependencias y versiones: Pendiente.
- Comandos de instalación, ejecución, migraciones y pruebas: Pendiente.

## Contenido de las normas

Los YAML de `contenido/` son la fuente oficial. Para corregir una norma, editar su YAML y volver a importar según las [reglas de carga](../03-base-de-datos/carga-contenido.md). Una familia nueva se registra desde administración sin cambiar código (HU-21).

- Comando de importación: Pendiente.
- Revisión de enlaces oficiales y de su fecha de verificación: Pendiente.

## Operación

- Despliegue en la URL: Pendiente.
- Variables de entorno (sin valores secretos): Pendiente.
- Copia y restauración de la base de datos y de las evidencias: Pendiente.
- Alta y baja de usuarios: Pendiente.

## Cómo hacer un cambio

1. Registrar la [solicitud de cambio](../08-gestion-29110/05-solicitudes-de-cambio.md) si modifica el alcance.
2. Crear una rama a partir de `main`.
3. Programar el cambio con sus pruebas.
4. Actualizar requisitos y [trazabilidad](../01-requisitos/trazabilidad.md).
5. Abrir un pull request revisado por otra persona.
6. Etiquetar la nueva versión y desplegar.

## Problemas conocidos

Pendiente: limitaciones y errores abiertos al cierre, con su solución temporal.
