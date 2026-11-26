# Carga de contenido

Las normas y listas se mantienen en archivos YAML versionados, uno por norma, y un comando los importa a la base de datos ([ADR-003](../06-decisiones/adr-003-contenido-yaml.md)). Así el docente puede revisar y corregir la información sin recompilar.

## Formato

Archivo `contenido/iso-29110/29110-5-1-2.yaml`:

```yaml
familia: ISO/IEC 29110
norma:
  codigo: 29110-5-1-2
  titulo: Guía del Perfil Básico
  edicion: "2011"
  tipo: guias
  audiencia: ""
  perfiles: [Básico]
  proposito: Procesos GP e IS para una VSE con un proyecto a la vez.
  introduccion: ""        # redacción propia
  contenido_principal: ""
  fuentes: []
  normas_vinculadas: []
  enlace_oficial: ""
  tipo_acceso: ""         # gratuito | pago | institucional
  enlace_verificado_el: null
apartados:
  - codigo: GP
    nombre: Gestión del Proyecto
    tipo: proceso
    apartados:
      - codigo: GP.1
        nombre: ""        # tomar de la norma
        tipo: actividad
        items:
          - codigo: GP.1.1
            enunciado: Se revisó el Enunciado del trabajo y se definieron con el cliente las instrucciones de entrega.
            producto_esperado: Enunciado del trabajo [revisado]; Plan del proyecto
            roles: [GP, LT, CL]
```

## Reglas del importador

- Se puede ejecutar varias veces: actualiza por código y no duplica.
- Rechaza códigos repetidos y campos obligatorios vacíos.
- No borra respuestas ni evaluaciones existentes.
- Solo actualiza los registros presentes en los YAML; las familias creadas desde administración no se tocan.

## Fuente oficial

Los archivos YAML son la fuente oficial del contenido que describen. Las correcciones se hacen en el YAML y se reimportan; un cambio hecho desde administración sobre uno de esos registros se pierde en la siguiente importación si no se copia al YAML.
