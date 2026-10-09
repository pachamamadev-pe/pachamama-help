# Flujos Comunes - Pachamama Web Admin

[Volver al manual principal](guia-definitiva-negocio.md)

**Dirigido a:** Todos los usuarios de la web admin  
**Objetivo:** Explicar los flujos que comparten varios roles

---

## Índice

1. [Login y primer acceso](#login-y-primer-acceso)
2. [Recuperación de contraseña y verificación de correo](#recuperacion-de-contrasena-y-verificacion-de-correo)
3. [Sidebar, header y cierre de sesión](#sidebar-header-y-cierre-de-sesion)
4. [Inicio y dashboard](#inicio-y-dashboard)
5. [Mi perfil y seguridad](#mi-perfil-y-seguridad)
6. [Módulo Proyectos](#modulo-proyectos)
7. [Detalle de proyecto y avance de etapas](#detalle-de-proyecto-y-avance-de-etapas)
8. [Gestión de mapa](#gestion-de-mapa)
9. [Documentos de proyecto](#documentos-de-proyecto)
10. [Registro de actividades y evaluaciones](#registro-de-actividades-y-evaluaciones)
11. [Solicitudes de recolección](#solicitudes-de-recoleccion)
12. [Lotes de acopio](#lotes-de-acopio)
13. [Lotes de transformación](#lotes-de-transformacion)
14. [Formularios dinámicos](#formularios-dinamicos)
15. [Errores frecuentes y recomendaciones](#errores-frecuentes-y-recomendaciones)

---

<a id="login-y-primer-acceso"></a>
## 1. Login y primer acceso

### Qué hace el usuario aquí

Ingresa a la plataforma con su correo y contraseña.

### Paso a paso

1. Abrir la web admin.
2. Ingresar correo electrónico.
3. Ingresar contraseña.
4. Presionar `Iniciar sesión`.
5. Esperar a que la plataforma valide correo, permisos y menú.

### Qué verá normalmente

- La pantalla de login con correo, contraseña y opción para mostrar u ocultar la contraseña.
- Un mensaje de carga mientras se valida el acceso.
- Luego, la ruta `Inicio` y el menú lateral si el acceso fue correcto.

### Reglas importantes

- El correo debe estar verificado antes de permitir el ingreso operativo.
- La plataforma limpia una sesión previa antes de iniciar una nueva.
- Si el usuario no tiene módulos habilitados, la sesión se cierra y la web no lo deja operar.

### Qué hacer si falla

- Si el correo no está verificado, revisar el enlace enviado al correo.
- Si aparece un error de autenticación, validar correo y contraseña.
- Si entra pero no tiene ningún módulo disponible, revisar rol y permisos.

---

<a id="recuperacion-de-contrasena-y-verificacion-de-correo"></a>
## 2. Recuperación de contraseña y verificación de correo

### Qué hace el usuario aquí

Recupera acceso o completa la validación del correo antes de ingresar.

### Paso a paso para restablecer contraseña

1. En la pantalla de login, escribir el correo.
2. Elegir la opción de recuperación.
3. Revisar el correo recibido.
4. Abrir el enlace de restablecimiento.
5. Definir una nueva contraseña.

### Qué debe saber el usuario

- La recuperación de contraseña necesita que el correo esté escrito antes de pedir el enlace.
- Si el usuario cambia de correo desde administración, deberá volver a validarlo.
- Un usuario nuevo no entra al sistema hasta completar la verificación de correo.

### Qué hacer si falla

- Revisar carpeta de spam o correo no deseado.
- Confirmar que el correo ingresado sea el correcto.
- Si no llega el enlace, pedir validación al administrador de empresa.

---

<a id="sidebar-header-y-cierre-de-sesion"></a>
## 3. Sidebar, header y cierre de sesión

### Qué encuentra el usuario aquí

La estructura principal de navegación de toda la plataforma.

### Qué verá normalmente

- Un `Sidebar` con solo los módulos habilitados para su usuario.
- Un `Header` con el título de la pantalla actual.
- El nombre de la empresa en el encabezado.
- Un avatar con acceso a `Mi perfil` y `Cerrar sesión`.

### Cómo usar esta zona

1. Elegir un módulo desde el menú lateral.
2. Revisar el título de la pantalla en el encabezado.
3. Abrir el menú de usuario si necesita entrar a perfil o cerrar sesión.

### Qué debe entender el usuario

- El menú no es fijo: depende del rol y permisos.
- Si un módulo no aparece, no debe asumirse que es un error visual.
- En móvil, el sidebar se abre y cierra como panel lateral.

### Qué hacer si falla

- Si el menú carga incompleto o vacío, volver a iniciar sesión.
- Si un módulo esperado no aparece, revisar permisos antes de reportar falla.

---

<a id="inicio-y-dashboard"></a>
## 4. Inicio y dashboard

### Qué hace el usuario aquí

Revisa indicadores generales de negocio y accede al trabajo diario.

### Qué verá normalmente

- Una bienvenida con su nombre y rol.
- Dashboard empresarial si su usuario tiene permiso para verlo.
- Tarjetas, gráficos y métricas por fecha.
- Un modal obligatorio de cambio de contraseña si aún no actualizó su clave.

### Paso a paso

1. Entrar a `Inicio`.
2. Revisar la fecha de corte del dashboard.
3. Ajustar la fecha si necesita otra lectura.
4. Usar `refresh` para recargar indicadores.

### Qué debe saber el usuario

- No todos los roles ven el dashboard empresarial.
- El cambio de contraseña puede ser obligatorio al primer ingreso real.

### Qué hacer si falla

- Si el dashboard no carga, revisar conexión y volver a intentar.
- Si el cambio de contraseña aparece, completarlo antes de continuar.

---

<a id="mi-perfil-y-seguridad"></a>
## 5. Mi perfil y seguridad

### Qué hace el usuario aquí

Actualiza sus datos personales, cambia avatar y modifica su contraseña.

### Paso a paso

1. Abrir el menú del avatar.
2. Entrar a `Mi perfil`.
3. Editar datos personales si hace falta.
4. Subir o eliminar avatar si corresponde.
5. Cambiar contraseña ingresando la actual y la nueva.

### Qué verá normalmente

- Datos personales cargados desde el backend.
- Un formulario de edición controlada.
- Un componente de carga de imagen para avatar.
- Un formulario de cambio de contraseña con confirmación.

### Reglas importantes

- El cambio de contraseña exige la contraseña actual.
- Si la contraseña actual es incorrecta, la operación falla.
- Al cambiar la contraseña correctamente, la web marca ese requisito como cumplido.

### Qué hacer si falla

- Si el avatar no carga, volver a intentar o revisar conectividad.
- Si la contraseña no cambia, validar la contraseña actual y que la confirmación coincida.

---

<a id="modulo-proyectos"></a>
## 6. Módulo Proyectos

### Qué hace el usuario aquí

Busca proyectos, aplica filtros y entra al detalle operativo.

### Qué verá normalmente

- Búsqueda por texto.
- Filtros por producto, comunidad y estado.
- Tabla de proyectos con nombre, producto, comunidad, periodo, etapa y estado.
- Acciones de crear, editar o eliminar si su rol lo permite.

### Paso a paso

1. Entrar a `Proyectos`.
2. Buscar por nombre o usar filtros.
3. Abrir el proyecto deseado.
4. Si tiene permisos, crear o editar desde el mismo módulo.

### Qué hacer si falla

- Si no aparecen proyectos, revisar filtros activos.
- Si falta el botón de crear o editar, revisar permisos del rol.

---

<a id="detalle-de-proyecto-y-avance-de-etapas"></a>
## 7. Detalle de proyecto y avance de etapas

### Qué hace el usuario aquí

Opera el proyecto según la etapa en que se encuentra.

### Qué verá normalmente

- Cabecera del proyecto con producto, comunidad, periodo y etapa actual.
- Línea de tiempo de etapas.
- Botón `Avanzar` si el usuario tiene permiso.
- Pestañas operativas según permisos y etapa.

### Pestañas visibles más importantes

| Pestaña | Para qué sirve |
|---|---|
| `Resumen` | Estado general, KPIs y mapa |
| `Recolectores` | Estado del personal y QR de onboarding |
| `Brigadas` | Organización de equipos |
| `Registro de actividades` | Revisión de inventario o recolección |
| `Generar PMF` | Flujo del PMF |
| `Revisión Solicitudes` | Revisar solicitudes de recolección |
| `Lotes de Acopio` | Crear y procesar lotes |
| `Documentos` | Subir, revisar y descargar documentos |
| `Configuración` | Fórmulas y agregaciones |

### Qué bloquea el avance de etapas

| Etapa actual | Bloqueos reales más visibles |
|---|---|
| `planning` | Faltan recolectores, brigadas o documentos obligatorios aprobados |
| `inventory` | No hay actividades registradas |
| `pmf_development` | El PMF aún no está aprobado |
| `serfor_evaluation` | Faltan documentos obligatorios de esa etapa |

### Qué hacer si falla

- Leer el mensaje del tooltip o bloqueo del botón `Avanzar`.
- Revisar primero documentos, actividades y pestañas dependientes de etapa.
- No asumir que el backend avanzará si la UI ya muestra bloqueos pendientes.

---

<a id="gestion-de-mapa"></a>
## 8. Gestión de mapa

### Qué hace el usuario aquí

Carga, visualiza y depura las áreas geográficas del proyecto.

### Paso a paso

1. Entrar a la gestión de mapa del proyecto.
2. Revisar las áreas ya cargadas.
3. Subir nuevos archivos si necesita actualizar el área.
4. Esperar el procesamiento.
5. Ocultar o eliminar áreas si corresponde.

### Formatos y reglas reales

- Se aceptan `ZIP`, `RAR`, `SHP`, `DBF`, `SHX`, `PRJ`, `CPG`, `QMD`, `SBN`, `SBX`, `XML`, `SHP.XML`, `GeoJSON`, `JSON` y `KML`.
- El tamaño máximo por archivo es `150 MB`.
- La importación se procesa en backend y la web consulta el estado cada pocos segundos.
- Si el proceso tarda demasiado, la web corta la espera después de aproximadamente `5 minutos`.
- La edición de áreas solo está habilitada en etapa `planning`.

### Qué verá normalmente

- El mapa del proyecto.
- La lista de áreas cargadas.
- Un indicador de procesamiento cuando sube archivos.

### Qué hacer si falla

- Si el formato no es válido, volver a cargar un archivo permitido.
- Si el archivo pesa demasiado, reducirlo o fragmentarlo.
- Si la etapa ya no es `planning`, la web no permitirá editar.

---

<a id="documentos-de-proyecto"></a>
## 9. Documentos de proyecto

### Qué hace el usuario aquí

Sube, revisa, descarga y resube documentos del proyecto.

### Paso a paso para subir documentos

1. Entrar a la pestaña `Documentos`.
2. Revisar obligatorios pendientes, obligatorios ya subidos y opcionales.
3. Elegir el tipo documental.
4. Seleccionar archivo.
5. Esperar confirmación de carga.

### Qué verá normalmente

- Una tarjeta de progreso documental.
- Una tabla con estado de cada documento.
- Botón `Subir Documentos` si el rol puede cargar.
- Estados como `Pendiente`, `Aprobado`, `Observado` o `Rechazado`.

### Revisión documental

- Aprobar exige notas de validación.
- Observar exige notas.
- Rechazar exige notas.
- Algunos tipos documentales pueden exigir un adjunto de validación adicional.
- Un documento aprobado queda en modo de solo lectura de revisión.

### Regla crítica de PMF

- Si el documento `PMF` es observado mientras el proyecto está en `serfor_evaluation`, el proyecto vuelve a `pmf_development`.

### Resubida

- Un documento observado puede resubirse.
- La nueva carga crea una nueva versión pendiente de revisión.

### Qué hacer si falla

- Si el archivo no sube, revisar formato y tamaño permitidos por ese tipo documental.
- Si no aparece el botón de revisión, revisar permiso `document:review`.
- Si el PMF observado hizo retroceder el proyecto, continuar la corrección desde la etapa anterior.

---

<a id="registro-de-actividades-y-evaluaciones"></a>
## 10. Registro de actividades y evaluaciones

### Qué hace el usuario aquí

Revisa actividades de inventario o recolección enviadas desde la app móvil.

### Qué verá normalmente

- Dos tabs internos: inventario y recolección, según permisos y etapa.
- Filtros por estado.
- Búsqueda por formulario, recolector, código forestal, tipo de actividad o estado.
- Botones `Evaluar` o `Detalle` según el caso.

### Reglas operativas importantes

- Una actividad aprobada pasa a consulta, no a edición.
- En inventario, el botón puede cambiar de `Evaluar` a `Detalle` según etapa y permiso.
- En recolección, la evaluación depende del permiso de revisión correspondiente.
- El botón `Recalcular Columnas` no aparece en etapas avanzadas como `collection`, `ctp_entry` o `primary_transformation`.

### Qué hacer si falla

- Si no aparece una actividad, revisar tab activo, filtros y búsqueda.
- Si el botón `Evaluar` no está disponible, revisar etapa del proyecto y permiso de revisión.

---

<a id="solicitudes-de-recoleccion"></a>
## 11. Solicitudes de recolección

### Qué hace el usuario aquí

Crea, revisa o consulta solicitudes de recolección.

### Paso a paso

1. Entrar al módulo `Solicitudes de Recolección` o a la pestaña de revisión dentro del proyecto.
2. Filtrar por estado si hace falta.
3. Abrir el detalle o revisión.
4. Crear una nueva solicitud si el rol lo permite.
5. Editar solo si la solicitud está `Observada`.

### Qué verá normalmente

- Estados `Pendiente`, `Aprobado`, `Rechazado`, `Observado` y `Cancelado`.
- Un botón `Revisar` para pendientes.
- Un botón `Ver detalles` para estados ya resueltos.

### Reglas reales

- Solo las solicitudes `Observadas` pueden editarse.
- Las pendientes se revisan desde la UI de detalle/revisión.

### Qué hacer si falla

- Si no deja editar, revisar si la solicitud realmente está `Observada`.
- Si no aparece el botón de revisión, revisar permiso `collection_request:review`.

---

<a id="lotes-de-acopio"></a>
## 12. Lotes de acopio

### Qué hace el usuario aquí

Crea lotes desde solicitudes disponibles y genera los documentos del acopio.

### Creación de lote

1. Entrar a la pestaña `Lotes de Acopio`.
2. Elegir `Crear lote`.
3. Seleccionar una solicitud disponible.
4. Completar datos del lote.
5. Confirmar ubicación.
6. Completar datos de transporte.
7. Guardar el lote.

### Qué debe saber sobre ubicación

- La web intenta detectar la ubicación automáticamente.
- Si la geolocalización falla, el usuario puede mover el marcador manualmente.
- Sin ubicación, el lote no puede terminar de crearse.

### Detalle del lote

- El detalle trabaja tres documentos.
- Cuando todos están generados y el lote aún está en borrador, puede finalizarse.
- Un lote en estados avanzados queda en modo de solo lectura.

### Regla de acceso al detalle

- Un lote `draft` requiere permiso de procesamiento.
- Un lote con documentos generados requiere permiso de lectura.

### Qué hacer si falla

- Si no puede crear el lote, revisar solicitud seleccionada, formularios obligatorios y ubicación.
- Si no puede abrir un lote, revisar estado del lote y permiso disponible.

---

<a id="lotes-de-transformacion"></a>
## 13. Lotes de transformación

### Qué hace el usuario aquí

Opera transformación primaria o secundaria según su rol.

### Qué verá normalmente

- Filtros por búsqueda, producto y proyecto.
- Sección de lotes primarios, secundarios o ambas.
- Acciones de crear lote, ver detalle, ver ubicación y QR según permisos.

### Transformación primaria

- Se crea desde lotes de acopio disponibles.
- El flujo incluye recepción, acondicionado, ablandamiento opcional, pulpeado, envasado y almacenamiento.
- No se puede avanzar si el documento de la etapa actual no fue generado.
- Si un lote primario ya fue usado para un lote secundario, la edición queda bloqueada.

### Transformación secundaria

- Se crea desde lotes primarios disponibles.
- El flujo trabaja aportes de lotes fuente, recepción secundaria y transporte.
- Puede incluir generación de QR de trazabilidad y QR para cliente según permisos.

### Caso especial del rol de almacenamiento

- Un usuario de almacenamiento temporal solo ve lotes primarios en estado `almacenamiento`.

### Qué hacer si falla

- Si no aparece una sección, revisar permisos del tipo de transformación.
- Si no deja avanzar etapa, revisar si ya se generó el documento correspondiente.

---

<a id="formularios-dinamicos"></a>
## 14. Formularios dinámicos

### Qué hace el usuario aquí

Crea, mantiene, publica y versiona formularios dinámicos.

### Qué verá normalmente

- Tabs por estado: `Todos`, `Publicados`, `Borradores`, `Archivados`.
- Filtros por producto, etapa, ámbito y proyecto.
- Acciones de crear, editar, copiar, ver historial y publicar según permisos.

### Paso a paso

1. Entrar a `Formularios Dinámicos`.
2. Filtrar el universo que quiere revisar.
3. Crear un formulario nuevo o abrir uno existente.
4. Completar metadatos: producto, ámbito, proyecto si aplica y etapas.
5. Pasar al builder.
6. Definir campos ligados a protocolo y campos libres.
7. Guardar borrador o publicar con vigencia.

### Qué debe saber el usuario

- El builder trabaja en dos pasos: metadatos y construcción del formulario.
- Los formularios tienen versión, estado y vigencia.
- El ámbito puede ser de empresa o de proyecto.

### Qué hacer si falla

- Si no aparece un proyecto para el ámbito `project`, revisar que exista proyecto disponible para la empresa.
- Si no deja avanzar al builder, completar título, producto y etapas.

---

<a id="errores-frecuentes-y-recomendaciones"></a>
## 15. Errores frecuentes y recomendaciones

### Problemas frecuentes

| Escenario | Qué suele significar |
|---|---|
| No aparece un módulo | Falta permiso o el backend no lo devolvió en el menú |
| El botón está deshabilitado | Falta un requisito previo o la etapa del proyecto no lo permite |
| No deja entrar después del login | Correo no verificado, permisos vacíos o error al cargar menú |
| Falla una carga documental | Formato o tamaño inválido, o error del backend |
| Falla geolocalización | El usuario debe ubicar el punto manualmente |
| El mapa no termina de importar | El archivo falló o el procesamiento excedió el tiempo esperado |

### Recomendaciones prácticas

- Usar preferentemente Chrome o un navegador basado en Chromium.
- No capacitar desde módulos que el usuario no ve en su menú real.
- Antes de reportar una falla, revisar permiso, etapa y datos obligatorios.
- En documentos, registrar claramente por qué se aprueba, observa o rechaza.
- En proyectos, revisar el bloqueo del botón de avance antes de escalar el caso.

Siguiente paso recomendado: abrir el manual del rol correspondiente desde [el documento principal](guia-definitiva-negocio.md#manuales-por-rol)
