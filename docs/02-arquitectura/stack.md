# Stack tecnológico

El sistema se desarrolla con Python y Django. Las razones frente a otras opciones están en [ADR-002](../06-decisiones/adr-002-stack.md).

| Componente | Tecnología | Motivo |
|---|---|---|
| Lenguaje | Python 3.12 | Permitido por la guía |
| Framework web | Django 5.2 LTS | Trae autenticación con contraseñas cifradas, ORM, formularios y panel de administración (RNF-03, M7) |
| Base de datos | SQLite | Un solo archivo, sin servidor; facilita la instalación en otro equipo (RNF-02, RNF-06) |
| Interfaz | Plantillas Django, Bootstrap 5, HTMX | Marcar ítems sin recargar la página y sin un frontend separado |
| Gráficos | Chart.js | Gráficos del tablero (RF-11) |
| Mapa de la familia | SVG generado en plantilla | Nodos enlazables y navegables con teclado (RF-03, RNF-07) |
| Reportes PDF | ReportLab | Se instala con pip en Windows sin dependencias del sistema |
| Hoja de cálculo | openpyxl | Exportación `.xlsx` (RF-13) |
| Contenido | YAML con PyYAML | El docente revisa y corrige sin recompilar |
| Pruebas | pytest y pytest-django | Cálculo y estados automatizados |
| Control de versiones | Git y GitHub | Exigido por la guía |

## Despliegue

El sistema se entrega en una URL desplegada. El alojamiento debe conservar en disco la base SQLite y las evidencias; el proveedor se elige antes de HU-28.

## Requisito de instalación

Django 5.2 necesita Python 3.10 o superior. Cada integrante debe revisar su versión con `python --version` antes de empezar.

