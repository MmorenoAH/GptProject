# Diseño funcional del formulario

## Objetivo
Definir la estructura funcional del formulario de captura de evidencia multimedia para entregas, recepciones y cambios de equipos.

## Decisión de diseño recomendada
Usar un formulario principal dinámico con campos condicionados por tipo de movimiento, siempre que Zoho Forms permita cubrir las reglas requeridas.

## Alternativa
Crear formularios separados por tipo de movimiento:
- Formulario de entrega.
- Formulario de recepción.
- Formulario de cambio de equipo.

## Evaluación inicial

### Formulario único dinámico
Ventajas:
- Menor mantenimiento.
- Un solo punto de acceso para bodega.
- Misma estructura de datos para consulta.
- Mejor para reportes e historial.

Riesgos:
- Puede volverse complejo si los checklist son muy distintos.
- Depende de reglas condicionales en Zoho Forms.
- Puede ser más difícil controlar errores si se agregan muchos escenarios.

### Formularios separados
Ventajas:
- Más simple para el usuario en cada caso.
- Reglas más fáciles de controlar.
- Checklist específico por proceso.

Riesgos:
- Mayor mantenimiento.
- Datos más fragmentados.
- Más difícil consolidar historial si no se normalizan bien los campos.

## Recomendación inicial
Iniciar con un formulario único dinámico si los campos base son comunes y los checklist no cambian drásticamente entre entrega y recepción.

Si el checklist de recepción requiere validaciones más complejas por condición del equipo, accesorios u observaciones especiales, considerar formularios separados.

---

# Secciones del formulario

## 1. Identificación del registro
Campos sugeridos:
- Número de contrato.
- Cliente.
- Equipo.
- Código del equipo.
- Tipo de movimiento.
- Fecha y hora.
- Usuario responsable.

## 2. Información del movimiento
Campos sugeridos:
- Sucursal o ubicación.
- Observaciones generales.
- Responsable que entrega o recibe.
- Referencia de comprobante ERP, si aplica.

## 3. Checklist operativo
Campos sugeridos para entrega:
- Equipo revisado físicamente.
- Equipo funcional al momento de entrega.
- Accesorios completos.
- Estado exterior documentado.
- Observaciones de entrega.

Campos sugeridos para recepción:
- Equipo recibido físicamente.
- Estado exterior revisado.
- Accesorios recibidos.
- Condición especial identificada, si aplica.
- Observaciones de recepción.

## 4. Evidencia multimedia
Campos sugeridos:
- Foto frontal del equipo.
- Foto lateral o posterior.
- Foto de número de serie o identificador.
- Foto de accesorios.
- Foto de condición especial, si aplica.
- Archivo adicional opcional.

## 5. Confirmación
Campos sugeridos:
- Confirmación de checklist completo.
- Confirmación de evidencia adjunta.
- Firma o aceptación, si aplica.

---

# Validaciones sugeridas

## Validaciones obligatorias
- Número de contrato requerido.
- Equipo requerido.
- Tipo de movimiento requerido.
- Evidencia multimedia mínima requerida.
- Checklist completo requerido.

## Validaciones condicionales
- Si tipo de movimiento es Recepción y se marca condición especial, exigir fotografía correspondiente.
- Si accesorios incompletos, exigir observación.
- Si equipo no aparece asociado al contrato, impedir envío o marcar como excepción.

---

# Pendientes

- Confirmar campos disponibles desde Zoho CRM.
- Confirmar si el número de contrato será campo de búsqueda o lista filtrada.
- Confirmar si equipos se cargan dinámicamente por contrato.
- Definir checklist final aprobado por bodega.
- Definir reglas para corrección de registros enviados.
