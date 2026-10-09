# Indicadores de sincronización

**Periodo:** marzo 2026

## Qué cambió

Durante la validación en campo se detectó que algunas fotografías podían perderse
o quedar inconsistentes al sincronizarse, especialmente sin conexión estable.
Esta entrega corrigió esa pérdida de datos y agregó indicadores (KPIs) de éxito y
fallos de sincronización para dar visibilidad al equipo de negocio.

## Qué ve el usuario

- En el panel de administración, nuevas tarjetas y gráficas muestran la tasa de
  éxito de sincronización y el estado general de las actividades por proyecto.
- En la app móvil, una actividad ya no se envía como completa hasta que todas
  sus imágenes estén efectivamente respaldadas en el servidor.

## Beneficio

Visibilidad clara y confiable sobre la estabilidad de la sincronización para el
equipo de negocio, y la garantía de que ninguna imagen capturada en campo se
pierde por una incidencia de red. En las pruebas de validación, se confirmó una
tasa de éxito del 100% sobre un lote real de evidencia fotográfica.
