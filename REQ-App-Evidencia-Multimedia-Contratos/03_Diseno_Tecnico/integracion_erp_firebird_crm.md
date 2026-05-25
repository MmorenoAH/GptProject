# Integración ERP - Firebird - Zoho CRM

## Objetivo
Documentar el estado actual de la integración entre el ERP, la base Firebird y Zoho CRM, así como los ajustes necesarios para soportar la captura de evidencia multimedia desde Zoho Forms.

## Estado actual conocido
Actualmente los contratos se sincronizan desde el ERP hacia Zoho CRM en un módulo específico de contratos.

## Información disponible en el módulo de contratos
Campos sincronizados actualmente:
- Número de contrato.
- Cliente.
- Tipo de pago.
- Fecha de creación en ERP.

## Evaluación técnica inicial
La existencia de un módulo específico de contratos en Zoho CRM es positiva porque permite que Zoho Forms pueda usar el contrato como punto de referencia para la captura de evidencia.

Sin embargo, la información sincronizada actualmente es limitada para el objetivo completo del proyecto, porque la evidencia debe asociarse no solo al contrato, sino también al equipo específico y al tipo de movimiento operativo.

## Brecha identificada
Para que el formulario sea realmente dinámico y útil, se necesita validar cómo se obtendrá la información de equipos asociados al contrato.

Información pendiente o requerida:
- Equipos asociados al contrato.
- Código o identificador del equipo.
- Descripción del equipo.
- Estado o vigencia del equipo dentro del contrato.
- Relación entre contrato y movimientos operativos, si aplica.
- Referencia de remito, devolución o cambio de mercadería, si aplica.

## Riesgo principal
Si Zoho Forms solo puede consultar el módulo de contratos con información básica, el usuario de bodega podría seleccionar el contrato, pero tendría que ingresar manualmente el equipo. Esto reduce la confiabilidad del registro y puede generar errores de trazabilidad.

## Opciones de solución

### Opción A: Ampliar sincronización hacia Zoho CRM
Sincronizar también los equipos asociados al contrato hacia Zoho CRM, preferiblemente como módulo relacionado o subformulario relacionado.

Ventajas:
- Mejor experiencia para bodega.
- Menos captura manual.
- Mayor consistencia en la evidencia.
- Mejor consulta histórica por contrato y equipo.

Riesgos:
- Requiere ajuste en integración existente.
- Puede requerir revisar modelo de datos del ERP.
- Puede necesitar control de actualización frecuente.

### Opción B: Captura manual del equipo en Zoho Forms
Permitir que bodega ingrese o seleccione manualmente el equipo dentro del formulario.

Ventajas:
- Más rápido de implementar.
- Menor dependencia inicial de integración.

Riesgos:
- Mayor posibilidad de errores.
- Menor trazabilidad.
- Dificulta búsquedas históricas confiables por equipo.

### Opción C: Catálogo intermedio de equipos por contrato
Crear o alimentar una estructura intermedia en Zoho con los equipos activos por contrato, aunque no sea una réplica completa del ERP.

Ventajas:
- Puede ser más simple que sincronizar todos los movimientos.
- Permite que Zoho Forms filtre mejor la selección.
- Mantiene el ERP como fuente principal.

Riesgos:
- Requiere definir frecuencia de actualización.
- Requiere reglas claras de vigencia.

## Recomendación inicial
La opción recomendada es ampliar la sincronización para que Zoho CRM tenga al menos la relación contrato-equipo necesaria para el formulario. No se recomienda depender de captura manual de equipo como solución final, salvo para una prueba piloto controlada.

## Decisión pendiente
Definir si los equipos asociados al contrato se sincronizarán como:
- Módulo propio de equipos contratados.
- Registros relacionados dentro del módulo de contratos.
- Subformulario dentro del contrato.
- Catálogo intermedio consultable desde Zoho Forms.

## Pregunta clave pendiente
¿El ERP permite extraer de forma confiable los equipos activos o vinculados a cada contrato desde Firebird para sincronizarlos hacia Zoho CRM?
