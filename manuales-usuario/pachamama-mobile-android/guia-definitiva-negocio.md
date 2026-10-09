# Manual de Usuario - Pachamama Mobile

**Dirigido a:** Equipo de negocio, operación, supervisión y validación funcional  
**Objetivo:** Explicar cómo usar la app de forma clara y práctica  
**Incluye:** Cambios recientes de actividades en borrador y multimedia persistente

---

## Índice

1. [Propósito de esta guía](#proposito)
2. [Qué puede hacer el usuario en la app](#que-hace-la-app)
3. [Qué cambió en esta versión](#cambios-recientes)
4. [Flujo general de uso](#flujo-general)
5. [Onboarding de nuevo recolector](#onboarding)
6. [Envío y uso de OTP](#otp)
7. [Inicio de sesión con DNI y últimos 3 dígitos del teléfono](#inicio-de-sesion)
8. [Pantalla Inicio y visualización del mapa](#inicio-y-mapa)
9. [Registro de actividades](#registro-de-actividades)
10. [Estados de las actividades](#estados-de-las-actividades)
11. [Actividades en borrador](#actividades-en-borrador)
12. [Sincronización de actividades](#sincronizacion-de-actividades)
13. [Escenarios de error en registro y sincronización](#errores-de-registro-y-sincronizacion)
14. [Actividades sincronizadas](#actividades-sincronizadas)
15. [Perfil del usuario](#perfil-del-usuario)
16. [Actualización de foto de perfil](#actualizacion-de-foto-de-perfil)
17. [Actualización de fotos de DNI](#actualizacion-de-fotos-de-dni)
18. [Actualización de método de pago](#actualizacion-de-metodo-de-pago)
19. [Cerrar sesión](#cerrar-sesion)
20. [Cómo guarda la app información en el teléfono](#almacenamiento-local)
21. [Cuánto tiempo puede quedar información en el teléfono](#retencion-de-datos)
22. [Cómo proteger el teléfono y la información](#seguridad-en-el-telefono)
23. [Recomendaciones operativas para negocio](#recomendaciones-operativas)
24. [Resumen final](#resumen-final)

---

<a id="proposito"></a>
## 1. Propósito de esta guía

Este manual explica, paso a paso, cómo usa un recolector la aplicación Pachamama Mobile en su trabajo diario.

Su objetivo es ayudar a que el equipo de negocio pueda:

- Entender qué ve el usuario en cada pantalla.
- Saber qué debe hacer el usuario en cada flujo.
- Identificar qué pasa cuando hay conexión, cuando no la hay, o cuando aparece un error.
- Incorporar correctamente el nuevo uso de borradores y continuidad de actividades.

---

<a id="que-hace-la-app"></a>
## 2. Qué puede hacer el usuario en la app

Con Pachamama Mobile, el recolector puede:

- Registrarse por primera vez y validar su identidad.
- Iniciar sesión de forma segura.
- Consultar su proyecto, comunidad y mapa de trabajo.
- Registrar actividades en campo con evidencia.
- Guardar actividades como borrador para continuarlas después.
- Trabajar sin conexión y sincronizar cuando vuelva la señal.
- Revisar su perfil y actualizar datos clave.

---

<a id="cambios-recientes"></a>
## 3. Qué cambió en esta versión

Los cambios más importantes de la versión actual están relacionados con el registro de actividades en borrador.

- La evidencia multimedia ahora se guarda en almacenamiento persistente del teléfono desde el momento en que se captura o adjunta.
- Una misma actividad conserva el mismo identificador desde que nace como borrador hasta que se envía.
- El usuario puede guardar borrador manualmente y retomar más tarde sin perder respuestas ni multimedia.
- La app guarda el borrador automáticamente si detecta cambios reales y pasa el tiempo configurado.
- Si la app pasa a segundo plano, el borrador se intenta guardar de inmediato.
- Si el usuario intenta salir con cambios sin guardar, la app pregunta si desea guardar el borrador.
- Al reabrir un borrador, se recuperan respuestas, selecciones y evidencia asociada.
- Si se elimina un borrador, también se elimina su multimedia asociada.

En la práctica, esto significa:

- Menor pérdida de trabajo en campo.
- Menor reproceso por cierres inesperados.
- Mejor continuidad cuando la actividad no puede terminarse en una sola sesión.

---

<a id="flujo-general"></a>
## 4. Flujo general de uso

De forma simple, este es el recorrido normal dentro de la app:

1. El usuario abre la app.
2. Si no tiene sesión, se registra o inicia sesión.
3. Ingresa al menú principal.
4. Revisa su información en `Inicio`.
5. Registra actividades en `Actividades`.
6. Guarda borradores o envía actividades.
7. La app sincroniza cuando hay conexión.
8. El usuario consulta o actualiza su información en `Recolector`.

---

<a id="onboarding"></a>
## 5. Onboarding de nuevo recolector

El onboarding es el registro inicial del recolector cuando usa la app por primera vez.

### Qué hace el usuario aquí

Completa su registro inicial para poder usar la app y quedar listo para operar en su proyecto.

### Paso a paso

| Paso | Qué hace el usuario | Resultado esperado |
|---|---|---|
| 1. Código o QR | Escanea un QR o ingresa manualmente un código de invitación | La app valida el acceso al proyecto y la comunidad |
| 2. Datos personales | Ingresa DNI y valida o completa sus datos | La app registra la identidad base del recolector |
| 3. Teléfono | Ingresa su celular y valida el OTP | El teléfono queda confirmado |
| 4. Método de pago | Selecciona cómo recibirá pagos | Queda configurado el medio de pago |
| 5. Fotos de DNI | Toma foto del frente y reverso del DNI | Se adjunta evidencia documental |
| 6. Foto de perfil | Se toma una selfie | Queda registrada la foto de perfil |
| 7. Consentimiento | Lee, acepta y firma el consentimiento | Se completa el registro |

### Qué verá normalmente

- Pantallas consecutivas de registro.
- Mensajes para completar datos y validar el teléfono.
- Un paso final de consentimiento y firma.
- Una entrada automática al flujo principal si el registro termina correctamente.

### Puntos operativos importantes

- El paso de fotos de DNI hoy puede omitirse en la app, aunque operativamente sigue siendo recomendable capturarlo.
- La foto de perfil sí debe capturarse para continuar.
- El consentimiento requiere aceptación y firma.
- Si el registro finaliza bien, el usuario entra al flujo principal con su sesión ya creada.

### Qué hacer si falla

- Si el código o QR no es válido, debe volver a escanearse o pedirse uno correcto.
- Si el DNI no avanza, debe revisarse que esté completo y bien escrito.
- Si el teléfono no se valida por OTP, no podrá completarse el registro.
- Si el método de pago está incompleto, debe completarse antes de continuar.
- Si falta selfie o firma, la app no dejará finalizar.
- Si el flujo se interrumpe, puede ser necesario repetir parte del registro.

### Consejo práctico

- El registro se hace una sola vez por recolector, salvo que se cambie de equipo o deba repetirse por alguna razón operativa.
- Es importante que el usuario tenga a la mano su DNI, su celular y su método de pago antes de empezar.
- Si el usuario interrumpe el registro inicial, puede necesitar volver a comenzar algunas partes del flujo.

---

<a id="otp"></a>
## 6. Envío y uso de OTP

La app usa códigos OTP para validar la identidad del usuario y algunos datos sensibles.

### Cuándo aparece

| Escenario | Para qué sirve | Qué debe hacer el usuario |
|---|---|---|
| Onboarding - teléfono principal | Confirmar el celular del recolector | Ingresar el código recibido por SMS |
| Onboarding - billetera móvil | Validar un número distinto al celular principal | Ingresar el código recibido por SMS |
| Inicio de sesión | Confirmar identidad antes de entrar | Ingresar el código recibido por SMS |
| Actualización de billetera móvil | Confirmar un nuevo número desde perfil | Ingresar el código recibido por SMS |

### Paso a paso

1. La app envía un código al celular.
2. El usuario revisa el SMS recibido.
3. Ingresa los 4 dígitos en la pantalla.
4. La app valida el código.
5. Si es correcto, el flujo continúa.

### Qué verá normalmente

- Un mensaje indicando que se envió un código al celular.
- Un espacio para ingresar los 4 dígitos.
- Un contador visible mientras el código sigue vigente.
- Una opción para reenviar el código si ya venció o si no llegó.

### Reglas visibles para el usuario

- El código OTP es de 4 dígitos.
- Durante onboarding e inicio de sesión, el tiempo visible de vigencia es de aproximadamente 5 minutos.
- En la actualización de billetera móvil desde perfil, el tiempo visible es más corto.
- Si el código falla varias veces, la app exige solicitar uno nuevo.
- En onboarding, la app limita los intentos de verificación y también los reenvíos.
- Si el código expira, el usuario debe reenviarlo.

### Qué hacer si falla

- Validar que el número ingresado sea correcto antes de pedir el OTP.
- Si el OTP no llega, revisar señal y esperar unos segundos antes de reenviar.
- Si el código expiró, debe solicitarse uno nuevo.
- Si el código falla varias veces, la app pedirá uno nuevo.
- Si el usuario cambia de número durante el flujo, debe volver a validarlo.

---

<a id="inicio-de-sesion"></a>
## 7. Inicio de sesión con DNI y últimos 3 dígitos del teléfono

Este flujo se usa cuando el recolector ya fue registrado anteriormente.

### Qué hace el usuario aquí

Ingresa a su cuenta usando su DNI, una validación corta del teléfono y un OTP.

### Paso a paso

1. Ingresa su DNI de 8 dígitos.
2. Ingresa los últimos 3 dígitos del teléfono registrado.
3. Presiona `Iniciar sesión`.
4. Recibe un OTP.
5. Ingresa el OTP y entra a la app.

### Qué valida la app

- Que el DNI tenga el formato correcto.
- Que los 3 dígitos coincidan con el teléfono registrado.
- Que el OTP sea correcto.

### Qué verá normalmente

- La pantalla de ingreso con DNI y 3 dígitos.
- Luego, la pantalla para ingresar el OTP.
- Finalmente, el menú principal si todo salió bien.

### Qué hace la app después de ingresar

- La app actualiza la información principal del recolector en el teléfono.
- Esto incluye datos como proyecto, comunidad, etapa del proyecto y estado del recolector.
- Gracias a esto, el usuario puede seguir viendo información actualizada aunque luego trabaje sin conexión.

### Qué pasa si algo falla

- Si los datos iniciales no coinciden, no avanza al OTP.
- Si el OTP es incorrecto, la app permite nuevos intentos hasta exigir un nuevo código.
- Si el OTP expira, debe reenviarse.

### Consejo práctico

- Si el usuario cambia de teléfono o vuelve a instalar la app, este suele ser el flujo normal para entrar nuevamente.

---

<a id="inicio-y-mapa"></a>
## 8. Pantalla Inicio y visualización del mapa

La pestaña `Inicio` es la pantalla principal de trabajo del recolector.

### Qué encuentra el usuario aquí

| Bloque | Qué ve el usuario |
|---|---|
| Estado de sincronización | Si hay datos sincronizando, errores o actividades pendientes |
| Resumen operativo | Proyecto, etapa, comunidad, brigada y solicitud si aplica |
| Mapa del proyecto | Vista previa del área del proyecto |
| Estado de ubicación | Si está dentro o fuera del área del proyecto |
| Calidad GPS | Detalles de señal y precisión cuando el usuario decide verla |

### Paso a paso para usar esta pantalla

1. Revisar el estado de sincronización.
2. Confirmar proyecto, comunidad, brigada y solicitud si aplica.
3. Revisar el mapa del proyecto.
4. Confirmar si la ubicación está dentro o fuera del área.
5. Si necesita refrescar información, usar el botón de sincronización de la cabecera.

### Qué verá normalmente

- El mapa puede verse en una tarjeta dentro de `Inicio`.
- El usuario puede presionar `Expandir` para verlo a pantalla completa.
- Si ya existe información descargada, la app puede seguir mostrando el mapa aunque no haya conexión.
- Si no hay permisos o no hay datos disponibles, la experiencia puede mostrar error o pedir reintento.

### Sincronización desde la cabecera de `Inicio`

La pestaña `Inicio` tiene un botón de sincronización en la cabecera.

- Este botón permite refrescar manualmente la información principal del recolector y su asignación.
- Al usarlo, la app intenta actualizar información como proyecto asignado, comunidad, etapa o estado del proyecto, estado del recolector, y brigada y solicitud actual si aplica.
- También dispara la actualización de recursos que ayudan al trabajo offline, como formularios y mapa del proyecto.

Para el usuario, esto sirve para:

- Actualizar su información sin tener que cerrar sesión.
- Descargar cambios recientes del proyecto y del recolector.
- Mantener el teléfono listo para seguir trabajando offline con datos más actuales.

### Ubicación y GPS

- La app intenta obtener la ubicación actual del usuario.
- Si el GPS está apagado, la app lo informa.
- Si faltan permisos, la app los solicita.
- Si la ubicación no puede validarse, la creación de nuevas actividades puede quedar bloqueada.

### Qué hacer si falla

- Si el mapa no carga, usar la sincronización de la cabecera y volver a intentar.
- Si la app indica falta de permisos, autorizarlos en el teléfono.
- Si el GPS está apagado, encenderlo antes de registrar actividades.
- Si la ubicación no puede validarse, el registro de nuevas actividades puede quedar bloqueado temporalmente.

### Consejo práctico

- Antes de empezar el trabajo de campo, conviene entrar a `Inicio` y usar la sincronización manual para refrescar la información del teléfono.

---

<a id="registro-de-actividades"></a>
## 9. Registro de actividades

La pestaña `Actividades` es el lugar donde el usuario registra, guarda y revisa su trabajo de campo.

### Qué encuentra el usuario aquí

| Sección | Para qué sirve |
|---|---|
| `Pendientes` | Ver borradores y actividades aún no enviadas |
| `Historial` | Ver actividades ya sincronizadas desde el servidor |

### Antes de empezar

| Condición | Comportamiento |
|---|---|
| Recolector activo y ubicación válida | Puede crear nueva actividad |
| Recolector inactivo | No puede crear nuevas actividades |
| Ubicación fuera del área | No puede iniciar nuevas actividades desde la lista principal |
| Validación de ubicación en curso | La app espera antes de habilitar el flujo |
| Error de ubicación | La app muestra advertencia y permite reintentar |

### Qué debe entender el usuario antes de registrar

- No siempre podrá registrar una actividad apenas entra a esta sección.
- La app primero revisa si su estado como recolector le permite trabajar.
- También revisa si la ubicación es válida para el registro.
- Además, el proyecto debe estar en una etapa que sí permita registrar actividades.

### Paso a paso

1. El usuario entra a `Actividades`.
2. Presiona `+` para agregar una actividad nueva.
3. Elige el tipo de actividad permitido para su proyecto.
4. Completa la información de la unidad forestal.
5. Completa el formulario dinámico.
6. Agrega evidencia si el formulario la solicita.
7. Decide si guarda borrador o registra la actividad.

### Tipos de actividad que puede ver el usuario

La app contempla dos opciones principales de registro:

| Tipo | Uso |
|---|---|
| `Inventario` | Registrar unidades forestales en etapa de inventario |
| `Recolección` | Registrar unidades o eventos de recolección |

### Regla clave de habilitación

- Estas opciones no están siempre disponibles.
- La app solo habilita `Inventario` o `Recolección` cuando el proyecto tiene habilitado ese tipo de trabajo en su configuración y etapa operativa actual.
- Si el proyecto está en una etapa previa, distinta o posterior, el registro de actividades puede no habilitarse.
- En ese caso, aunque el usuario entre a `Actividades`, no verá habilitada la opción de registrar ese tipo de actividad.

En términos simples:

- Si el proyecto está en etapa de `Inventario`, se habilita `Inventario`.
- Si el proyecto está en etapa de `Recolección`, se habilita `Recolección`.
- Si el proyecto todavía no llegó a esas etapas o ya pasó a otra fase sin registro operativo móvil, el alta de actividades no estará disponible.

### Qué verá normalmente

- La lista de `Pendientes` o `Historial`.
- Un botón `+` cuando el registro está habilitado.
- Las opciones `Inventario` o `Recolección` solo cuando el proyecto lo permite.
- Si el tipo de actividad no está disponible, la opción aparecerá deshabilitada o no habilitada para ese proyecto.
- Esto no significa necesariamente un error de la app.
- En muchos casos solo significa que el proyecto aún no está en la etapa correcta para registrar actividades desde el móvil.

### Qué puede contener el formulario

- Texto.
- Números.
- Fecha y hora.
- Preguntas de selección.
- Ubicación.
- Fotos.
- Videos.
- Selfies.
- Firma digital.

### Validación antes del guardado final

- La app revisa que estén completos los campos obligatorios.
- La app exige una ubicación válida para registrar la actividad.
- Si al momento de registrar detecta que la ubicación está fuera del área, muestra una advertencia y permite `Continuar` o `Cancelar`.

### Qué hacer si falla

- Si no aparece el botón `+`, revisar estado del recolector, ubicación y etapa del proyecto.
- Si no se habilita `Inventario` o `Recolección`, revisar si el proyecto está en la etapa correcta.
- Si no deja registrar, completar los campos obligatorios y revisar GPS.
- Si falla la captura de evidencia, volver a tomar la foto o video y revisar permisos de cámara.

---

<a id="estados-de-las-actividades"></a>
## 10. Estados de las actividades

Cada actividad puede pasar por distintos estados mientras el usuario la registra y la envía.

| Estado visible | Significado para negocio |
|---|---|
| `Borrador` | La actividad fue guardada parcialmente y aún puede seguir editándose |
| `Pendiente...` | La actividad ya quedó lista para enviarse, pero todavía no se ha sincronizado |
| `Enviando...` | La app está intentando enviar la actividad |
| `No se pudo enviar` | La actividad llegó a un estado de error visible y requiere atención |
| `Enviado` | La actividad ya fue aceptada por el flujo de sincronización |

### Aclaración importante

La app intenta reintentar varios errores de sincronización antes de mostrar el estado visible `No se pudo enviar`. Por eso, una actividad puede permanecer un tiempo en `Pendiente...` antes de que el error se haga explícito.

### Cómo interpretar estos estados

- `Borrador` significa que la actividad todavía está en construcción.
- `Pendiente...` significa que ya está lista y espera envío.
- `Enviando...` significa que la app ya está intentando sincronizar.
- `No se pudo enviar` significa que la actividad necesita revisión o reintento.
- `Enviado` significa que el flujo local terminó correctamente.

### Qué puede hacer el usuario según el estado

- `Borrador`: seguir editando o eliminarlo si ya no se necesita.
- `Pendiente...`: esperar conexión o usar `Sincronizar Todo`.
- `Enviando...`: esperar a que termine el intento actual.
- `No se pudo enviar`: revisar el caso antes de reintentar o reportarlo.
- `Enviado`: buscar la actividad en `Historial`.

---

<a id="actividades-en-borrador"></a>
## 11. Actividades en borrador

Esta es una de las funciones más importantes de la versión actual.

### Qué hace el usuario aquí

Usa el borrador cuando todavía no termina una actividad pero no quiere perder el avance.

### Paso a paso

1. Comienza una actividad.
2. Llena parte del formulario.
3. Presiona `Guardar borrador` o deja que la app lo guarde automáticamente.
4. Más tarde, entra a `Pendientes`.
5. Reabre el borrador y continúa.
6. Cuando termina, registra la actividad.

### Qué puede hacer el usuario con un borrador

- Guardarlo manualmente con el botón `Guardar borrador`.
- Retomarlo después desde la sección `Pendientes`.
- Eliminarlo de forma controlada.
- Continuar desde donde se quedó, incluyendo multimedia.

### Qué hace ahora la app

| Comportamiento | Resultado para el usuario |
|---|---|
| Guardado manual | Puede pausar una actividad sin terminarla |
| Autoguardado cada 5 minutos si hubo cambios reales | Reduce pérdida de avance |
| Guardado al pasar a segundo plano | Protege el avance si la app se minimiza o se interrumpe |
| Reapertura de borrador | Recupera respuestas, selecciones y evidencia |
| Eliminación de borrador | Elimina también la multimedia asociada |

### Reglas operativas importantes

- `Guardar borrador` solo funciona si ya existe alguna información cargada.
- Si el usuario intenta salir con cambios sin guardar, la app pregunta si desea guardar el borrador.
- Si no hubo cambios nuevos, la app no muestra alertas innecesarias al salir.
- Un borrador se reabre en el mismo formulario, no como historial.

### Qué mejoró con el último cambio

- La misma actividad puede seguir trabajándose como un solo registro desde borrador hasta envío.
- La multimedia ya no depende solo de ubicaciones temporales.
- La evidencia se conserva aunque la app pase a segundo plano.
- La relación entre formulario, borrador y evidencia es más estable.
- El riesgo de perder fotos o videos por demoras de sincronización es menor.

### Cuándo conviene usar borrador

- Cuando el usuario todavía no termina de llenar el formulario.
- Cuando aún no tiene toda la evidencia necesaria.
- Cuando debe interrumpir el trabajo y retomarlo después.
- Cuando desea proteger el avance antes de moverse de lugar o perder señal.

### Qué hacer si falla

- Si `Guardar borrador` no funciona, revisar que ya exista información cargada en el formulario.
- Si el borrador no aparece, revisar la sección `Pendientes`.
- Si el usuario sale con cambios, conviene aceptar el guardado antes de abandonar la pantalla.

---

<a id="sincronizacion-de-actividades"></a>
## 12. Sincronización de actividades

La app fue pensada para que el usuario pueda trabajar incluso cuando la señal es limitada o inexistente.

### Qué hace el usuario aquí

Envía las actividades pendientes o espera a que la app las envíe cuando vuelva la señal.

### Paso a paso

1. El usuario registra o completa una actividad.
2. Si hay internet, la app intenta sincronizar en segundo plano y el usuario puede usar `Sincronizar Todo`.
3. Si no hay internet, la actividad queda guardada localmente para enviarse después.
4. Cuando vuelve la conexión, la app vuelve a intentar sincronizar.

### Sincronización al iniciar sesión o entrar a la app principal

- Cada vez que el usuario entra al flujo principal con sesión activa, la app intenta sincronizar su asignación y su contexto operativo.
- Esa actualización busca mantener vigente en el teléfono la información del recolector incluso para uso offline posterior.
- Gracias a eso, el equipo puede seguir viendo localmente datos recientes como proyecto, comunidad, etapa del proyecto y estado del recolector aunque después se pierda la señal.

### Qué se sincroniza en la práctica

- Actividades pendientes.
- Evidencia multimedia asociada a esas actividades.
- Información operativa como formularios y mapa cuando corresponde.

### Qué ve el usuario

- Indicadores de sincronización en `Inicio`.
- Botón `Sincronizar Todo` en `Pendientes` cuando hay conexión.
- Mensaje offline cuando no hay internet.
- Detalle del estado de sincronización desde perfil.

### Qué debe hacer el usuario

- Si tiene señal, puede usar `Sincronizar Todo` para acelerar el envío.
- Si no tiene señal, no necesita repetir el registro: la app conserva la actividad localmente.
- Cuando recupere internet, puede esperar el reintento automático o forzar la sincronización manualmente.

### Qué hacer si falla

- Si no hay internet, no volver a registrar la misma actividad.
- Si una actividad sigue pendiente, revisar `Pendientes` y usar `Sincronizar Todo` cuando haya señal.
- Si aparece `No se pudo enviar`, revisar el caso antes de reintentar o reportarlo.

---

<a id="errores-de-registro-y-sincronizacion"></a>
## 13. Escenarios de error en registro y sincronización

### Qué hacer si aparece un problema

1. Leer el mensaje que muestra la app.
2. Revisar conexión, GPS y permisos del teléfono.
3. Confirmar si la actividad quedó en `Borrador`, `Pendiente...` o `No se pudo enviar`.
4. Evitar registrar de nuevo la misma actividad antes de revisar su estado.

### Errores durante el registro de actividades

| Escenario | Qué hace la app |
|---|---|
| Faltan campos obligatorios | No permite registrar la actividad |
| Falta ubicación o permisos de ubicación | No permite registrar la actividad |
| GPS apagado o falla de ubicación | Informa el problema y pide reintentar |
| Ubicación fuera del área | Muestra advertencia y permite continuar o cancelar |
| Falla de cámara o captura | Muestra error y el usuario debe reintentar la evidencia |

### Errores durante la sincronización

| Escenario | Qué hace la app |
|---|---|
| Sin internet | Mantiene la actividad pendiente y espera nueva señal |
| Señal débil o cortes | Reintenta automáticamente |
| Error temporal del servidor | Reintenta automáticamente |
| Archivo multimedia faltante | Puede terminar en error visible de envío |
| Exceso de reintentos | La actividad pasa a `No se pudo enviar` |

### Qué debe saber negocio

- No todo error aparece inmediatamente como error final.
- La app primero intenta recuperar el envío sola.
- El historial depende de conexión con servidor, por lo que offline puede verse vacío.

### Qué debe hacer el usuario cuando aparece un problema

- Leer el mensaje que muestra la app antes de repetir acciones.
- Revisar primero conexión, GPS y permisos del teléfono.
- Si la actividad quedó pendiente, no volver a registrarla de inmediato.
- Si la actividad quedó en error visible, revisar si corresponde reintentar o reportar el caso.

---

<a id="actividades-sincronizadas"></a>
## 14. Actividades sincronizadas

### Qué pasa cuando una actividad ya fue enviada

- Deja de mostrarse como pendiente.
- Pasa a la consulta de `Historial`.
- Se revisa por fecha.
- Su detalle es de solo lectura.

### Qué debe saber sobre `Historial`

- El historial se consulta desde el servidor.
- Requiere internet para cargar.
- Si no hay conexión, el historial puede no mostrar resultados.

### Qué debe esperar el usuario

- No siempre verá la actividad enviada de inmediato en el historial si en ese momento no hay conexión suficiente.
- El historial sirve para consulta, no para edición.

---

<a id="perfil-del-usuario"></a>
## 15. Perfil del usuario

La pestaña `Recolector` reúne la información personal y operativa del usuario.

### Qué hace el usuario aquí

Consulta su información, revisa su asignación y actualiza datos personales importantes.

### Qué muestra

| Pestaña | Qué contiene |
|---|---|
| `Datos` | Documento, datos personales y teléfono |
| `Mis Pagos` | Método de pago actual y sus datos |
| `Mi Comunidad` | Proyecto, comunidad y brigadas |

### Estados del recolector

| Estado | Efecto operativo |
|---|---|
| `Activo` | Puede operar normalmente |
| `Inactivo` | No puede crear nuevas actividades |
| `Archivado` | La app obliga al cierre de sesión |

### Acciones disponibles desde perfil

- Ver estado de sincronización.
- Editar foto de perfil.
- Ver y actualizar fotos del DNI.
- Actualizar método de pago.
- Cerrar sesión.

### Paso a paso

1. Entrar a la pestaña `Recolector`.
2. Revisar `Datos`, `Mis Pagos` y `Mi Comunidad`.
3. Si necesita cambiar algo, usar la opción correspondiente.
4. Si quiere salir de la cuenta, usar `Cerrar sesión`.

### Para qué le sirve esta pantalla al usuario

- Confirmar que sigue asignado al proyecto correcto.
- Revisar si su método de pago está bien configurado.
- Ver si su cuenta está activa o tiene alguna restricción.
- Mantener sus datos actualizados.

---

<a id="actualizacion-de-foto-de-perfil"></a>
## 16. Actualización de foto de perfil

### Paso a paso

1. El usuario entra a `Editar foto de perfil`.
2. Se toma una nueva selfie.
3. Revisa la vista previa.
4. Presiona `Guardar`.

### Qué verá normalmente

- Una vista previa de la nueva foto.
- Un proceso de carga al guardar.
- Un mensaje de confirmación si el envío salió bien.

### Qué hace la app

- Procesa la imagen.
- La envía al servidor.
- Actualiza el perfil del usuario.

### Qué esperar operativamente

- Si no hay foto nueva, no se puede guardar.
- Si el envío sale bien, la app confirma la actualización.

### Recomendación para el usuario

- Tomar la foto con buena luz y con el rostro visible.
- Esperar la confirmación antes de salir de la pantalla.

### Qué hacer si falla

- Volver a tomar la foto si no quedó bien.
- Verificar conexión antes de guardar.
- Esperar el mensaje de confirmación antes de salir.

---

<a id="actualizacion-de-fotos-de-dni"></a>
## 17. Actualización de fotos de DNI

### Paso a paso

1. El usuario entra al detalle de su documento.
2. Ve el frente y el reverso si ya existen.
3. Puede volver a tomar uno o ambos lados.
4. La app actualiza la información.

### Qué verá normalmente

- Si no había fotos previas, igual puede capturarlas desde esta pantalla.
- La app muestra carga y confirmación mientras actualiza.
- Si falla la actualización, informa el error.

### Recomendación para el usuario

- Verificar que el texto del documento se vea con claridad.
- Repetir la foto si hay reflejos, desenfoque o cortes.

### Qué hacer si falla

- Repetir la captura si la imagen quedó borrosa.
- Revisar conexión antes de actualizar.
- Confirmar que se vea el frente y el reverso completos.

---

<a id="actualizacion-de-metodo-de-pago"></a>
## 18. Actualización de método de pago

### Métodos disponibles

| Método | Qué necesita |
|---|---|
| `Efectivo` | No requiere datos adicionales |
| `Giro DNI - Banco de la Nación` | No requiere una cuenta bancaria tradicional |
| `Transferencia bancaria` | Banco, número de cuenta y tipo de cuenta |
| `Billetera móvil` | Número de billetera validado por OTP |

### Paso a paso

1. Entrar a `Mis Pagos`.
2. Elegir el nuevo método de pago.
3. Completar los datos requeridos.
4. Si corresponde, validar el número con OTP.
5. Presionar `Guardar`.

### Reglas importantes

- En transferencia bancaria, la app pide completar todos los datos antes de guardar.
- En billetera móvil, la app exige validar el número con OTP antes de guardar.
- Si el OTP no se valida, el botón `Guardar` no queda habilitado.

### Qué hacer si falla

- Revisar si falta algún dato obligatorio.
- Si el método es billetera móvil, validar primero el OTP.
- Esperar la confirmación antes de salir de la pantalla.

### Recomendación para el usuario

- No salir de la pantalla hasta que vea que el cambio fue guardado.
- Confirmar que el número o cuenta ingresada sea la correcta antes de validar.

---

<a id="cerrar-sesion"></a>
## 19. Cerrar sesión

### Paso a paso

1. El usuario entra a `Recolector`.
2. Elige `Cerrar sesión`.
3. La app revisa si existen borradores o actividades pendientes.
4. Muestra una confirmación.
5. Si el usuario confirma, la sesión se cierra.

### Qué verá normalmente

- Si no hay pendientes, muestra una confirmación simple.
- Si existen borradores o actividades pendientes, muestra una advertencia más fuerte.
- Si el usuario confirma cerrar sesión con pendientes, la app elimina la información local operativa y vuelve al inicio.

### Qué hacer si falla o aparece una advertencia

- Si la app advierte que hay borradores o pendientes, conviene cancelar, revisar `Pendientes` y sincronizar antes de salir.
- Si el usuario no está seguro de haber enviado todo, debe revisar primero el estado de sus actividades.
- Si la cuenta fue archivada y la app fuerza el cierre de sesión, el caso debe revisarse con supervisión.

### Recomendación operativa

- Antes de cerrar sesión, se recomienda sincronizar todo lo pendiente.
- Si el teléfono va a cambiar de usuario, primero debe sincronizarse, luego cerrar sesión y finalmente validarse la limpieza del equipo.

### Qué debe entender el usuario

- Cerrar sesión no es lo mismo que simplemente salir de la app.
- Si existen pendientes o borradores, cerrar sesión puede implicar perder trabajo local no enviado.

---

<a id="almacenamiento-local"></a>
## 20. Cómo guarda la app información en el teléfono

La app guarda información local para poder funcionar aun cuando no haya conexión.

| Tipo de información | Cómo se conserva en el teléfono | Para qué sirve |
|---|---|---|
| Sesión y asignación actual | Datos locales de sesión de la app | Evitar pedir la información cada vez que se abre la app |
| Perfil del recolector | Caché local protegido | Cargar rápido los datos del perfil |
| Actividades y borradores | Base local de la app | Permitir trabajo offline y continuidad |
| Fotos, videos, selfies y firmas de actividades | Almacenamiento interno privado de la app | Proteger evidencia hasta que se sincronice |
| Formularios | Caché local | Permitir registro aunque la señal sea limitada |
| Mapa del proyecto | Caché local | Mostrar el área del proyecto incluso sin conexión reciente |

### Qué significa en el uso diario

- La app no depende totalmente de internet para operar.
- El teléfono actúa como respaldo temporal del trabajo del recolector.
- Esa retención local es intencional para proteger continuidad y evidencia.

### Qué debe entender el usuario

- Si no tiene señal, la app puede seguir funcionando en varias tareas.
- El teléfono conserva información para que el trabajo no se pierda.
- Por eso es importante no prestar el equipo ni cerrar sesión sin revisar pendientes.

---

<a id="retencion-de-datos"></a>
## 21. Cuánto tiempo puede quedar información en el teléfono

| Tipo de dato | Permanece en el teléfono hasta | Cómo se limpia normalmente |
|---|---|---|
| Datos temporales del onboarding | Completar el flujo o reiniciar el acceso | La app los limpia al reiniciar el flujo |
| Borradores | Que el usuario los elimine, los complete o cierre sesión | Eliminación manual o cierre de sesión |
| Actividades pendientes | Que se sincronicen o se cierre sesión | Sincronización o cierre de sesión |
| Formularios y mapa en caché | Nueva descarga o cierre de sesión | Limpieza de caché local |
| Perfil cacheado | Nueva sincronización o cierre de sesión | Limpieza de caché local |
| Multimedia operativa | Mientras esté asociada a borradores o pendientes | Se limpia al borrar borrador y en procesos de limpieza asociados |

### Consideración importante para operación

Como la app ahora protege la multimedia en almacenamiento persistente, el teléfono puede retener evidencia local durante más tiempo que antes. Eso es bueno para evitar pérdidas, pero obliga a tener disciplina operativa cuando un equipo cambia de usuario, sale de operación o requiere limpieza total.

Recomendación práctica:

- No asumir que un cambio de sesión equivale por sí solo a una limpieza completa del equipo.
- Para recambio de teléfono, aplicar cierre de sesión y limpieza controlada del dispositivo.

### En palabras simples

- La app guarda información en el teléfono para ayudar al usuario a no perder su trabajo.
- Esa misma ventaja exige cuidado cuando el teléfono cambia de manos.

---

<a id="seguridad-en-el-telefono"></a>
## 22. Cómo proteger el teléfono y la información

### Protecciones actuales que sí existen

| Protección | Qué significa en términos simples |
|---|---|
| Almacenamiento privado de la app | Otras apps no deberían acceder fácilmente a estos datos |
| Caché del perfil del recolector protegido | La información principal del perfil tiene una capa adicional de protección |
| OTP para accesos y cambios sensibles | Reduce el riesgo de uso indebido del número del usuario |
| Consentimiento y documentos sensibles con protección reforzada | La información más sensible viaja con controles adicionales |
| Permisos explícitos de cámara y ubicación | La app pide autorización antes de usar funciones sensibles |

### Consideraciones actuales que negocio debe conocer

| Consideración | Implicancia operativa |
|---|---|
| La app no tiene PIN propio ni biometría propia | La seguridad del teléfono sigue siendo fundamental |
| Parte de la operación offline queda guardada para continuidad | No se debe compartir el teléfono entre usuarios sin limpieza controlada |
| La protección del equipo depende también del bloqueo del sistema operativo | El teléfono debe usar contraseña, PIN o biometría del dispositivo |

### Recomendaciones de seguridad para campo

- Cada teléfono debe estar asignado a una sola persona mientras esté en operación.
- El teléfono debe tener bloqueo de pantalla activo.
- No se debe prestar el equipo con sesión iniciada.
- Antes de cambiar de usuario o devolver un equipo, se debe sincronizar, cerrar sesión y validar limpieza.
- Si el usuario reporta pérdida o robo del equipo, debe gestionarse el bloqueo del dispositivo cuanto antes.

### Mensaje clave para usuario y supervisión

- La seguridad de la app también depende del cuidado del teléfono.
- Un teléfono sin bloqueo o compartido pone en riesgo la información y la operación.

---

<a id="recomendaciones-operativas"></a>
## 23. Recomendaciones operativas para negocio

- Capacitar al usuario en `Guardar borrador` y no solo en `Registrar actividad`.
- Reforzar que la app puede trabajar sin conexión, pero que el envío final depende de recuperar señal.
- Pedir a supervisión que revise pendientes y errores visibles antes del cierre de jornada.
- Recomendar sincronización antes de cambio de turno, cambio de equipo o cierre de sesión.
- En problemas de OTP, validar número, señal y tiempo de vigencia antes de reiniciar el flujo.
- En problemas de GPS, revisar permisos y estado del GPS del teléfono antes de asumir una falla funcional de la app.

### Recomendación de capacitación

Si este manual se usa para entrenar usuarios, conviene explicar la app en este orden:

1. Inicio de sesión.
2. Pantalla `Inicio`.
3. Registro de actividades.
4. Borradores.
5. Sincronización.
6. Perfil y cierre de sesión.

---

<a id="resumen-final"></a>
## 24. Resumen final

Pachamama Mobile ya funciona como una herramienta de campo pensada para que el recolector pueda continuar su trabajo aun cuando la conectividad no sea estable.

Las tres ideas más importantes de este manual son:

1. La app puede guardar trabajo localmente para no perderlo.
2. El borrador ya es una parte formal del flujo de operación.
3. La seguridad y limpieza del teléfono siguen siendo responsabilidad crítica del proceso operativo.

En resumen:

- El usuario puede registrar, pausar, retomar y sincronizar su trabajo desde el teléfono.
- La app ayuda a proteger el avance y la evidencia del trabajo en campo.
- El equipo de negocio y supervisión debe acompañar ese uso con buenas prácticas de sincronización, revisión de pendientes y cuidado del dispositivo.
