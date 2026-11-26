# ADR-001: Monolito web en capas

Fecha: 2026-11-25.

## Contexto

Equipo de cuatro personas y plazo de dos semanas. La guía exige separar presentación, lógica de negocio y datos.

## Decisión

Una sola aplicación web, organizada por módulos, con las tres capas separadas y el cálculo de cumplimiento en funciones puras.

## Alternativas

API y frontend separados: dos proyectos que configurar, desplegar y documentar en el mismo plazo.

## Consecuencias

Instalación y despliegue simples. La separación en capas depende de la disciplina del equipo y se revisa en cada pull request.
