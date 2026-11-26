# ADR-003: Contenido en YAML importado a la base

Fecha: 2026-11-25.

## Contexto

La guía sugiere guardar normas y listas en la base de datos o en JSON o YAML, para que el docente corrija sin recompilar. También exige administrarlas desde el sistema (M7) y registrar nuevas familias sin cambiar código.

## Decisión

YAML versionado para la carga inicial, importado a la base con un comando. La aplicación lee solo de la base. Los YAML son la fuente oficial del contenido que describen.

## Alternativas

- Solo base de datos: la revisión del contenido en Git se pierde.
- Solo archivos: la administración y las relaciones con respuestas se complican.

## Consecuencias

El equipo puede redactar fichas en paralelo y revisarlas en pull requests. Hay que evitar que una reimportación pise cambios hechos en administración.
