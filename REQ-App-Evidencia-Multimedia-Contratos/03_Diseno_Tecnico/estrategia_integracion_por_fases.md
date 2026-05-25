# Estrategia de integración por fases

## Objetivo
Definir una estrategia progresiva para implementar la solución sin detener el avance del desarrollo, manteniendo como meta final una integración más robusta entre ERP y Zoho CRM.

## Contexto técnico actual
La integración actual entre ERP y Zoho fue realizada por un proveedor de desarrollo. La empresa cuenta con acceso a:

- Códigos de integración en Zoho.
- Swagger del ERP.
- Credenciales de conexión.
- Conexiones nativas configuradas entre ERP y Zoho.

En Zoho se observan conexiones activas relacionadas con:
- Zoho CRM.
- Conexión RTI / ERP.
- Zoho OAuth.

## Decisión de avance
Durante la primera etapa del desarrollo se permitirá la captura manual del equipo dentro del formulario para no retrasar el progreso funcional del proyecto.

Esta decisión no representa el diseño final recomendado, sino una medida temporal para validar el flujo de captura, almacenamiento y consulta de evidencias.

---

# Fase 1: Captura manual controlada

## Objetivo
Construir y validar el flujo funcional mínimo con Zoho Forms, Zoho CRM y Google Drive.

## Características
- Bodega selecciona o ingresa el contrato.
- Bodega ingresa o selecciona manualmente el equipo.
- Se captura checklist.
- Se adjunta evidencia multimedia.
- Se almacena la evidencia en Google Drive.
- Se permite consulta desde Zoho.

## Ventajas
- Permite avanzar sin esperar ajustes de integración.
- Facilita validar la aceptación del usuario.
- Permite probar estructura de formulario, permisos y almacenamiento.

## Riesgos
- Riesgo de errores al ingresar datos del equipo.
- Menor trazabilidad automática.
- Dependencia de disciplina operativa del usuario.

## Controles recomendados
- Usar campos obligatorios.
- Usar listas desplegables cuando sea posible.
- Definir formato estándar para escribir código o identificador de equipo.
- Incluir validación visual o revisión de registros durante piloto.

---

# Fase 2: Catálogo intermedio provisional

## Objetivo
Reducir captura manual mediante un catálogo básico de equipos por contrato, antes de ampliar completamente la sincronización con CRM.

## Características
- Crear una estructura temporal con contrato y equipos asociados.
- Alimentar el catálogo desde una extracción controlada del ERP o carga inicial.
- Permitir que Zoho Forms use esta información para selección más controlada.

## Ventajas
- Mejora la calidad de datos.
- Reduce errores de digitación.
- Permite pruebas en producción con menor riesgo.

## Riesgos
- Requiere mantenimiento temporal.
- Puede quedar desactualizado si no se define frecuencia de actualización.
- No debe convertirse en solución final sin control formal.

---

# Fase 3: Ampliación de sincronización hacia Zoho CRM

## Objetivo
Integrar de forma más robusta la relación contrato-equipo dentro de Zoho CRM.

## Características esperadas
- Sincronizar equipos asociados a cada contrato.
- Permitir consulta dinámica desde Zoho Forms.
- Mantener ERP como fuente principal.
- Mejorar búsqueda histórica por contrato y equipo.

## Resultado esperado
La captura de evidencia debe quedar vinculada a registros estructurados de contrato y equipo, evitando ingreso manual y mejorando la trazabilidad.

---

# Criterio de avance entre fases

## Para pasar de Fase 1 a Fase 2
- Formulario funcional validado por bodega.
- Evidencia guardada correctamente.
- Consulta desde Zoho validada por cartera.
- Checklist operativo aceptado.
- Errores de captura manual identificados.

## Para pasar de Fase 2 a Fase 3
- Solución validada como útil por las áreas usuarias.
- Modelo de datos mínimo confirmado.
- Relación contrato-equipo validada en ERP.
- Alcance técnico aprobado para ampliar integración.

## Nota de control
La captura manual no debe considerarse solución definitiva. Debe quedar registrada como fase de arranque para acelerar validación funcional.
