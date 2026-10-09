# Manual por Rol - GESTOR_TRANSFORMACION_PRIMARIA

[Volver al manual principal](guia-definitiva-negocio.md)  
[Ver flujos comunes](flujos-comunes.md)

## Índice

1. [Propósito del rol](#proposito)
2. [Qué verá normalmente en su menú](#que-vera)
3. [Recorrido diario recomendado](#recorrido)
4. [Tareas clave del rol](#tareas-clave)
5. [Bloqueos y validaciones reales](#bloqueos-y-validaciones)
6. [Errores frecuentes](#errores-frecuentes)
7. [Checklist operativo](#checklist-operativo)

---

<a id="proposito"></a>
## 1. Propósito del rol

`GESTOR_TRANSFORMACION_PRIMARIA` opera los lotes y las etapas de transformación primaria.

Su foco no está en crear proyectos ni en manejar comunidades, sino en convertir lotes de acopio en lotes de transformación primaria correctamente documentados.

---

<a id="que-vera"></a>
## 2. Qué verá normalmente en su menú

- `Proyectos` en modo de consulta
- `Lotes de Transformación`
- `Formularios Dinámicos` si su empresa lo usa de ese modo
- `Mi perfil`

### Qué encontrará con más frecuencia

| Módulo | Para qué lo usa |
|---|---|
| `Lotes de Transformación` | Crear, revisar y procesar lotes primarios |
| `Proyectos` | Consultar contexto del proyecto asociado |

---

<a id="recorrido"></a>
## 3. Recorrido diario recomendado

### Paso a paso

1. Entrar a `Lotes de Transformación`.
2. Filtrar por producto o proyecto si hace falta.
3. Revisar si hay lotes en curso.
4. Crear un lote primario desde lotes de acopio disponibles si corresponde.
5. Abrir el detalle del lote.
6. Operar sus etapas en orden.
7. Generar documentos y avanzar hasta almacenamiento.

---

<a id="tareas-clave"></a>
## 4. Tareas clave del rol

### Crear lote primario

#### Paso a paso

1. Elegir `Nuevo lote primario`.
2. Seleccionar los lotes de acopio disponibles.
3. Completar la recepción por lote fuente.
4. Confirmar totales.
5. Registrar notas si hace falta.
6. Confirmar ubicación.
7. Crear el lote.

### Operar etapas del lote

#### Secuencia real

1. `Recepción`
2. `Acondicionado`
3. `Ablandamiento` si aplica
4. `Pulpeado`
5. `Envasado`
6. `Almacenamiento`

### Qué hace dentro del detalle

- Generar documento de la etapa.
- Revisar PDF generado.
- Guardar datos de proceso.
- Avanzar de etapa.
- Ver ubicación del lote si el permiso está disponible.
- Generar QR si el flujo y permiso lo permiten.

---

<a id="bloqueos-y-validaciones"></a>
## 5. Bloqueos y validaciones reales

- No se puede avanzar si el documento de la etapa actual no está generado.
- `Ablandamiento` es una etapa opcional.
- Si el lote primario ya fue usado como fuente para un lote secundario, se bloquea su edición.
- Si el usuario está viendo una etapa anterior o ya cerrada, puede encontrar el lote solo como lectura.

---

<a id="errores-frecuentes"></a>
## 6. Errores frecuentes

- Si no aparece el botón para avanzar, revisar si el documento de la etapa está generado.
- Si no deja editar, revisar si el lote ya fue usado en transformación secundaria.
- Si no aparece la sección primaria, revisar permisos de lectura o procesamiento.
- Si no hay lotes disponibles para crear uno nuevo, revisar disponibilidad de lotes de acopio fuente.

---

<a id="checklist-operativo"></a>
## 7. Checklist operativo

- Confirmar qué lotes están en curso.
- Verificar que cada etapa tenga su documento generado.
- No avanzar una etapa sin revisar el PDF o registro correspondiente.
- Confirmar si el lote quedó bloqueado por uso en secundaria antes de reportar una falla.
