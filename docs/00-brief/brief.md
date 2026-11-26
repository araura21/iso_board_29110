# Brief del proyecto

## Datos de la actividad

| Campo | Información |
|---|---|
| Universidad | Universidad de las Fuerzas Armadas ESPE |
| Departamento y carrera | Ciencias de la Computación, Ingeniería de Software |
| Actividad | Proyecto final del parcial 2 |
| Asignatura | Aseguramiento de la Calidad del Software |
| Unidad | Normas para entidades muy pequeñas (VSE): ISO/IEC 29110 |
| Tipo | Proyecto práctico de desarrollo (aprendizaje basado en proyectos) |
| Modalidad | Grupal, 4 estudiantes |
| Duración | Dos semanas, del 25 de noviembre al 8 de diciembre de 2026 ([cronograma](../05-backlog/cronograma.md)) |
| Docente | Ing. Diego Gamboa Mgtr. |
| NRC / paralelo | 36844/5 |
| Fecha de entrega | Según plataforma Moodle |
| Fecha de la guía | Sangolquí, noviembre de 2026 |

## Contexto

La familia ISO/IEC 29110 reúne normas, informes técnicos y guías para entidades muy pequeñas (VSE): empresas, departamentos, proyectos u organizaciones que desarrollan software o sistemas con un equipo de hasta 25 personas. Ofrece perfiles de ciclo de vida progresivos, fáciles de adoptar y adaptados a sus límites de tiempo, presupuesto y conocimiento (Laporte, 2016).

A diferencia de normas extensas como ISO/IEC/IEEE 12207, la serie organiza sus documentos por audiencia:

| Documentos | Para qué sirven o a quién van dirigidos |
|---|---|
| Visión general y vocabulario | Todos los interesados |
| Especificaciones de perfil | Indican qué hacer |
| Guías de gestión e ingeniería | Explican cómo hacerlo |
| Evaluación y certificación | Evaluadores y auditores |

En 2024 se publicaron las nuevas partes 1-1 y 1-2, que reemplazaron al informe técnico de 2016 y actualizaron la estructura de la serie (ISO/IEC, 2024a). En 2025 se publicaron la guía de desarrollo ágil (parte 5-4) y una enmienda al esquema de certificación que elimina la recertificación cada tres años (ISO/IEC, 2025b). Por eso hacen falta herramientas para consultar cada parte y verificar su grado de aplicación de forma ordenada y trazable.

## Producto

iso_board_29110 (llamado provisionalmente «ISO-Guía 29110» en la guía) es una aplicación web que funciona como guía digital de la familia y como herramienta de autoevaluación. Permite conocer cada parte, acceder a su documento oficial y registrar apartado por apartado si una organización cumple lo que la norma establece.

## Objetivo general

Desarrollar un sistema informático que presente de forma automatizada la información de cada parte de la familia ISO/IEC 29110, permita acceder a su documento oficial y gestione listas de verificación para determinar el estado de aplicación de cada norma en una organización.

## Objetivos específicos

| Código | Objetivo | Módulos |
|---|---|---|
| OE1 | Construir una biblioteca digital tipo libro o guía que describa el propósito, la audiencia, el contenido y la relación de cada parte. | M1, M2 |
| OE2 | Implementar un mecanismo de descarga o acceso al documento de cada norma que respete los derechos de autor de ISO e IEC. | M3 |
| OE3 | Diseñar listas de verificación interactivas por parte, donde el usuario marque el cumplimiento de cada apartado y adjunte evidencias. | M4 |
| OE4 | Calcular y visualizar el porcentaje de cumplimiento y el estado de aplicación de cada norma en un tablero de control. | M5 |
| OE5 | Aplicar las prácticas del Perfil Básico en la gestión e implementación del propio proyecto. | [Gestión](../08-gestion-29110/README.md) |

## Resultados de aprendizaje

Al finalizar, cada estudiante podrá:

- Explicar la estructura de la familia ISO/IEC 29110, sus perfiles y la audiencia de cada documento.
- Traducir los requisitos de una norma en elementos verificables de una lista de comprobación.
- Diseñar e implementar un sistema con persistencia de datos, cálculo de indicadores y generación de reportes.
- Producir evidencias de los procesos de Gestión del Proyecto (GP) e Implementación de Software (IS) del Perfil Básico.

## Alcance

Dentro del alcance:

- Todas las partes de la familia listadas en [familia-29110.md](../04-contenido/familia-29110.md).
- Aplicación web en el lenguaje que elija el equipo, con la elección justificada en el informe técnico.
- Código, documentación y README de uso publicados en GitHub.
- Diseño extensible: otras familias de normas (ISO 9001, ISO/IEC 25010) se registran desde administración sin modificar código.
- Separación en al menos tres capas: presentación, lógica de negocio y datos.

Fuera del alcance:

- Almacenar o redistribuir copias de documentos de pago.
- Emitir certificaciones. Los estados del sistema son una convención académica y no sustituyen el dictamen de un organismo certificador acreditado.

## Prioridad de entrega

Los módulos M1 a M5 son indispensables para aprobar. M6 y M7 completan la calificación máxima.

## Usuarios

| Rol | Uso del sistema |
|---|---|
| Administrador | Gestiona normas, apartados, ítems y usuarios |
| Evaluador | Registra evaluaciones, respuestas y evidencias |
| Consultor | Consulta sin editar |

La guía nombra los tres roles. Los permisos de cada uno están en [reglas de negocio](../01-requisitos/reglas-de-negocio.md).

## Referencias

- ISO/IEC. (2024a). *ISO/IEC 29110-1-1:2024. Systems and software engineering — Lifecycle profiles for very small entities (VSEs) — Part 1-1: Overview*. International Organization for Standardization. https://www.iso.org/standard/85337.html
- ISO/IEC. (2024b). *ISO/IEC 29110-1-2:2024. Systems and software engineering — Lifecycle profiles for very small entities (VSEs) — Part 1-2: Vocabulary*. International Organization for Standardization.
- ISO/IEC. (2025a). *ISO/IEC 29110-3-2:2018/Amd 1:2025. Systems and software engineering — Lifecycle profiles for very small entities (VSEs) — Part 3-2: Conformity certification scheme — Amendment 1*. International Organization for Standardization. https://www.iso.org/standard/62732.html
- ISO/IEC. (2025b). *ISO/IEC 29110-5-4:2025. Systems and software engineering — Life cycle profiles for very small entities (VSEs) — Part 5-4: Agile software development guidelines*. International Organization for Standardization. https://www.iso.org/standard/82668.html
- Laporte, C. Y. (2016). *ISO/IEC 29110: Normas y guías de ingeniería de software y sistemas para entidades muy pequeñas* [Presentación]. Convención Informática 2016, La Habana, Cuba.
