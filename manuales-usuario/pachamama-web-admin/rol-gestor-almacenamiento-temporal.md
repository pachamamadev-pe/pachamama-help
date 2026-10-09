# Manual por Rol - GESTOR_ALMACENAMIENTO_TEMPORAL

[Volver al manual principal](guia-definitiva-negocio.md)  
[Ver flujos comunes](flujos-comunes.md)

## Índice

1. [Propósito del rol](#proposito)
2. [Qué verá normalmente en su menú](#que-vera)
3. [Recorrido diario recomendado](#recorrido)
4. [Tareas clave del rol](#tareas-clave)
5. [Límites del rol](#limites-del-rol)
6. [Errores frecuentes](#errores-frecuentes)
7. [Checklist operativo](#checklist-operativo)

---

<a id="proposito"></a>
## 1. Propósito del rol

`GESTOR_ALMACENAMIENTO_TEMPORAL` trabaja en un tramo acotado del flujo de transformación primaria.

Su foco es la etapa de `almacenamiento` de los lotes primarios.

---

<a id="que-vera"></a>
## 2. Qué verá normalmente en su menú

- `Proyectos` en modo de consulta
- `Lotes de Transformación`
- `Mi perfil`

### Qué ve realmente este rol

- Acceso a la sección de transformación primaria.
- Vista filtrada a lotes en estado `almacenamiento` cuando opera como usuario solo de almacenamiento.
- Detalle del lote con edición limitada a esa etapa.

---

<a id="recorrido"></a>
## 3. Recorrido diario recomendado

### Paso a paso

1. Entrar a `Lotes de Transformación`.
2. Revisar lotes primarios en estado `almacenamiento`.
3. Abrir el detalle del lote.
4. Completar o revisar el documento de almacenamiento.
5. Guardar el registro correspondiente.

---

<a id="tareas-clave"></a>
## 4. Tareas clave del rol

### Lista de lotes

#### Qué hace aquí

Revisa los lotes que ya llegaron a almacenamiento.

#### Qué debe recordar

- La plataforma puede mostrar una lista mucho más corta que a otros roles porque filtra a almacenamiento.

### Detalle del lote

#### Qué hace aquí

Completa o consulta la etapa de almacenamiento.

#### Tareas comunes

- Revisar el estado del lote.
- Confirmar que se está trabajando realmente sobre `almacenamiento`.
- Completar o guardar el registro permitido para esa etapa.

---

<a id="limites-del-rol"></a>
## 5. Límites del rol

- No es el rol principal para crear lotes primarios.
- No es el rol principal para procesar recepción, pulpeado o envasado.
- No opera lotes secundarios.
- Si entra a etapas previas, normalmente las verá sin edición operativa.

---

<a id="errores-frecuentes"></a>
## 6. Errores frecuentes

- Si la pantalla muestra pocos lotes, recordar que este rol puede estar filtrado por estado.
- Si no puede editar, confirmar que está viendo la etapa correcta del lote.
- Si no hay lotes visibles, revisar que realmente existan lotes en `almacenamiento`.

---

<a id="checklist-operativo"></a>
## 7. Checklist operativo

- Confirmar que el lote está en `almacenamiento`.
- Revisar si la etapa está abierta a edición.
- Guardar solo el documento o registro correspondiente a almacenamiento.
- No escalar como bug un bloqueo que en realidad corresponde al alcance del rol.
