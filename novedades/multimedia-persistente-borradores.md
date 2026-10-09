# Multimedia persistente y borradores

**Periodo:** mayo 2026

## Qué cambió

Antes, si la app se cerraba, pasaba a segundo plano o la sincronización se
retrasaba, existía riesgo de perder las fotos, videos o avances de un formulario
que el recolector estaba llenando en campo. Con esta entrega, una actividad en
progreso se puede guardar como borrador y retomar más tarde sin perder nada de lo
ya registrado.

## Qué ve el usuario

- La evidencia (foto, video, selfie o firma) queda protegida desde el momento en
  que se agrega, aunque la sincronización ocurra después.
- El formulario se puede guardar manualmente con el botón **Guardar borrador**.
- La app guarda automáticamente los cambios reales cada pocos minutos.
- Si la app se minimiza o pasa a segundo plano, el borrador se guarda de inmediato.
- Al reabrir un borrador desde **Pendientes**, se recuperan las respuestas y la
  multimedia tal como se dejaron.
- Si hay cambios sin guardar al salir del formulario, se pregunta antes de
  descartarlos; si no hay cambios nuevos, se sale directo.

## Beneficio

Menos pérdida de evidencia capturada en campo, menos reprocesos por cierres
inesperados o cortes de conectividad, y continuidad real del trabajo cuando una
actividad no se puede completar en una sola sesión.
