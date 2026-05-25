# Plan de actividades del proyecto

## Proyecto
Aplicación Multimedia / Gestión de Evidencias Multimedia por Contrato y Movimiento de Equipo.

## Objetivo del plan
Listar las actividades necesarias de inicio a fin del proyecto, marcando el avance actual y dejando identificada la siguiente actividad operativa.

## Estados utilizados
- Completado: actividad realizada o documentada.
- En curso: actividad iniciada, pero requiere ampliación o validación.
- Pendiente: actividad aún no iniciada.
- Siguiente actividad: próxima acción recomendada.

---

# Matriz de actividades

| No. | Fase | Actividad | Estado | Observaciones |
|---:|---|---|---|---|
| 1 | Inicio | Crear estructura base del proyecto en GitHub | Completado | Carpeta raíz y documentos iniciales creados en el repositorio. |
| 2 | Inicio | Documentar contexto general del proyecto | Completado | Se documentó proceso actual, problema detectado y decisiones de gerencia. |
| 3 | Inicio | Documentar herramientas seleccionadas | Completado | Zoho Forms, Zoho CRM, Google Drive, ERP y Firebird. |
| 4 | Requerimiento | Definir objetivo funcional del proyecto | Completado | Gestión de evidencia multimedia asociada a contratos, equipos y movimientos. |
| 5 | Requerimiento | Definir alcance inicial | Completado | Entregas, recepciones, evidencia, checklist e historial desde Zoho. |
| 6 | Requerimiento | Definir fuera de alcance inicial | Completado | Retorno al ERP, cobros por daños e incidencias CRM quedan fuera de esta fase. |
| 7 | Requerimiento | Identificar actores y roles iniciales | Completado | Super Admin, Bodega y Cartera/Cobro. |
| 8 | Diseño funcional | Documentar flujo futuro de entrega y recepción | Completado | Flujo base documentado para bodega y consulta de cartera. |
| 9 | Diseño funcional | Evaluar formulario único dinámico vs formularios separados | En curso | Se documentó análisis preliminar, pendiente decisión con dueño del proceso. |
| 10 | Diseño funcional | Reunión con dueños o actores del proceso para determinar contenido del formulario | Siguiente actividad | Definir checklist, campos obligatorios, evidencia mínima, firmas y reglas por tipo de movimiento. |
| 11 | Diseño funcional | Definir campos finales del formulario de Fase 1 | Pendiente | Depende de la reunión con dueños del proceso. |
| 12 | Diseño funcional | Definir checklist de entrega | Pendiente | Debe ser validado por Bodega de Alquiler. |
| 13 | Diseño funcional | Definir checklist de recepción | Pendiente | Debe incluir condiciones del equipo, accesorios y observaciones. |
| 14 | Diseño funcional | Definir evidencia multimedia mínima requerida | Pendiente | Cantidad y tipo de fotos o archivos por movimiento. |
| 15 | Diseño funcional | Definir reglas de edición o corrección de registros enviados | Pendiente | Determinar si bodega puede corregir registros y bajo qué autorización. |
| 16 | Diseño técnico | Documentar arquitectura base | Completado | Zoho Forms, Zoho CRM, Google Drive, ERP y Firebird. |
| 17 | Diseño técnico | Documentar estado actual de integración ERP-Firebird-Zoho CRM | Completado | Contratos sincronizados con información básica. |
| 18 | Diseño técnico | Documentar brecha contrato-equipo | Completado | Falta relación estructurada de equipos asociados al contrato en CRM. |
| 19 | Diseño técnico | Definir estrategia de integración por fases | Completado | Fase 1 captura manual, Fase 2 catálogo intermedio, Fase 3 sincronización ampliada. |
| 20 | Diseño técnico | Validar capacidades reales de Zoho Forms con datos de Zoho CRM | Pendiente | Confirmar búsquedas, campos relacionados, reglas condicionales y cargas multimedia. |
| 21 | Diseño técnico | Definir estructura de almacenamiento en Google Drive | Pendiente | Carpeta por contrato, movimiento, equipo o fecha. |
| 22 | Diseño técnico | Definir nomenclatura de archivos multimedia | Pendiente | Recomendado: contrato_equipo_movimiento_fecha_usuario. |
| 23 | Configuración Zoho | Crear formulario inicial de Fase 1 en Zoho Forms | Pendiente | Depende de campos y checklist aprobados. |
| 24 | Configuración Zoho | Configurar campos obligatorios y reglas condicionales | Pendiente | Según diseño final del formulario. |
| 25 | Configuración Zoho | Configurar carga de archivos multimedia | Pendiente | Validar límites y comportamiento móvil. |
| 26 | Configuración Zoho | Configurar integración con Google Drive | Pendiente | Definir ubicación y permisos. |
| 27 | Configuración Zoho | Configurar relación o consulta con módulo de contratos en Zoho CRM | Pendiente | En Fase 1 al menos debe permitir referencia al contrato. |
| 28 | Seguridad | Configurar rol Super Admin | Pendiente | Administración completa. |
| 29 | Seguridad | Configurar rol Bodega | Pendiente | Captura de registros y evidencia. |
| 30 | Seguridad | Configurar rol Cartera/Cobro | Pendiente | Consulta sin edición de evidencia. |
| 31 | Pruebas | Preparar casos de prueba funcionales | En curso | Casos iniciales documentados, pendiente ajuste con formulario final. |
| 32 | Pruebas | Ejecutar prueba de captura de entrega | Pendiente | Requiere formulario configurado. |
| 33 | Pruebas | Ejecutar prueba de captura de recepción | Pendiente | Requiere formulario configurado. |
| 34 | Pruebas | Ejecutar prueba de consulta por cartera | Pendiente | Validar visibilidad y permisos. |
| 35 | Pruebas | Validar almacenamiento de archivos en Drive | Pendiente | Confirmar ruta, permisos y nomenclatura. |
| 36 | Pruebas | Validar captura desde dispositivo móvil | Pendiente | Prueba clave para usuario de bodega. |
| 37 | Pruebas | Documentar incidencias y ajustes | Pendiente | Crear registro de hallazgos. |
| 38 | Implementación | Preparar plan de implementación piloto | Pendiente | Definir usuarios, contratos de prueba y fechas. |
| 39 | Implementación | Capacitar a usuarios de bodega | Pendiente | Uso del formulario y criterios de evidencia. |
| 40 | Implementación | Capacitar a usuarios de cartera | Pendiente | Consulta de historial y restricciones. |
| 41 | Implementación | Ejecutar piloto controlado | Pendiente | Validar operación real en Fase 1. |
| 42 | Implementación | Revisar resultados del piloto | Pendiente | Medir errores, tiempos y adopción. |
| 43 | Implementación | Ajustar formulario y reglas según piloto | Pendiente | Correcciones antes de producción. |
| 44 | Producción | Preparar salida a producción de Fase 1 | Pendiente | Usar checklist de salida a producción. |
| 45 | Producción | Activar solución para operación formal | Pendiente | Comunicar punto oficial de captura y consulta. |
| 46 | Postproducción | Monitorear registros y errores de captura | Pendiente | Revisión inicial diaria o semanal. |
| 47 | Mejora | Diseñar catálogo intermedio de equipos por contrato | Pendiente | Fase 2. |
| 48 | Mejora | Ejecutar pruebas con catálogo intermedio | Pendiente | Reducir captura manual. |
| 49 | Mejora | Evaluar ampliación de sincronización hacia Zoho CRM | Pendiente | Fase 3. |
| 50 | Cierre | Generar documentación final funcional y técnica | Pendiente | Manuales, ficha técnica y ficha de mantenimiento. |

---

# Próxima actividad inmediata

## Reunión con dueños o actores del proceso para determinar contenido del formulario

### Objetivo de la reunión
Definir el contenido real del formulario que utilizará Bodega de Alquiler para registrar entregas y recepciones.

### Participantes sugeridos
- Dueño del proceso de Bodega de Alquiler.
- Usuario operativo de bodega.
- Representante de Cartera y Cobro.
- TI / Innovación.
- Proveedor o responsable de Zoho, si aplica.

### Temas a definir
- Si se usará un solo formulario o formularios separados.
- Campos obligatorios.
- Checklist de entrega.
- Checklist de recepción.
- Evidencia mínima requerida.
- Reglas para observaciones.
- Si se requiere firma o aceptación.
- Quién puede consultar registros.
- Quién puede corregir registros enviados.
- Qué datos se consultarán desde CRM y qué datos se capturarán manualmente en Fase 1.

### Resultado esperado
Formulario definido y aprobado para construir la primera versión funcional en Zoho Forms.
