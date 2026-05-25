# Flujo funcional: entrega y recepción de equipos

## Objetivo
Definir el flujo operativo futuro para capturar evidencia multimedia y checklist durante entregas y recepciones de equipos, usando Zoho Forms como punto principal de captura.

## Principio funcional
La evidencia debe capturarse en el momento operativo, desde un dispositivo móvil, asociada desde el inicio a contrato, equipo, tipo de movimiento, usuario responsable, fecha, checklist y archivos multimedia.

---

# Flujo de entrega

## Actor principal
Usuario de Bodega de Alquiler.

## Flujo propuesto
1. El usuario de bodega abre el formulario de captura en Zoho Forms.
2. Selecciona o busca el número de contrato.
3. El formulario muestra o permite seleccionar los equipos asociados al contrato.
4. El usuario selecciona el equipo que será entregado.
5. Selecciona el tipo de movimiento: Entrega.
6. El formulario carga el checklist correspondiente a entrega.
7. El usuario completa los campos requeridos del checklist.
8. Adjunta fotografías del estado del equipo.
9. Adjunta fotografías de accesorios, si aplica.
10. Registra observaciones relevantes.
11. Envía el formulario.
12. El registro queda disponible en Zoho para consulta posterior.
13. Los archivos multimedia quedan almacenados en Google Drive según la estructura definida.

## Resultado esperado
La entrega queda documentada con evidencia multimedia, checklist y trazabilidad mínima del movimiento.

---

# Flujo de recepción

## Actor principal
Usuario de Bodega de Alquiler.

## Flujo propuesto
1. El usuario de bodega abre el formulario de captura en Zoho Forms.
2. Selecciona o busca el número de contrato.
3. Selecciona el equipo que está siendo recibido.
4. Selecciona el tipo de movimiento: Recepción.
5. El formulario carga el checklist correspondiente a recepción.
6. El usuario revisa el estado físico del equipo.
7. Completa el checklist de recepción.
8. Adjunta fotografías del estado general del equipo.
9. Adjunta fotografías de daños visibles, si aplica.
10. Registra observaciones.
11. Envía el formulario.
12. El registro queda disponible en Zoho para consulta posterior.
13. Los archivos multimedia quedan almacenados en Google Drive según la estructura definida.

## Resultado esperado
La recepción queda documentada con evidencia suficiente para respaldar el estado del equipo al momento de devolución.

---

# Consulta de historial

## Actor principal
Cartera y Cobro.

## Flujo propuesto
1. El usuario de cartera ingresa al entorno Zoho.
2. Busca por número de contrato, cliente o equipo.
3. Revisa los registros de evidencia asociados.
4. Filtra por tipo de movimiento si es necesario.
5. Abre el registro correspondiente.
6. Consulta checklist, observaciones y evidencia multimedia.
7. Utiliza la información como respaldo operativo o comercial.

## Restricción recomendada
Cartera debe consultar la evidencia, pero no editarla ni eliminarla.

---

# Reglas funcionales iniciales

## Reglas obligatorias
- Todo registro debe tener número de contrato.
- Todo registro debe tener equipo asociado.
- Todo registro debe tener tipo de movimiento.
- Todo registro debe tener usuario responsable.
- Todo registro debe tener fecha y hora de captura.
- Todo registro debe incluir evidencia multimedia mínima.
- Todo registro debe incluir checklist completo según el tipo de movimiento.

## Reglas recomendadas
- El formulario debe impedir envío si falta evidencia mínima.
- El formulario debe ajustar campos requeridos según tipo de movimiento.
- Los registros enviados no deben ser editables por usuarios consultores.
- Las evidencias deben almacenarse con una nomenclatura trazable.

---

# Pendientes de validación

- Confirmar si Zoho Forms puede mostrar equipos filtrados por contrato usando la estructura actual de Zoho CRM.
- Confirmar si se usará un solo formulario para todos los movimientos o formularios separados por tipo de movimiento.
- Definir cantidad mínima de fotografías por entrega.
- Definir cantidad mínima de fotografías por recepción.
- Definir si se requiere firma o aceptación del cliente.
- Definir si la evidencia se bloquea después del envío.
- Definir si bodega puede corregir registros enviados y bajo qué condiciones.
