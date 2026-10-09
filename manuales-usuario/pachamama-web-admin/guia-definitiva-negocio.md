# Manual de Usuario - Pachamama Web Admin

**Dirigido a:** Equipo de negocio, operación, supervisión y validación funcional  
**Objetivo:** Explicar cómo usar la web admin de forma clara y práctica según el rol  
**Incluye:** Flujos comunes, módulos reales de la UI y manuales específicos por rol

---

## Índice

1. [Propósito de esta guía](#proposito)
2. [Cómo está organizada esta guía](#como-esta-organizada-esta-guia)
3. [Cómo funciona el acceso por rol y permisos](#como-funciona-el-acceso-por-rol-y-permisos)
4. [Qué ve cualquier usuario al ingresar](#que-ve-cualquier-usuario-al-ingresar)
5. [Módulos principales de la web admin](#modulos-principales-de-la-web-admin)
6. [El detalle de proyecto como centro de operación](#el-detalle-de-proyecto-como-centro-de-operacion)
7. [Manuales por rol](#manuales-por-rol)
8. [Qué diferencias pueden existir entre empresas](#que-diferencias-pueden-existir-entre-empresas)
9. [Recomendaciones operativas para capacitación](#recomendaciones-operativas-para-capacitacion)
10. [Resumen final](#resumen-final)

---

<a id="proposito"></a>
## 1. Propósito de esta guía

Este manual organiza el uso de `pachamama-web-admin` desde la mirada de negocio y operación.

Su objetivo es ayudar a que el equipo pueda:

- Entender qué ve cada rol dentro de la plataforma.
- Capacitar usuarios sin depender solo de la lectura de permisos técnicos.
- Explicar la navegación real de la UI y no solo el catálogo teórico de módulos.
- Aterrizar el trabajo diario por rol: qué revisar, qué crear, qué aprobar y qué no debería tocar.

La base funcional de esta guía combina:

- La matriz interna de roles y permisos (documento interno, no publicado aqui).
- El comportamiento real de la UI en `pachamama-web-admin`.

---

<a id="como-esta-organizada-esta-guia"></a>
## 2. Cómo está organizada esta guía

Esta guía se divide en un documento principal, un documento común y un manual por rol.

| Documento | Para qué sirve | Quién debería leerlo primero |
|---|---|---|
| [FLUJOS_COMUNES_PACHAMAMA_WEB_ADMIN.md](flujos-comunes.md) | Login, navegación, perfil, proyectos, documentos, mapa, actividades, solicitudes, lotes y errores comunes | Todos |
| [ROL_ADMIN_PACHAMAMA.md](rol-admin-pachamama.md) | Uso operativo del rol global con acceso total | ADMIN_PACHAMAMA |
| [ROL_ADMIN_EMPRESA.md](rol-admin-empresa.md) | Operación integral de empresa, proyectos, usuarios y transformación | ADMIN_EMPRESA |
| [ROL_GESTOR_RELACIONAMIENTO_COMUNITARIO.md](rol-gestor-relacionamiento-comunitario.md) | Arranque operativo: comunidades, productos, proyectos, PMF y recolección | GESTOR_RELACIONAMIENTO_COMUNITARIO |
| [ROL_GESTOR_TRANSFORMACION_PRIMARIA.md](rol-gestor-transformacion-primaria.md) | Gestión de lotes y etapas de transformación primaria | GESTOR_TRANSFORMACION_PRIMARIA |
| [ROL_GESTOR_ALMACENAMIENTO_TEMPORAL.md](rol-gestor-almacenamiento-temporal.md) | Operación de almacenamiento dentro de lotes primarios | GESTOR_ALMACENAMIENTO_TEMPORAL |
| [ROL_GESTOR_TRANSFORMACION_SECUNDARIA.md](rol-gestor-transformacion-secundaria.md) | Gestión de lotes y trazabilidad de transformación secundaria | GESTOR_TRANSFORMACION_SECUNDARIA |
| [ROL_RECOLECTOR_ADMINISTRADOR.md](rol-recolector-administrador.md) | Gestión operativa de recolectores, brigadas, actividades y solicitudes | RECOLECTOR_ADMINISTRADOR |

Orden de lectura recomendado:

1. Este documento principal.
2. `FLUJOS_COMUNES_PACHAMAMA_WEB_ADMIN.md`.
3. El manual del rol correspondiente.

---

<a id="como-funciona-el-acceso-por-rol-y-permisos"></a>
## 3. Cómo funciona el acceso por rol y permisos

En la web admin, el acceso no depende solo del nombre del rol.

También depende de:

- Los permisos concretos entregados al usuario.
- El menú lateral que devuelve el backend para ese usuario.
- La etapa del proyecto donde está trabajando.
- La configuración activa de la empresa.

En la práctica esto significa:

- Dos usuarios con el mismo rol pueden ver diferencias si su empresa o parametrización no es exactamente la misma.
- Un módulo puede existir en la plataforma, pero no aparecer en el menú de un usuario concreto.
- Un usuario puede entrar a un proyecto, pero no ver todas sus pestañas si no tiene el permiso correspondiente.
- Algunas acciones solo se habilitan en determinadas etapas del proyecto.
- Si existe diferencia entre la matriz teórica del rol y la UI real del usuario, para capacitación debe prevalecer lo que efectivamente aparece en su menú y en sus pantallas.

Regla simple para capacitación:

- Si una pantalla no aparece, primero revisar rol y permisos.
- Si un botón aparece deshabilitado, revisar etapa del proyecto y requisitos previos.
- Si el usuario entra pero no ve ningún módulo útil, su sesión queda bloqueada por falta de acceso operativo.

---

<a id="que-ve-cualquier-usuario-al-ingresar"></a>
## 4. Qué ve cualquier usuario al ingresar

Todo usuario parte de una estructura común.

| Zona | Qué ve normalmente |
|---|---|
| `Login` | Correo, contraseña, recuperación de contraseña y mensajes de error o verificación |
| `Sidebar` | Solo los módulos habilitados para su rol y permisos |
| `Header` | Título de la pantalla, nombre de empresa, avatar, rol y menú de usuario |
| `Inicio` | Dashboard si el rol lo permite, o entrada al flujo general de la plataforma |
| `Mi perfil` | Datos personales, avatar y cambio de contraseña |

Puntos importantes:

- La plataforma exige correo verificado antes de permitir el ingreso operativo.
- Si la contraseña aún no fue cambiada, la UI obliga a completar ese paso.
- El menú lateral es dinámico y puede cambiar entre usuarios.
- `Mi perfil` está disponible para todos los roles documentados.

---

<a id="modulos-principales-de-la-web-admin"></a>
## 5. Módulos principales de la web admin

Estos son los módulos principales detectados en la UI real.

| Módulo | Para qué sirve | Roles que normalmente lo usan |
|---|---|---|
| `Inicio` | Revisar dashboard y entrar al trabajo diario | ADMIN_PACHAMAMA, ADMIN_EMPRESA y cualquier rol con acceso general |
| `Empresas` | Crear empresas, asignar admins y completar documentos | ADMIN_PACHAMAMA |
| `Productos` | Mantener catálogo, protocolos y detalle de producto | ADMIN_PACHAMAMA, ADMIN_EMPRESA, GESTOR_RELACIONAMIENTO_COMUNITARIO |
| `Comunidades` | Crear y actualizar comunidades | ADMIN_EMPRESA, GESTOR_RELACIONAMIENTO_COMUNITARIO |
| `Usuarios de Empresa` | Crear, editar, desactivar usuarios y asignar roles | ADMIN_EMPRESA |
| `Proyectos` | Crear proyectos, abrir detalle y seguir etapas | Casi todos los roles operativos |
| `Solicitudes de Recolección` | Crear, editar observadas y revisar solicitudes | ADMIN_EMPRESA, GESTOR_RELACIONAMIENTO_COMUNITARIO, RECOLECTOR_ADMINISTRADOR |
| `Formularios Dinámicos` | Crear, editar, publicar, copiar e historizar formularios | ADMIN_EMPRESA y roles con permiso de formularios |
| `Lotes de Transformación` | Operar transformación primaria y secundaria | ADMIN_EMPRESA, GESTOR_TRANSFORMACION_PRIMARIA, GESTOR_ALMACENAMIENTO_TEMPORAL, GESTOR_TRANSFORMACION_SECUNDARIA |
| `Tipos de Documento` | Gestionar catálogo documental de empresa | ADMIN_EMPRESA |
| `Mi perfil` | Datos personales, avatar y seguridad | Todos |

---

<a id="el-detalle-de-proyecto-como-centro-de-operacion"></a>
## 6. El detalle de proyecto como centro de operación

La pantalla de detalle del proyecto es el núcleo de la operación web.

Desde allí, la plataforma concentra:

- El avance de etapas.
- El mapa del proyecto.
- Los recolectores.
- Las brigadas.
- El registro y revisión de actividades.
- La generación de PMF.
- La revisión de solicitudes.
- Los lotes de acopio.
- Los documentos del proyecto.
- La configuración avanzada.

### Pestañas principales del detalle de proyecto

| Pestaña | Cuándo aparece | Para qué sirve |
|---|---|---|
| `Resumen` | Siempre | Ver progreso, KPIs, mapa y etapa actual |
| `Recolectores` | Si el usuario puede leer recolectores | Gestionar estados, revisar historial y generar QR de onboarding |
| `Brigadas` | Si el usuario puede leer brigadas | Crear brigadas, editarlas y agregar miembros |
| `Registro de actividades` | Si el usuario puede leer actividades y el proyecto ya superó `planning` | Revisar inventario o recolección y evaluar registros |
| `Generar PMF` | Si el usuario puede generar PMF y el proyecto está en `pmf_development` o `serfor_evaluation` | Generar el PMF y mover ese tramo del flujo |
| `Revisión Solicitudes` | Si el usuario puede leer solicitudes y el proyecto está en `collection` o posterior | Revisar solicitudes de recolección del proyecto |
| `Lotes de Acopio` | Si el usuario puede leer lotes de acopio y el proyecto está en `ctp_entry` o posterior | Crear lotes y procesar sus documentos |
| `Documentos` | Si el usuario puede leer documentos | Subir, descargar, revisar y resubir documentos |
| `Configuración` | Si el usuario puede leer fórmulas o agregaciones | Configurar columnas calculadas y agregaciones del proyecto |

### Reglas reales para avanzar etapas

| Etapa actual | Qué debe estar listo para avanzar |
|---|---|
| `planning` | Recolectores registrados, al menos una brigada, documentos obligatorios cargados y documentos obligatorios aprobados |
| `inventory` | Al menos una actividad registrada |
| `pmf_development` | Documento PMF aprobado |
| `serfor_evaluation` | Documentos obligatorios de esa etapa cargados y aprobados |
| `collection` | El backend valida condiciones adicionales |
| `ctp_entry` | El backend valida existencia de lotes con documentos generados |

Para el usuario esto se ve así:

- El botón `Avanzar a siguiente etapa` puede aparecer pero quedar deshabilitado.
- La UI muestra una ayuda con lo que todavía falta completar.
- No todas las pestañas están visibles desde el inicio del proyecto.

---

<a id="manuales-por-rol"></a>
## 7. Manuales por rol

Estos son los documentos que deben usarse para entrenamiento y operación diaria por tipo de usuario.

1. [ROL_ADMIN_PACHAMAMA.md](rol-admin-pachamama.md)
   Rol global. Puede operar módulos transversales y supervisar más de una empresa.
2. [ROL_ADMIN_EMPRESA.md](rol-admin-empresa.md)
   Rol más completo dentro de una empresa. Maneja usuarios, proyectos, documentos, formularios y lotes.
3. [ROL_GESTOR_RELACIONAMIENTO_COMUNITARIO.md](rol-gestor-relacionamiento-comunitario.md)
   Rol de arranque operativo. Trabaja comunidades, productos, proyectos, recolectores, PMF y recolección.
4. [ROL_GESTOR_TRANSFORMACION_PRIMARIA.md](rol-gestor-transformacion-primaria.md)
   Rol especializado en lotes y etapas de transformación primaria.
5. [ROL_GESTOR_ALMACENAMIENTO_TEMPORAL.md](rol-gestor-almacenamiento-temporal.md)
   Rol especializado en el tramo de almacenamiento de lotes primarios.
6. [ROL_GESTOR_TRANSFORMACION_SECUNDARIA.md](rol-gestor-transformacion-secundaria.md)
   Rol especializado en lotes secundarios, recepción, transporte y QR.
7. [ROL_RECOLECTOR_ADMINISTRADOR.md](rol-recolector-administrador.md)
   Rol operativo de campo para recolectores, brigadas, actividades y solicitudes.

---

<a id="que-diferencias-pueden-existir-entre-empresas"></a>
## 8. Qué diferencias pueden existir entre empresas

Aunque esta guía usa los roles documentados internamente, la experiencia final puede variar.

Las diferencias más habituales son:

- El menú lateral puede cambiar según la empresa y sus permisos activos.
- Los tipos de documento obligatorios cambian por etapa y por configuración.
- Algunas acciones aparecen solo cuando el proyecto está en una etapa específica.
- Hay pantallas existentes en el código que no deben tratarse como flujo principal de capacitación.

No deben usarse como recorrido principal del manual:

- `/brigades` como módulo independiente.
- `/projects/:id/enable-inventory` como flujo de negocio principal.
- `/projects/:id/areas/import` como entrada principal si el usuario normalmente llega por detalle de proyecto.

La recomendación correcta es capacitar siempre por:

1. Rol.
2. Módulos visibles en el menú real.
3. Etapa del proyecto donde ese usuario trabaja.

---

<a id="recomendaciones-operativas-para-capacitacion"></a>
## 9. Recomendaciones operativas para capacitación

- Empezar siempre por `FLUJOS_COMUNES_PACHAMAMA_WEB_ADMIN.md`.
- Luego usar el manual del rol específico.
- Capacitar con un proyecto de ejemplo en una etapa realista, no con un proyecto vacío si el rol depende de tabs por etapa.
- Reforzar que si un botón no aparece, no necesariamente es falla: puede ser permiso o etapa.
- Explicar bien la diferencia entre `subir`, `aprobar`, `observar`, `rechazar` y `resubir` documentos.
- En roles de transformación, entrenar también ubicación, bloqueo por documentos y bloqueo por lotes ya usados.
- En roles con proyectos, enseñar el botón de avance de etapa junto con sus bloqueos reales.

Orden sugerido para sesiones de capacitación:

1. Login, verificación de correo y cambio de contraseña.
2. Sidebar, header y perfil.
3. Proyectos y detalle de proyecto.
4. Flujo específico del rol.
5. Errores frecuentes y validaciones.

---

<a id="resumen-final"></a>
## 10. Resumen final

Pachamama Web Admin no es un único flujo lineal para todos los usuarios.

Su uso real depende de tres cosas:

1. El rol documentado.
2. Los permisos concretos activos para ese usuario.
3. La etapa del proyecto donde está operando.

En resumen:

- Este documento principal te dice cómo leer el ecosistema completo.
- El documento de flujos comunes te explica la navegación y los comportamientos compartidos.
- Los manuales por rol te dicen qué debe hacer cada usuario en su trabajo diario.

Siguiente lectura recomendada: [FLUJOS_COMUNES_PACHAMAMA_WEB_ADMIN.md](flujos-comunes.md)
