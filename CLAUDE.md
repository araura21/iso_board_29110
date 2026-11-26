# CLAUDE.md

## Proyecto

iso_board_29110: aplicación web con biblioteca digital, listas de verificación y tablero de estado de la familia ISO/IEC 29110. Proyecto académico de Aseguramiento de la Calidad del Software (ESPE), equipo de 4. Plazo: 25 de noviembre al 8 de diciembre de 2026.

Estado actual: solo documentación, sin código.

## Fuentes de verdad

1. `docs/source/Guia_Actividad_ISO_29110_ESPE.pdf` (manda ante cualquier contradicción, salvo en tamaño del equipo, que es de 4, y plazo).
2. `docs/`, con índice en `docs/README.md`.

Leer antes de trabajar en cada tema:

| Tema | Documento |
|---|---|
| Requisitos | `docs/01-requisitos/` |
| Cálculo, estados y roles | `docs/01-requisitos/reglas-de-negocio.md` |
| Arquitectura y stack | `docs/02-arquitectura/` |
| Datos y carga YAML | `docs/03-base-de-datos/` |
| Contenido de las normas | `docs/04-contenido/` |
| Historias y prioridad | `docs/05-backlog/` |
| Decisiones | `docs/06-decisiones/` |
| Pruebas | `docs/07-pruebas/plan-pruebas.md` |

## Stack

Python 3.12, Django 5.2 LTS, SQLite, plantillas Django con Bootstrap 5 y HTMX, Chart.js, ReportLab, openpyxl, PyYAML, pytest y pytest-django. Detalle en `docs/02-arquitectura/stack.md`.

Los vacíos de la guía ya resueltos están en `docs/06-decisiones/pendientes.md`.

Al crear el proyecto (HU-01), añadir aquí los comandos reales de instalación, ejecución, importación de contenido y pruebas.

## Reglas de arquitectura

- Monolito con tres capas: presentación, negocio y datos. Estructura en `docs/02-arquitectura/arquitectura.md`.
- Vistas y plantillas no calculan porcentajes ni estados.
- El cálculo y el estado son funciones puras con pruebas unitarias.
- Familias, normas, procesos, perfiles e ítems son datos. No escribir códigos de la 29110 fijos en la lógica: otra familia debe registrarse sin tocar código.
- Los YAML de `contenido/` son la fuente oficial; el importador es idempotente y no borra evaluaciones.

## Reglas de negocio que no se rompen

- Cumplimiento = (C + 0,5 × P) / (T − NA) × 100. Los ítems sin respuesta cuentan en T.
- Estados: No iniciado, En inicio (menos de 40), En progreso (menos de 80), Casi conforme (menos de 100), Conforme (100 con evidencia). Comparar sin redondear. Casos límite en RN-02.
- Permisos verificados en el servidor. Contraseñas solo con hash.
- Evidencias: validar tamaño y extensión; enlaces solo `http` o `https`.

## Contenido y derechos de autor

- No copiar texto de documentos ISO. Paráfrasis propia con fuente.
- No guardar ni redistribuir documentos de pago, tampoco en el repositorio.
- Cada enlace oficial indica acceso gratuito, de pago o institucional.
- No inventar enlaces, ediciones, tareas de una norma ni citas. Si falta la fuente, dejar el campo vacío y avisar.

## Prioridad

Terminar M1 a M5 (obligatorios para aprobar) antes de M6 y M7. La autenticación y los roles van en la base (E0).

## Calidad

- Objetivos: marcar un ítem en menos de 3 clics desde la ficha; ficha y lista cargan en menos de 2 s; contraste legible, textos alternativos y navegación con teclado.
- Interfaz y documentación en español. Comentarios en los módulos principales.
- Una historia está terminada con criterios de aceptación cumplidos, pruebas en verde, pull request revisado por otro integrante y `docs/01-requisitos/trazabilidad.md` actualizada.

## Git

- `main` siempre ejecutable. Rama por historia: `feature/HU-13-marcar-items`.
- Mensaje de commit con el ID de la historia.
- Nunca subir secretos, la base de datos ni archivos de evidencias.

## Evidencias ISO/IEC 29110

El propio proyecto se evalúa con el Perfil Básico (`docs/08-gestion-29110/`).

- Al completar una historia, actualizar backlog y trazabilidad.
- Un cambio de alcance se registra como solicitud de cambio.
- No inventar actas, firmas, fechas, resultados de pruebas ni validaciones del cliente.
- La guía exige declarar el uso de IA: anotar cada sesión relevante en `docs/09-entrega/normas-presentacion.md`.
