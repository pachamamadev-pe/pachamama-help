# Verificación pública de trazabilidad

**Periodo:** mayo 2026

## Qué cambió

La página pública de un lote ya mostraba su historia de trazabilidad, pero no había
forma de confirmar, desde esa misma página, que la información seguía coincidiendo
con el registro validado por la plataforma. Ahora, al final de la página pública de
cada lote, aparece un bloque de verificación que confirma:

- Que la composición del lote coincide con el registro validado.
- Que el contenido visible en la página sigue coincidiendo con lo que la
  plataforma espera mostrar para ese lote.

## Qué ve el usuario

Un mensaje claro al final de la página del lote, con uno de estos estados:

| Estado | Significado para quien consulta el lote |
|---|---|
| Verificado | La información coincide con el registro validado. |
| Advertencia | Se detectó una diferencia que requiere revisión. |
| No disponible | La verificación todavía no está lista para ese lote. |
| Desconocido | No fue posible determinar el resultado en ese momento. |

## Beneficio

Cualquier persona que consulte un lote —cliente, auditor o consumidor final— puede
confiar en que la trazabilidad mostrada es verificable y no solo informativa,
sin necesidad de conocimientos técnicos.
