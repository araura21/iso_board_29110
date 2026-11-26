# Documentación del proyecto iso_board_29110

Sistema web que funciona como biblioteca digital, lista de verificación y tablero de estado de la familia ISO/IEC 29110. La fuente de todos los requisitos es la [guía de actividad](source/Guia_Actividad_ISO_29110_ESPE.pdf). Si un documento de esta carpeta la contradice, manda la guía, salvo en el tamaño del equipo (4 estudiantes) y el plazo (25 de noviembre al 8 de diciembre de 2026).

## Dónde encontrar cada cosa

| Necesito saber... | Documento |
|---|---|
| Qué se construye, para quién y con qué objetivos | [Brief del proyecto](00-brief/brief.md) |
| Qué significa un término o una sigla | [Glosario](00-brief/glosario.md) |
| Qué debe hacer el sistema | [Requisitos funcionales](01-requisitos/funcionales.md) |
| Qué calidad debe tener | [Requisitos no funcionales](01-requisitos/no-funcionales.md) |
| Cómo se calcula el porcentaje y el estado | [Reglas de negocio](01-requisitos/reglas-de-negocio.md) |
| Qué requisito cubre cada módulo, historia y prueba | [Trazabilidad](01-requisitos/trazabilidad.md) |
| Capas, componentes y estructura de carpetas | [Arquitectura](02-arquitectura/arquitectura.md) |
| Tecnologías y su justificación | [Stack](02-arquitectura/stack.md) |
| Entidades, relaciones y campos | [Modelo de datos](03-base-de-datos/modelo-datos.md) |
| Cómo se carga el contenido de las normas | [Carga de contenido](03-base-de-datos/carga-contenido.md) |
| Las partes de la familia que hay que cargar | [Familia ISO/IEC 29110](04-contenido/familia-29110.md) |
| Los ítems de las listas de verificación | [Listas de verificación](04-contenido/listas-verificacion.md) |
| Qué se puede enlazar y qué no | [Derechos de autor](04-contenido/derechos-de-autor.md) |
| Módulos M1 a M7 | [Módulos](05-backlog/modulos.md) |
| Historias de usuario | [Backlog](05-backlog/backlog.md) |
| Fechas y fases | [Cronograma](05-backlog/cronograma.md) |
| Decisiones tomadas y pendientes | [Decisiones](06-decisiones/README.md) |
| Cómo se prueba | [Plan de pruebas](07-pruebas/plan-pruebas.md) |
| Evidencias del Perfil Básico (GP e IS) | [Gestión ISO 29110](08-gestion-29110/README.md) |
| Qué se entrega y cómo se califica | [Entregables y rúbrica](09-entrega/entregables-rubrica.md) |
| Cómo mantener el sistema después de la entrega | [Documento de mantenimiento](09-entrega/documento-mantenimiento.md) |
| Formato, integridad académica y uso de IA | [Normas de presentación](09-entrega/normas-presentacion.md) |

## Antes de programar

1. Revisar las reglas acordadas en el [registro de pendientes](06-decisiones/pendientes.md).
2. Consultar los roles de cada integrante en el [plan del proyecto](08-gestion-29110/02-plan-del-proyecto.md).
3. Empezar por la épica E0 del [backlog](05-backlog/backlog.md).

## Mantenimiento

Cada cambio de alcance se registra como [solicitud de cambio](08-gestion-29110/05-solicitudes-de-cambio.md) y se actualizan el requisito, el backlog y la trazabilidad en el mismo commit.
