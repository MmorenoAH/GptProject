# Proyecto: Aplicación Multimedia

## Nombre funcional sugerido
Gestión de Evidencias Multimedia por Contrato y Movimiento de Equipo.

## Objetivo
Implementar una solución interna para capturar, almacenar y consultar evidencia multimedia asociada a contratos, equipos y movimientos operativos de entrega, recepción y cambio de equipos.

## Problema
El proceso actual requiere tomar fotografías, llenar checklist manual, guardar archivos en servidor y luego cargar recursos en el comprobante del ERP. Esto genera demasiados pasos manuales, dependencia del acceso al servidor y riesgo de omisión de evidencias.

## Solución seleccionada
Uso de Zoho Forms para captura móvil, Zoho CRM para consulta estructurada y Google Drive para almacenamiento multimedia. Se aprovecha la integración existente entre ERP, Firebird y Zoho CRM.

## Alcance inicial
- Captura de evidencia en entregas.
- Captura de evidencia en recepciones.
- Asociación por número de contrato.
- Asociación por equipo.
- Clasificación por tipo de movimiento.
- Checklist operativo dentro del formulario.
- Consulta de historial desde Zoho.
- Almacenamiento ordenado de multimedia en Google Drive.

## Fuera de alcance inicial
- Retornar evidencia al ERP.
- Gestión de cobros por daños.
- Integración con incidencias CRM.
- Reemplazo del ERP.
- Rediseño completo del proceso contractual.

## Herramientas base
- Zoho Forms.
- Zoho CRM.
- Google Drive.
- ERP con base Firebird.
