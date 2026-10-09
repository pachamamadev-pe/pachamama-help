# Manual por Rol - GESTOR_TRANSFORMACION_SECUNDARIA

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

`GESTOR_TRANSFORMACION_SECUNDARIA` opera la transformación secundaria y la trazabilidad asociada.

Trabaja con lotes secundarios, lotes fuente, transporte y QR finales.

---

<a id="que-vera"></a>
## 2. Qué verá normalmente en su menú

- `Proyectos` en modo de consulta
- `Lotes de Transformación`
- `Mi perfil`

### Qué encontrará con más frecuencia

| Módulo | Para qué lo usa |
|---|---|
| `Lotes de Transformación` | Crear y operar lotes secundarios |
| `Proyectos` | Consultar el contexto del proyecto relacionado |

---

<a id="recorrido"></a>
## 3. Recorrido diario recomendado

### Paso a paso

1. Entrar a `Lotes de Transformación`.
2. Ir a la sección de lotes secundarios.
3. Crear un nuevo lote secundario si corresponde.
4. Seleccionar lotes primarios disponibles.
5. Definir aportes de cada lote fuente.
6. Completar transporte y ubicación.
7. Generar documentos y QR.

---

<a id="tareas-clave"></a>
## 4. Tareas clave del rol

### Crear lote secundario

#### Paso a paso

1. Elegir `Nuevo lote secundario`.
2. Seleccionar lotes primarios disponibles.
3. Definir el aporte de cada lote fuente.
4. Completar el resumen del lote.
5. Registrar transporte.
6. Confirmar ubicación.
7. Crear el lote.

### Detalle del lote secundario

#### Qué hace aquí

Opera la recepción secundaria y el transporte del lote.

#### Tareas comunes

- Generar ficha de recepción secundaria.
- Revisar lotes fuente.
- Guardar guía o documento de transporte.
- Ver ubicación del lote.
- Generar QR de trazabilidad.
- Generar QR para cliente si el permiso existe.

---

<a id="bloqueos-y-validaciones"></a>
## 5. Bloqueos y validaciones reales

- El flujo depende de lotes primarios disponibles.
- El documento de recepción secundaria bloquea cambios posteriores de ese paso.
- El transporte fluvial requiere matrícula de embarcación.
- El detalle puede alternar entre panel de recepción y panel de transporte según documento existente.

---

<a id="errores-frecuentes"></a>
## 6. Errores frecuentes

- Si no aparece el botón de crear lote, revisar permisos de creación.
- Si no aparecen lotes fuente, revisar disponibilidad real de lotes primarios.
- Si no deja guardar transporte fluvial, completar matrícula de embarcación.
- Si no carga el PDF, volver a abrir el detalle o revisar el documento generado.

---

<a id="checklist-operativo"></a>
## 7. Checklist operativo

- Confirmar disponibilidad de lotes primarios.
- Revisar los aportes de cada lote fuente.
- Generar recepción secundaria antes de dar el paso por cerrado.
- Completar el transporte con los datos obligatorios.
- Generar QR solo cuando el lote ya tenga la información necesaria.
