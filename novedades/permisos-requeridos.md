# Permisos obligatorios en la app móvil

**Periodo:** abril 2026

## Qué cambió

Se detectó que, si un recolector no concedía los permisos necesarios (cámara,
ubicación, almacenamiento o notificaciones), la app podía fallar en silencio o
mostrar mensajes técnicos confusos: actividades sin coordenadas, sin foto, o sin
alertas del sistema. Ahora la app no permite avanzar hasta que todos los permisos
indispensables estén concedidos, y guía al usuario para resolverlo.

## Qué ve el usuario

Una pantalla de bloqueo con dos opciones claras cuando falta un permiso:

- **Reintentar pedir permisos** — vuelve a mostrar el diálogo estándar de Android.
- **Abrir ajustes del sistema** — lleva directo a la pantalla de permisos de la
  app, para los casos en que Android ya no vuelve a preguntar automáticamente.

## Beneficio

Ninguna actividad se registra sin poder tomar foto o georreferenciar
correctamente, y el recolector puede resolver el problema por sí mismo sin
necesitar asistencia técnica.
