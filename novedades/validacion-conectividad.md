# Validación de conectividad en sincronización

**Periodo:** abril 2026

## Qué cambió

Los recolectores en campo veían a veces un error de sincronización tras varios
intentos fallidos. Al investigar, se detectó que en muchos casos no era un error
del sistema, sino que el teléfono aparecía conectado (WiFi o datos) pero sin
acceso real a internet —por ejemplo, una red WiFi sin salida a internet o una
señal inestable en zonas rurales. Ahora la app comprueba que exista conexión real
antes de intentar sincronizar.

## Qué ve el usuario

- Si no hay conexión real a internet, la app muestra un aviso claro de "sin
  conexión" en vez de un error confuso.
- El botón **Sincronizar todo** sigue disponible siempre, sin límite de intentos
  fallidos que bloquee su uso.
- Cuando la conexión vuelve, la sincronización puede reintentarse con normalidad.

## Beneficio

Menos errores confusos para el recolector, menos llamadas de soporte por
"errores de sincronización" que en realidad eran de cobertura, y mejor
diagnóstico para el equipo que da soporte en campo.
