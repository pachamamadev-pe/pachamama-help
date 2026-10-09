# Guía de Usuario — Pachamama Mobile

## Mapa de Flujos de la Aplicación

---

## 1. FLUJO DE INICIO (Splash)

**Propósito:** Determinar si el usuario ya tiene una sesión activa o es nuevo.

| Elemento | Detalle |
|---|---|
| **Pantalla** | Logo de Pachamama + indicador de carga |
| **Duración** | ~2 segundos |
| **Acción automática** | El sistema revisa si existe un usuario registrado previamente en el dispositivo |

**Condiciones:**
- **Si el usuario ya inició sesión antes** → Avanza directamente al **Menú Principal** (se salta todo el registro e inicio de sesión)
- **Si el usuario es nuevo** → Avanza a la pantalla de **Bienvenida**

**Mensajes que verás:**
- _"Inicializando..."_ → mientras se prepara la app
- _"Cargando tu perfil..."_ → si ya tienes sesión
- _"Preparando tu bienvenida..."_ → si eres nuevo

---

## 2. FLUJO DE BIENVENIDA Y REGISTRO (Onboarding)

### 2.1 Pantalla de Bienvenida

**Propósito:** Elegir entre registrarse por primera vez o iniciar sesión con cuenta existente.

**Opciones disponibles:**
| Botón | Acción |
|---|---|
| **"Registrarme por primera vez"** | Inicia el proceso de registro de 7 pasos |
| **"Ya tengo cuenta"** | Va al inicio de sesión (Login) |

---

### 2.2 FLUJO A: SOY NUEVO — Registro en 7 Pasos

> **Nota:** En cualquier paso puedes presionar "Atrás" para volver al paso anterior. Si sales completamente, tus datos temporales se borrarán.

#### Paso 1/7 — Escanear Código QR o Ingresar Código

**Propósito:** Ingresar el código de invitación del proyecto.

**¿Qué puedes hacer?**
- **Opción A:** Escanear un código QR con la cámara del celular
- **Opción B:** Ingresar manualmente un código de invitación de 6 caracteres

**¿Qué sucede después?**
- El sistema valida el código
- Si es válido, se guarda la información del proyecto y comunidad a la que pertenecerás
- Automáticamente avanza al **Paso 2**

**Condiciones:**
- Si el código es inválido, se muestra un mensaje de error y puedes intentar de nuevo

---

#### Paso 2/7 — Datos Personales

**Propósito:** Registrar tu identificación con el DNI.

**¿Qué debes hacer?**
1. Ingresar tu **número de DNI** (8 dígitos)
2. El sistema consulta una base de datos externa para obtener tu información
3. Revisa que los datos sean correctos: **Nombres, Apellidos, Fecha de Nacimiento, Género**
4. Presiona "Continuar"

**Condiciones:**
- Si el DNI no se encuentra, puedes escribir tus datos manualmente
- Si los datos consultados no coinciden, puedes corregirlos
- El sistema muestra un indicador de carga mientras consulta

---

#### Paso 3/7 — Información de Contacto

**Propósito:** Registrar tu número de celular y verificarlo.

**¿Qué debes hacer?**
1. Ingresar tu **número de teléfono celular**
2. Recibirás un código de verificación por **SMS (OTP)**
3. Ingresa el código de 4 dígitos que llegó a tu celular
4. Presiona "Continuar"

**Condiciones:**
- El código tiene un **tiempo de vencimiento** (cuenta regresiva)
- Si el código expira, puedes solicitar uno nuevo
- Si el código es incorrecto, puedes intentar de nuevo (máximo 3 intentos)

---

#### Paso 4/7 — Información de Pago

**Propósito:** Registrar cómo deseas recibir tus pagos como recolector.

**Opciones de pago disponibles:**

| Método | ¿Qué debes ingresar? |
|---|---|
| **Efectivo** | No requiere datos adicionales |
| **Transferencia Bancaria** | Nombre del banco, número de cuenta, tipo de cuenta (Ahorros/Corriente) |
| **Billetera Móvil** | Número de celular de la billetera (requiere verificación OTP) |

**Condiciones:**
- Si eliges **Transferencia Bancaria**, aparecen campos adicionales para los datos bancarios
- Si eliges **Billetera Móvil**, se te envía un código de verificación al número de billetera que ingresaste
- Presiona "Continuar" cuando esté listo

---

#### Paso 5/7 — Captura de DNI (Fotos)

**Propósito:** Tomar fotos de tu documento de identidad (opcional pero recomendado).

**¿Qué debes hacer?**
1. Tomar una foto del **anverso (frente)** de tu DNI
2. Tomar una foto del **reverso (dorso)** de tu DNI
3. Puedes usar la cámara frontal o trasera

**Condiciones:**
- **Paso opcional:** Puedes omitir este paso si no deseas tomar las fotos
- Si ya capturaste las fotos, puedes repetirlas si no quedaron bien
- Las imágenes se guardan temporalmente en el dispositivo

---

#### Paso 6/7 — Foto de Perfil

**Propósito:** Tomarte una selfie para tu foto de perfil (opcional).

**¿Qué debes hacer?**
- Tomar una **selfie** con la cámara frontal
- La foto se usará como tu imagen de perfil en la aplicación

**Condiciones:**
- **Paso opcional:** Puedes omitir este paso si lo prefieres
- Puedes repetir la foto si no te gustó el resultado

---

#### Paso 7/7 — Consentimiento Informado

**Propósito:** Leer, aceptar y firmar el consentimiento informado para participar como recolector.

**¿Qué debes hacer?**
1. Leer el documento de consentimiento (puedes desplazarte para ver todo el contenido)
2. Marcar la casilla de **aceptación**
3. **Dibujar tu firma** en el recuadro usando tu dedo
4. Presiona "Finalizar" para completar el registro

**Condiciones:**
- **Debes** aceptar el consentimiento y firmar para poder continuar
- Si decides cancelar, se cancela todo el registro y vuelves al inicio
- Al confirmar, el sistema envía toda tu información al servidor

---

#### ¡Registro Exitoso!

**Propósito:** Confirmar que tu registro se completó y mostrarte tu asignación.

**¿Qué verás?**
- Un mensaje de felicitaciones con tu nombre
- El nombre del **proyecto** y la **comunidad** a la que fuiste asignado
- El sistema verifica el estado de tu registro (pendiente, en proceso, completado)
- Presiona "Continuar" para ingresar al **Menú Principal**

**Condiciones:**
- Si hay errores en el servidor, se mostrará un mensaje y podrás intentar más tarde
- Una vez exitoso, tu sesión queda guardada y no tendrás que volver a registrarte

---

### 2.3 FLUJO B: YA TENGO CUENTA — Opciones para Recolector Existente

#### Pantalla de Opciones

**Propósito:** Elegir entre iniciar sesión o unirse a un nuevo proyecto.

| Opción | Descripción |
|---|---|
| **Iniciar Sesión** | Acceder a tu cuenta actual con tus credenciales |
| **Unirme a Nuevo Proyecto** | Si ya tienes cuenta y te invitaron a un nuevo proyecto |

---

### 2.4 Inicio de Sesión (Login)

**Propósito:** Acceder a tu cuenta existente.

**¿Qué debes hacer?**
1. Ingresar tu **número de DNI** (8 dígitos)
2. Ingresar los **últimos 3 dígitos de tu celular** registrado
3. Presiona "Iniciar Sesión"

**Condiciones:**
- El botón se habilita solo cuando ambos campos están completos
- Si las credenciales son incorrectas, verás un mensaje de error
- Si son correctas, se te enviará un código de verificación

#### Verificación OTP (Código de 4 dígitos)

**Propósito:** Verificar tu identidad con un código enviado a tu celular.

**¿Qué debes hacer?**
1. Ingresa el código de **4 dígitos** que recibiste por SMS
2. El código tiene un tiempo límite (cuenta regresiva visible)
3. Presiona "Validar código"

**Condiciones:**
- El botón se habilita cuando ingresas los 4 dígitos
- **Máximo 3 intentos** de verificación
- Si el código expira, presiona **"Reenviar código"** para recibir uno nuevo
- Si la verificación es exitosa, accedes automáticamente al **Menú Principal**
- Si fallas los 3 intentos, deberás volver a la pantalla de inicio de sesión

---

### 2.5 Unirse a Nuevo Proyecto (para Recolectores Existentes)

**Propósito:** Cuando ya tienes cuenta pero te asignaron a un proyecto nuevo.

**¿Qué debes hacer?**
1. Escanear el **código QR** del nuevo proyecto
2. O ingresar manualmente el **código de invitación**
3. El sistema valida el código y te asigna al nuevo proyecto

**¿Qué verás después?**
- Pantalla de éxito con el nombre del proyecto y comunidad al que te uniste
- Presiona "Continuar" para ir al **Menú Principal**

---

## 3. MENÚ PRINCIPAL

**Propósito:** Navegación principal de la aplicación con 3 pestañas.

| Pestaña | Icono | Nombre |
|---|---|---|
| 1 | Inicio | **Inicio** |
| 2 | Actividades | **Actividades** |
| 3 | Recolector | **Recolector** |

**Barra Superior (Top Bar):**
- Logo de Pachamama
- **Icono de notificaciones** — Muestra un punto rojo si hay notificaciones sin leer
- **Icono de sincronización** — Solo visible en la pestaña Inicio. Presiona para sincronizar datos manualmente
- **Menú de opciones** — Solo visible en la pestaña Recolector

**Barra Inferior (Bottom Navigation):**
- Las 3 pestañas para cambiar entre secciones

---

### 3.1 PESTAÑA INICIO (Home / Dashboard)

**Propósito:** Mostrar un resumen de tu información operativa y el área del proyecto.

#### ¿Qué información verás?

**Estado de sincronización:**
- Si hay datos sincronizándose: muestra _"Sincronizando..."_
- Si hay errores: muestra mensaje de error
- Si hay actividades pendientes: muestra el conteo

**Saludo personalizado:**
- _"¡Hola, [Tu Nombre]!"_
- _"Gracias por tu colaboración"_

**Resumen Operativo (tarjetas informativas):**

| Tarjeta | Descripción |
|---|---|
| **Proyecto** | Nombre del proyecto al que perteneces |
| **Estado** | Etapa del proyecto (Ej: "Inventario", "Recolección") |
| **Comunidad** | Nombre de la comunidad asignada |
| **Brigada** | Nombre de tu brigada (si aplica) |
| **Solicitud** | Código de solicitud de recolección (si aplica) |

**Área del Proyecto (Mapa):**
- Mapa interactivo del área del proyecto
- Puedes presionar **"Expandir"** para ver el mapa en pantalla completa
- El mapa muestra los límites del proyecto y tu ubicación actual

**Indicador de ubicación:**
- Muestra si estás **dentro** o **fuera** del área del proyecto
- Si estás fuera, verás una advertencia

**Calidad de Señal GPS (opcional):**
- Puedes presionar **"Ver detalles"** para monitorear la calidad del GPS
- Muestra: calidad (Excelente/Buena/Regular/Mala), precisión, coordenadas y tiempo de monitoreo
- Botones: **"Iniciar toma"** / **"Detener"** para empezar o parar el monitoreo

**Condiciones especiales:**
- Si tu cuenta está **archivada**, aparecerá un diálogo forzoso que te obligará a cerrar sesión
- El botón de sincronización manual solo aparece en esta pestaña

---

### 3.2 PESTAÑA ACTIVIDADES (Tareas)

**Propósito:** Gestionar todas tus actividades de recolección de datos.

#### Vista Principal: Dos secciones

| Sección | Descripción |
|---|---|
| **Pendientes** | Actividades que aún no has enviado (borradores y pendientes) |
| **Historial** | Actividades ya enviadas al servidor (requiere conexión) |

---

#### Sección Pendientes

**¿Qué verás?**
- Lista de actividades con su estado:
  - **Borrador** — Guardaste la actividad pero no la has completado
  - **Pendiente...** — Completaste la actividad pero no se ha enviado
  - **Enviando...** — Se está subiendo al servidor
  - **No se pudo enviar** — Error al enviar (con intentos)
  - **Enviado** — Ya está en el servidor
- Cada actividad muestra: código de unidad forestal, fecha, hora, y tipo (Inventario/Recolección)
- Los **borradores** tienen un botón **"Eliminar"** para borrarlos

**¿Qué puedes hacer?**
- **Presionar una actividad** para ver sus detalles o continuar editándola (si es borrador)
- **Presionar el icono de estado** para ver información de sincronización
- **Sincronizar Todo** — Botón que envía todas las actividades pendientes (solo si hay conexión)

**¿Cómo agregar una nueva actividad?**
- Presiona el botón **"+"** (flotante) en la esquina inferior derecha
- Se abrirá un diálogo para elegir el tipo de actividad:
  - **Inventario** (si está habilitado para tu proyecto)
  - **Recolección** (si está habilitado para tu proyecto)
- Al seleccionar, se abre el **Formulario de Registro**

**Condiciones importantes:**
- Si el recolector está **Inactivo**, el botón "+" no aparece y verás una advertencia
- Si estás **fuera del área del proyecto**, el botón "+" no aparece
- Si no hay conexión a internet, verás una advertencia _"Sin conexión. Su información se enviará cuando recupere la señal."_

---

#### Sección Historial

**¿Qué verás?**
- Actividades que ya fueron enviadas al servidor
- Puedes **filtrar por fecha** usando los botones de fecha anterior y fecha siguiente
- La fecha se muestra en formato legible: _"lunes, 21 de mayo de 2026"_
- No puedes navegar a una fecha futura

**Condiciones:**
- **Requiere conexión a internet** para cargar los datos del historial
- Sin conexión: muestra _"No hay datos para mostrar. Se consultarán automáticamente cuando mejore la conexión."_
- Si hay error: muestra mensaje y botón **"Reintentar"**
- Si no hay actividades: muestra mensaje _"No hay actividades registradas"_

---

### 3.3 FORMULARIO DE REGISTRO DE ACTIVIDAD

**Propósito:** Capturar información de una unidad forestal (árbol o troza).

**Esta pantalla tiene 3 partes:**

#### Parte 1: Información de la Unidad Forestal

**Comportamiento según la etapa del proyecto:**

**Si la etapa es INVENTARIO:**
- Ingresa el **código de la unidad forestal** manualmente
- La opción _"¿Es troza?"_ está deshabilitada (no aplica en inventario)

**Si la etapa es RECOLECCIÓN:**
- Automáticamente se marca como **"troza"**
- Debes ingresar:
  1. **Código de la unidad (Troza)** — Código manual de la troza que estás registrando
  2. **Unidad forestal padre** — Toca el campo para buscar y seleccionar el árbol padre del cual proviene la troza

**Para buscar una unidad padre:**
- Se abre una pantalla de selección con lista de unidades disponibles
- Puedes buscar por nombre o desplazarte por la lista
- Presiona la unidad deseada para seleccionarla

#### Parte 2: Formulario Dinámico

- El formulario se genera automáticamente según el tipo de actividad
- Puede incluir varios tipos de campos:
  - **Texto** — Para escribir información
  - **Número** — Para valores numéricos
  - **Fecha y Hora** — Para fechas y horas
  - **Sí/No** — Interruptor de opción
  - **Selección única** — Elegir una opción de varias
  - **Fotos / Videos** — Tomar fotos o grabar videos con la cámara
  - **Firma digital** — Dibujar tu firma
  - **Ubicación** — Capturar coordenadas GPS

#### Parte 3: Acciones del Formulario

| Botón | Acción |
|---|---|
| **"Guardar borrador"** | Guarda lo que has avanzado para continuar después |
| **"Registrar actividad"** | Envía la actividad (primero valida ubicación) |

**¿Qué pasa cuando presionas "Registrar actividad"?**
1. El sistema **valida tu ubicación** (geocerca)
2. Si estás **dentro del área** → La actividad se guarda y se agenda para sincronizar
3. Si estás **fuera del área** → Aparece un diálogo preguntando si deseas continuar de todas formas, mostrando la distancia al área
4. Presiona **"Continuar"** para guardar igual o **"Cancelar"** para no guardar

**Auto-guardado:**
- El formulario se guarda automáticamente cada cierto tiempo
- Si sales del formulario sin guardar, te preguntará si deseas guardar el borrador
- Si cierras la app, el borrador se guarda automáticamente

---

### 3.4 PESTAÑA RECOLECTOR (Perfil)

**Propósito:** Ver y editar tu información personal.

#### Cabecera del Perfil
- **Foto de perfil** (si tienes una)
- **Nombre completo**
- **Comunidad**
- **Estado:** Activo / Inactivo / Archivado

#### Tres pestañas de contenido:

##### Pestaña 1: "Datos"

| Sección | Información mostrada |
|---|---|
| **Información Personal** | Tipo de documento, Número de documento (con flecha para ver fotos del DNI), Fecha de nacimiento, Género, Edad |
| **Información de Contacto** | Teléfono |

- Presiona la **flecha** junto al número de documento para ver o actualizar las fotos de tu DNI

##### Pestaña 2: "Mis Pagos"

| Información | Detalle |
|---|---|
| **Método de Pago** | Muestra el método actual (Efectivo, Transferencia, Billetera Móvil) |
| **Detalles** | Si es transferencia: banco, número de cuenta (oculto parcialmente), tipo de cuenta |
| | Si es billetera móvil: número de la billetera |

- Presiona **"Editar"** para cambiar tu método de pago (seguirás los mismos pasos que en el registro)

##### Pestaña 3: "Mi Comunidad"

| Información | Detalle |
|---|---|
| **Tu Asignación** | Proyecto y Comunidad |
| **Asignaciones de Brigada** | Lista de brigadas a las que perteneces (actuales e históricas) |

- Cada brigada muestra: nombre, solicitud, tipo, período de asignación y estado (Activo/Archivado)
- La brigada **actual** tiene una estrella y está resaltada

#### Menú de opciones en la barra superior:

| Opción | Acción |
|---|---|
| **Estado de sincronización** | Ver detalles de los datos sincronizados |
| **Editar foto de perfil** | Tomar una nueva selfie |
| **Cerrar sesión** | Salir de la aplicación |

**Cerrar sesión:**
1. Presiona "Cerrar sesión"
2. Confirmas en el diálogo
3. **Si hay actividades pendientes:** se te advertirá que perderás los datos locales no sincronizados. Puedes elegir **"Borrar datos y salir"** o **"Cancelar"**

**Estado de sincronización:**
- Muestra el estado de los **Formularios** (versión, cantidad, hash)
- Muestra el estado del **Mapa del Proyecto** (hash, última actualización)
- Botón **"Sincronizar datos"** para forzar la sincronización

---

## 4. NOTIFICACIONES

**Propósito:** Ver mensajes y alertas del sistema.

**¿Cómo acceder?**
- Presiona el icono de notificaciones en la barra superior del Menú Principal
- El punto rojo indica que hay notificaciones sin leer

**¿Qué verás?**
- Lista de notificaciones con:
  - **Título** (en negrita si no está leída)
  - **Cuerpo** del mensaje
  - **Fecha y hora**
  - Punto indicador azul si no ha sido leída

**¿Qué puedes hacer?**
- Presionar una notificación para marcarla como leída
- Presionar "Atrás" para volver al Menú Principal

---

## 5. MAPA DEL PROYECTO (Pantalla Completa)

**Propósito:** Ver el área del proyecto en un mapa interactivo.

**¿Cómo acceder?**
- Desde la pestaña Inicio, presiona **"Expandir"** en la sección del mapa

**¿Qué verás?**
- Mapa con los límites del proyecto (polígonos)
- Tu ubicación actual
- Puedes hacer zoom, desplazarte, etc.

---

## 6. SINCRONIZACIÓN DE DATOS

**Propósito:** Mantener actualizados los datos entre tu dispositivo y el servidor.

**¿Cómo funciona?**
- **Automática:** La app sincroniza datos periódicamente cuando hay conexión
- **Manual:** Puedes presionar el icono de sincronización en la pestaña Inicio para sincronizar ahora

**¿Qué se sincroniza?**
| Tipo de dato | Descripción |
|---|---|
| **Formularios** | Plantillas de formularios actualizadas |
| **Mapa (GeoJSON)** | Límites y áreas del proyecto |
| **Actividades** | Tus registros de recolección (pendientes → enviados) |

**Estados de conexión y señal:**
- **Excelente/Buena** — Sincronización óptima
- **Regular** — La sincronización puede ser lenta
- **Débil/Sin señal** — No es posible sincronizar
- Presiona el indicador de señal para ver detalles

**Condiciones:**
- Las actividades pendientes se sincronizan automáticamente cuando hay conexión
- Puedes forzar la sincronización desde **Inicio** (icono de sincronización) o desde **Recolector > Menú > Estado de sincronización**

---

## 7. DIAGRAMA DE FLUJO COMPLETO

```
APLICACIÓN INICIADA
        │
        ▼
    ┌─────────┐
    │  SPLASH  │
    └────┬─────┘
         │
    ┌────┴─────┐
    │ ¿Sesión  │
    │ activa?  │
    └────┬─────┘
         │
    ┌────┴────┐        ┌───────────────────┐
    │   SÍ    │        │        NO         │
    └────┬────┘        └───────┬───────────┘
         │                     │
         ▼                     ▼
    ┌──────────┐      ┌─────────────────┐
    │  MENÚ    │      │   BIENVENIDA    │
    │ PRINCIPAL│      └────────┬────────┘
    │          │               │
    │ 3 tabs:  │    ┌──────────┴──────────┐
    │          │    │ ¿Qué deseas hacer?  │
    │ Inicio   │    ├─────────────────────┤
    │ Activ.   │    │ "Registrarme"      │
    │ Perfil   │    │   │ (7 pasos)       │
    └──────────┘    │   ▼                │
         │         │ ┌──────────────┐   │
         │         │ │ 1. QR/Código │   │
         │         │ │ 2. DNI       │   │
         │         │ │ 3. Celular   │   │
         │         │ │ 4. Pago      │   │
         │         │ │ 5. Fotos DNI │   │
         │         │ │ 6. Selfie    │   │
         │         │ │ 7. Firma     │   │
         │         │ └──────┬───────┘   │
         │         │        ▼          │
         │         │ ┌──────────────┐   │
         │         │ │   ÉXITO     │   │
         │         │ │ → MENÚ      │   │
         │         │ └──────────────┘   │
         │         │                    │
         │         │ "Ya tengo cuenta"  │
         │         │   │                │
         │         │   ▼                │
         │         │ ┌──────────────┐   │
         │         │ │   LOGIN     │   │
         │         │ │ DNI+3dig    │   │
         │         │ │   → OTP     │   │
         │         │ │   → MENÚ    │   │
         │         │ └──────────────┘   │
         │         └────────────────────┘
         │
    ┌────┴────────────────────────────────────┐
    │           MENÚ PRINCIPAL                │
    ├─────────────────────────────────────────┤
    │ [INICIO]                                 │
    │ Info del proyecto, comunidad, brigada    │
    │ Mapa del área                            │
    │ Estado de GPS                            │
    │ Sincronización manual                    │
    ├─────────────────────────────────────────┤
    │ [ACTIVIDADES]                            │
    │ PENDIENTES (borradores + pendientes)     │
    │   → Presionar "+" → Formulario           │
    │   → Llenar campos → Guardar/Enviar       │
    │ HISTORIAL (filtro por fecha)             │
    ├─────────────────────────────────────────┤
    │ [RECOLECTOR]                             │
    │ Datos personales                         │
    │ Mis Pagos (ver/editar)                   │
    │ Mi Comunidad (proyecto/brigadas)         │
    │ Opciones: sincronización, editar foto,   │
    │   cerrar sesión                          │
    └──────────────────────────────────────────┘
```

---

## 8. CONDICIONES Y COMPORTAMIENTOS ESPECIALES

| Situación | Comportamiento |
|---|---|
| **Cuenta archivada** | Diálogo forzoso → Solo puedes aceptar y cerrar sesión |
| **Recolector inactivo** | No puedes crear nuevas actividades; solo ver información |
| **Sin conexión a internet** | Las actividades se guardan localmente y se envían cuando hay conexión |
| **Fuera del área del proyecto** | No puedes crear actividades nuevas, pero sí puedes forzar el envío |
| **Código OTP expirado** | Presiona "Reenviar código" para recibir uno nuevo |
| **3 intentos fallidos de OTP** | Debes volver a la pantalla de inicio de sesión |
| **Actividades pendientes al cerrar sesión** | Advertencia de pérdida de datos locales |
| **Cierre inesperado de la app** | Los borradores se guardan automáticamente |

---

## 9. GLOSARIO DE TÉRMINOS

| Término | Significado |
|---|---|
| **OTP** | Código de verificación de un solo uso enviado por SMS |
| **Geocerca (Geofence)** | Área geográfica del proyecto; debes estar dentro para registrar actividades |
| **Unidad Forestal** | Árbol o troza que se está registrando |
| **Troza** | Parte de un árbol (tronco cortado) que se recolecta |
| **Inventario** | Etapa del proyecto donde se registran los árboles en pie |
| **Recolección** | Etapa del proyecto donde se registran las trozas |
| **Borrador** | Actividad guardada parcialmente, aún no completada |
| **Sincronización** | Proceso de enviar datos al servidor o recibir actualizaciones |
| **GeoJSON** | Formato de datos del mapa del proyecto |
| **Brigada** | Grupo de recolectores asignados a una solicitud específica |

---

*Documento generado a partir del análisis de código fuente de Pachamama Mobile versión Beta.*
