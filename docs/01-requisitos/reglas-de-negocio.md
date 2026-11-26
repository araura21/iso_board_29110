# Reglas de negocio

## RN-01 Porcentaje de cumplimiento

```
Cumplimiento (%) = [ (C + 0,5 × P) / (T − NA) ] × 100
```

| Símbolo | Significado |
|---|---|
| C | Ítems que cumplen |
| P | Ítems que cumplen parcialmente (valen la mitad) |
| T | Total de ítems de la norma |
| NA | Ítems que no aplican (se excluyen del cálculo) |

Un ítem sin respuesta cuenta en T y no suma.

## RN-02 Estado de aplicación

| Cumplimiento | Estado | Interpretación |
|---|---|---|
| 0 % (sin ítems evaluados) | No iniciado | La organización aún no ha revisado la norma. |
| 1 % a 39 % | En inicio | Existen prácticas aisladas; se requiere un plan de implantación. |
| 40 % a 79 % | En progreso | La mayoría de las prácticas está en marcha; persisten brechas relevantes. |
| 80 % a 99 % | Casi conforme | Faltan ajustes menores antes de una evaluación formal. |
| 100 % | Conforme | Todos los ítems aplicables se cumplen con evidencia; listo para evaluación o auditoría. |

Los rangos son una convención académica de la actividad.

## Agregados

| Nivel | Cálculo |
|---|---|
| Por proceso | Fórmula de RN-01 sobre los ítems del proceso |
| Por organización | Fórmula de RN-01 sobre la suma de ítems de la última evaluación de cada norma |

## Casos límite

Complementan la tabla de la guía, que no los define.

| Caso | Regla |
|---|---|
| Ninguna respuesta | No iniciado. |
| Valores entre rangos (39,75 %, 79,9 %) | Comparar sin redondear: menos de 40 es En inicio, menos de 80 es En progreso, menos de 100 es Casi conforme. Mostrar un decimal truncado. |
| Ítems evaluados con resultado 0 % (todos NC) | En inicio, porque la norma sí fue revisada. |
| Mayor que 0 % y menor que 1 % | En inicio. |
| Todos los ítems NA (T − NA = 0) | No calcular; mostrar "Sin ítems aplicables". |
| 100 % con ítems C sin evidencia | Mostrar 100 % con estado Casi conforme y la lista de evidencias que faltan. Al adjuntarlas pasa a Conforme. |

## RN-03 Brechas

Una brecha es un ítem con valor NC o P. Cada brecha admite una acción de mejora (RF-12).

## RN-04 Permisos por rol

El acceso se controla por rol. Cada permiso se verifica en el servidor y tiene prueba automatizada.

| Acción | Administrador | Evaluador | Consultor |
|---|---|---|---|
| Consultar biblioteca, fichas y tablero | Sí | Sí | Sí |
| Registrar organizaciones y evaluaciones | Sí | Sí | No |
| Exportar reportes | Sí | Sí | Sí |
| Administrar normas, apartados, ítems y usuarios | Sí | No | No |

## RN-05 Acceso a documentos

Ver [derechos de autor](../04-contenido/derechos-de-autor.md). El sistema nunca almacena ni redistribuye documentos de pago.

## RN-06 Listas de verificación

- Cada parte tiene su propia lista.
- La lista de 29110-5-1-2 incluye todas las tareas de la norma, partiendo de los ítems mínimos.
- Las demás partes tienen al menos cinco ítems cada una.
