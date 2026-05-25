# Casos de prueba iniciales

## CP-001 Captura de entrega
**Objetivo:** Validar que bodega pueda registrar evidencia de entrega de equipo.

**Pasos:**
1. Abrir formulario.
2. Seleccionar contrato.
3. Seleccionar equipo.
4. Seleccionar tipo de movimiento: Entrega.
5. Completar checklist.
6. Adjuntar evidencia multimedia.
7. Enviar registro.

**Resultado esperado:** Registro creado correctamente con contrato, equipo, checklist y evidencia asociada.

## CP-002 Captura de recepción
**Objetivo:** Validar que bodega pueda registrar evidencia de recepción.

**Resultado esperado:** Registro consultable desde Zoho por contrato y equipo.

## CP-003 Consulta por cartera
**Objetivo:** Validar que cartera pueda consultar historial sin modificar evidencia.

**Resultado esperado:** Usuario de cartera visualiza registros y archivos, pero no puede editar ni eliminar evidencia.

## CP-004 Contrato sin equipos disponibles
**Objetivo:** Validar comportamiento cuando un contrato no muestra equipos asociados.

**Resultado esperado:** El sistema muestra mensaje claro o impide continuar hasta corregir la referencia.

## CP-005 Evidencia incompleta
**Objetivo:** Validar que el formulario exija evidencia mínima.

**Resultado esperado:** El formulario no permite enviar si faltan archivos requeridos.
