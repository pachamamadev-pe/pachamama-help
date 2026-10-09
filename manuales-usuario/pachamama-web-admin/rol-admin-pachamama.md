# Manual por Rol - ADMIN_PACHAMAMA

[Volver al manual principal](guia-definitiva-negocio.md)  
[Ver flujos comunes](flujos-comunes.md)

## Índice

1. [Propósito del rol](#proposito)
2. [Qué verá normalmente en su menú](#que-vera)
3. [Recorrido diario recomendado](#recorrido)
4. [Tareas clave por módulo](#tareas-clave)
5. [Límites y cuidados del rol](#limites-y-cuidados)
6. [Errores frecuentes](#errores-frecuentes)
7. [Checklist operativo](#checklist-operativo)

---

<a id="proposito"></a>
## 1. Propósito del rol

`ADMIN_PACHAMAMA` es el rol global de la plataforma.

En términos prácticos, este usuario:

- Opera módulos transversales.
- Supervisa varias áreas del sistema.
- Puede revisar más de una empresa según el contexto disponible.
- Funciona como rol de control, configuración y soporte funcional.

No es el rol ideal para capacitar operación cotidiana de una sola empresa. Su valor principal está en la visión global.

---

<a id="que-vera"></a>
## 2. Qué verá normalmente en su menú

Los módulos visibles pueden variar según el contexto recibido desde backend, pero normalmente este rol trabaja con:

- `Inicio`
- `Empresas`
- `Productos`
- `Comunidades`
- `Proyectos`
- `Formularios Dinámicos`
- `Lotes de Transformación`
- `Mi perfil`

### Qué encontrará con más frecuencia

| Módulo | Para qué lo usa |
|---|---|
| `Inicio` | Revisar la entrada general del sistema |
| `Empresas` | Crear empresas, asignar admins y completar documentos de empresa |
| `Productos` | Mantener catálogo, protocolos y conceptos globales |
| `Comunidades` | Revisar o apoyar gestión territorial cuando hace falta |
| `Proyectos` | Supervisar etapas, bloqueos y operación transversal |
| `Formularios Dinámicos` | Validar formularios de empresa o proyecto |
| `Lotes de Transformación` | Soporte y revisión de transformación primaria o secundaria |

---

<a id="recorrido"></a>
## 3. Recorrido diario recomendado

### Paso a paso

1. Ingresar a la plataforma.
2. Revisar `Inicio` para ubicarse en el estado general.
3. Entrar a `Empresas` si el trabajo del día es alta, actualización o soporte de tenant.
4. Entrar a `Productos` si se necesita ajustar catálogo o protocolos.
5. Entrar a `Proyectos` para revisar bloqueos, etapas o inconsistencias operativas.
6. Entrar a módulos especializados solo cuando el caso requiera soporte transversal.

### Qué verá normalmente

- Más amplitud de acceso que otros roles.
- Módulos que para otros usuarios están ocultos.
- Casos donde una pantalla depende igualmente de contexto de empresa o tenant.

---

<a id="tareas-clave"></a>
## 4. Tareas clave por módulo

### Empresas

#### Qué hace aquí

Administra empresas y su estructura básica.

#### Paso a paso

1. Entrar a `Empresas`.
2. Buscar la empresa o crear una nueva.
3. Completar los datos principales.
4. Asignar administradores si hace falta.
5. Abrir el flujo documental de empresa.

#### Qué debe recordar

- Al crear empresa, la plataforma abre el flujo documental de inmediato.
- La documentación puede completarse más tarde, pero conviene dejar claro el estado.

### Productos

#### Qué hace aquí

Mantiene el catálogo de productos a nivel transversal.

#### Tareas comunes

- Crear productos.
- Editar datos principales.
- Ajustar protocolos.
- Mantener conceptos o requerimientos especiales.

#### Qué debe recordar

- Este rol puede encontrarse con acciones que otros roles no ven, como edición más amplia del detalle de producto.

### Proyectos

#### Qué hace aquí

Usa proyectos para supervisión y soporte funcional.

#### Qué suele revisar

- Etapa actual del proyecto.
- Bloqueos para avanzar.
- Estado documental.
- Estado del mapa.
- Recolectores, brigadas, actividades y lotes si el caso lo requiere.

### Formularios Dinámicos

#### Qué hace aquí

Revisa o valida la estructura de formularios que alimentan la operación.

#### Qué suele hacer

- Ver formularios publicados, borradores o archivados.
- Abrir historial.
- Confirmar que un formulario esté alineado a producto, etapa y ámbito.

### Lotes de Transformación

#### Qué hace aquí

Supervisa la parte de transformación cuando necesita diagnóstico o soporte.

#### Qué suele revisar

- Si el lote está bloqueado por documento faltante.
- Si el lote ya fue usado en otro flujo y por eso quedó sin edición.
- Si la ubicación o QR están disponibles.

---

<a id="limites-y-cuidados"></a>
## 5. Límites y cuidados del rol

- No asumir que todos los módulos tenant-scoped funcionan igual para todos los contextos.
- Verificar siempre en qué empresa o tenant está operando realmente.
- No usar este rol como atajo para entrenamiento diario de usuarios de empresa.
- Confirmar si una diferencia es de permisos, de tenant o de etapa antes de reportarla como bug.

---

<a id="errores-frecuentes"></a>
## 6. Errores frecuentes

- Si un módulo dependiente de empresa no carga bien, revisar contexto de tenant.
- Si un usuario no ve menú, revisar permisos y menú devuelto por backend.
- Si una empresa queda incompleta, revisar su documentación y admins asignados.
- Si una pantalla existe pero se comporta de forma parcial, revisar si fue pensada para contexto de empresa y no solo para superadmin.

---

<a id="checklist-operativo"></a>
## 7. Checklist operativo

- Confirmar el tenant o empresa sobre la que está trabajando.
- Revisar si el caso es de catálogo, empresa, proyecto o transformación.
- Validar permisos y menú visibles antes de escalar un problema.
- Entrar al detalle de proyecto solo cuando necesite revisar el flujo operativo real.
