# Integración ERP - Firebird - Zoho CRM

## Objetivo
Documentar el estado actual de la integración entre el ERP, la base Firebird y Zoho CRM, así como los ajustes necesarios para soportar la captura de evidencia multimedia desde Zoho Forms.

## Estado actual conocido
Actualmente los contratos se sincronizan desde el ERP hacia Zoho CRM en un módulo específico de contratos.

La integración fue realizada por un proveedor de desarrollo. La empresa cuenta con acceso a los códigos de integración en Zoho, swagger del ERP, credenciales de conexión y conexiones nativas configuradas.

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
Si Zoho Forms solo puede consultar el módulo de contratos con información básica, el usuario de bodega podría seleccionar el contrato, pero tendría que ingresar manualmente el equipo. Esto permite avanzar, pero reduce la confiabilidad del registro y puede generar errores de trazabilidad si no se controla.

## Estrategia aprobada por fases

### Fase 1: Captura manual controlada
Durante el desarrollo inicial se permitirá la captura manual del equipo para no retrasar el avance funcional.

Esta fase sirve para validar:
- Formulario.
- Checklist.
- Carga multimedia.
- Almacenamiento en Google Drive.
- Consulta de historial en Zoho.
- Aceptación operativa por bodega y cartera.

### Fase 2: Catálogo intermedio provisional
Para las primeras pruebas en producción se evaluará un catálogo intermedio de equipos por contrato, reduciendo captura manual sin depender todavía de una sincronización completa.

### Fase 3: Ampliación de sincronización hacia Zoho CRM
El objetivo final será ampliar la sincronización hacia Zoho CRM para incluir la relación contrato-equipo, una vez que la solución sea validada como funcional.

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
- Útil para validar el flujo durante el desarrollo.

Riesgos:
- Mayor posibilidad de errores.
- Menor trazabilidad.
- Dificulta búsquedas históricas confiables por equipo si se mantiene como solución definitiva.

### Opción C: Catálogo intermedio de equipos por contrato
Crear o alimentar una estructura intermedia en Zoho con los equipos activos por contrato, aunque no sea una réplica completa del ERP.

Ventajas:
- Puede ser más simple que sincronizar todos los movimientos.
- Permite que Zoho Forms filtre mejor la selección.
- Mantiene el ERP como fuente principal.
- Sirve como puente entre captura manual y sincronización final.

Riesgos:
- Requiere definir frecuencia de actualización.
- Requiere reglas claras de vigencia.
- No debe convertirse en solución final sin control formal.

## Recomendación actualizada
La estrategia recomendada es avanzar por fases:

1. Captura manual controlada para acelerar desarrollo.
2. Catálogo intermedio para pruebas iniciales en producción.
3. Ampliación de sincronización hacia Zoho CRM como solución final.

## Decisión pendiente
Definir si los equipos asociados al contrato se sincronizarán finalmente como:
- Módulo propio de equipos contratados.
- Registros relacionados dentro del módulo de contratos.
- Subformulario dentro del contrato.
- Catálogo intermedio consultable desde Zoho Forms.

## Pregunta clave pendiente
¿El ERP permite extraer de forma confiable los equipos activos o vinculados a cada contrato desde Firebird o desde el swagger del ERP para sincronizarlos hacia Zoho CRM?
