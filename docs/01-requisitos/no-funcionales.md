# Requisitos no funcionales

Atributo y criterio vienen de la tabla 3 de la guía. La forma de verificación es una propuesta.

| Código | Atributo | Criterio de aceptación | Cómo se verifica |
|---|---|---|---|
| RNF-01 | Usabilidad | Un usuario nuevo marca un ítem de la lista de verificación en menos de tres clics desde la ficha de la norma. | Recorrido con una persona ajena al equipo; contar clics (máximo 2). |
| RNF-02 | Persistencia | Las evaluaciones se conservan al cerrar y volver a abrir el sistema (base de datos o archivo estructurado). | Registrar, reiniciar el servidor y consultar. |
| RNF-03 | Seguridad | Acceso con usuario y contraseña cifrada; los roles limitan quién edita contenido y quién solo consulta. | Pruebas automatizadas de permisos; revisar que la base no guarda texto plano. |
| RNF-04 | Rendimiento | La ficha de una norma y su lista de verificación cargan en menos de dos segundos en un equipo de laboratorio. | Medir en las herramientas del navegador con los datos completos. |
| RNF-05 | Mantenibilidad | Código versionado en Git, con README, instrucciones de instalación y comentarios en los módulos principales. | Revisión del repositorio antes de entregar. |
| RNF-06 | Portabilidad | El sistema se instala y ejecuta siguiendo el manual técnico en un equipo distinto al de desarrollo. | Instalación limpia en otra máquina siguiendo solo el manual. |
| RNF-07 | Accesibilidad | Contraste legible, textos alternativos en imágenes y navegación básica con teclado. | Recorrido con teclado y auditoría de accesibilidad del navegador. |

## Restricciones técnicas de la guía

| Restricción | Sección |
|---|---|
| Aplicación web, lenguaje libre y justificado en el informe técnico | 4.1 |
| Repositorio en GitHub con documentación y README de uso | 4.1 |
| Estructura de datos extensible a otras familias de normas sin tocar código | 4.1 |
| Al menos tres capas: presentación, lógica de negocio y datos | 4.8 |
| Contenido en base de datos, JSON o YAML, corregible sin recompilar (sugerido) | 4.8 |
| Pruebas automatizadas del cálculo y del estado (se valora) | 4.8 |
