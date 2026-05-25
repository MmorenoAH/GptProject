# Actores y roles

## Roles iniciales

### Super Admin
Responsable de administración general de la solución.

Permisos sugeridos:
- Crear y modificar formularios.
- Administrar integraciones.
- Ver todos los registros.
- Gestionar usuarios y permisos.
- Revisar estructura de almacenamiento.
- Auditar registros.

### Bodega de Alquiler
Usuario operativo responsable de capturar evidencia.

Permisos sugeridos:
- Crear registros de entrega, recepción o cambio.
- Adjuntar evidencia multimedia.
- Completar checklist.
- Consultar registros propios o registros recientes si el proceso lo requiere.
- No modificar registros históricos validados, salvo regla explícita.

### Cartera y Cobro
Usuario consultor de evidencia.

Permisos sugeridos:
- Consultar historial por contrato.
- Consultar historial por equipo.
- Ver checklist y evidencia multimedia.
- No editar evidencia.
- No eliminar archivos.

## Recomendación de control
Cartera debe tener permisos de consulta y no de edición para preservar trazabilidad y evitar alteraciones posteriores de evidencia.
