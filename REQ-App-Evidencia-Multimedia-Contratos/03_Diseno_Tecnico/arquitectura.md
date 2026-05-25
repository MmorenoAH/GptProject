# Arquitectura propuesta

## Vista general
La solución funcionará como una capa operativa de captura y consulta de evidencia, sin reemplazar al ERP.

```text
Usuario de bodega
    ↓
Zoho Forms
    ↓
Zoho CRM / registros relacionados
    ↓
Google Drive para multimedia
    ↓
Consulta por Cartera y Cobro desde Zoho
```

## Sistemas involucrados
- ERP: sistema principal de contratos y movimientos.
- Firebird: base de datos del ERP.
- Zoho CRM: entorno de consulta y relación con datos sincronizados.
- Zoho Forms: captura móvil de checklist y evidencia.
- Google Drive: almacenamiento de archivos multimedia.

## Principio de diseño
El ERP continúa siendo la fuente principal para contratos y movimientos. Zoho será la capa de captura y consulta de evidencia multimedia.

## Punto crítico de validación
Debe confirmarse si los contratos y equipos están disponibles en Zoho CRM como módulos, registros relacionados o campos consultables. Si no están disponibles, se requerirá ajustar o ampliar la integración ERP-Firebird-Zoho CRM.

## No retorno al ERP
En esta fase, la evidencia no regresa al ERP. Esta decisión debe quedar aceptada por las áreas usuarias porque cambia el punto de consulta principal de evidencias futuras.
