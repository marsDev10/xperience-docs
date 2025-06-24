---
sidebar_position: 2
---

# Admistración

Observa el comportamiento del prospecto.

![Detalles de lead](https://xperience-docs-prod.s3.us-east-2.amazonaws.com/Manuales_devs/documentation/leads/leads-view-details.png)

### Navegación Principal

El sistema cuenta con 6 secciones principales:

- **Llamadas**: Gestión de llamadas telefónicas
- **Emails**: Seguimiento de comunicaciones por correo electrónico
- **Calificaciones**: Sistema de puntuación y calificación de leads
- **WhatsApp**: Interacciones a través de mensajería instantánea
- **Historial**: Registro completo de actividades
- **CRM**: Integración con sistemas externos

## **Sección de Llamadas**

Xperience realiza un resgistro de las llamadas guardando la grabación y la duración de dicha llamada

![Detalles - Llamadas](https://xperience-docs-prod.s3.us-east-2.amazonaws.com/Manuales_devs/documentation/leads/leads-view-details.png)

## **Sección de Emails**

El sistema incluye una plantilla por defecto que sera enviada con la infomacion del producto:

- **Propósito**: Email de bienvenida para nuevos leads
- **Estado**: Seguimiento automático de apertura
- **Funcionalidades**:
  - Historial de clicks en enlaces
  - Tracking de interacciones con URLs específicas
  - Registro de descargas de documentos



### Seguimiento de Interacciones

Cada email enviado incluye:

- Fecha y hora de envío
- Estado de apertura
- Links clickeados por el usuario
- Archivos descargados

![Detalles - Emails](https://xperience-docs-prod.s3.us-east-2.amazonaws.com/Manuales_devs/documentation/leads/leads-view-details.png)

## **Sección Calificaciones**

### Sistema de Puntuación

El sistema asigna valores numéricos a cada lead:

- **ID único**: Identificador del lead (ej: 98509)
- **Valor**: Puntuación asignada (ej: 8 puntos)
- **Tipo**: Clasificación del lead (ej: "Cita Exitosa")
- **Comentarios**: Observaciones del asesor

### Proceso de Calificación

1. El sistema evalúa automáticamente las interacciones
2. Asigna una puntuación basada en el comportamiento
3. El asesor puede agregar comentarios adicionales
4. Se registra la fecha y hora de la calificación

![Detalles - Calificaciones](https://xperience-docs-prod.s3.us-east-2.amazonaws.com/Manuales_devs/documentation/leads/leads-view-details.png)

## **Sección WhatsApp**

### Automatización de Mensajes

El sistema incluye un bot automatizado que:

#### Respuesta Inicial
- Saluda al lead por su nombre
- Confirma la recepción de la solicitud
- Asigna un asesor específico
- Proporciona opciones de contacto

#### Información del Lead
El bot comparte automáticamente:
- ID del contacto
- Nombre completo
- Correo electrónico
- Número de teléfono

### Tiempos de Respuesta

El sistema monitorea:
- **Tiempo del vendedor**: Tiempo en responder al lead
- **Tiempo del lead**: Tiempo del lead en responder
- **Primera interacción**: Registro de la primera comunicación

### Métricas de Interacción

- Tiempo promedio de respuesta
- Tasa de interacción por primera vez
- Seguimiento de encuestas enviadas

![Detalles - Whatsapp](https://xperience-docs-prod.s3.us-east-2.amazonaws.com/Manuales_devs/documentation/leads/leads-view-details.png)

## **Sección Historial**

### Registro de Actividades

Todas las modificaciones quedan registradas:

- **Usuario responsable**: Quién realizó la acción
- **Acción realizada**: Tipo de modificación
- **Asesor asignado**: Registro del asesor responsable
- **Nombre del lead**: Identificación completa
- **Timestamp**: Fecha y hora exacta

### Trazabilidad Completa

El historial permite:
- Auditoría de cambios
- Seguimiento de responsabilidades
- Análisis de performance por asesor
- Registro completo de la gestión del lead

![Detalles - Historial](https://xperience-docs-prod.s3.us-east-2.amazonaws.com/Manuales_devs/documentation/leads/leads-view-details.png)

## **Sección CRM**

### Integración Externa

El sistema se integra con CRMs externos:

#### Envío de Datos
- **Fecha de envío**: Timestamp de la transmisión
- **Respuesta del CRM**: Confirmación de recepción
- **Status de respuesta**: Código de estado (ej: 200 = exitoso)

#### Validación de Datos
- Verificación de existencia en base de datos
- Proceso de revisión cuando es necesario
- Sincronización automática de información

### Funcionalidades Adicionales

- **Ver Datos Enviados**: Revisión de información transmitida
- **Status de Integración**: Monitor del estado de conexión
- **Logs de Sincronización**: Registro detallado de transferencias

## Flujo de Trabajo Típico

1. **Generación del Lead**: El lead ingresa al sistema
2. **Asignación Automática**: Se asigna un asesor
3. **Contacto Inicial**: Bot de WhatsApp realiza primer contacto
4. **Seguimiento**: Asesor continúa la comunicación
5. **Calificación**: Se evalúa y puntúa el lead
6. **Integración CRM**: Datos se sincronizan con sistema externo
7. **Historial**: Todas las acciones quedan registradas

## Mejores Prácticas

### Para Asesores
- Responder dentro de los primeros minutos
- Utilizar las plantillas de email disponibles
- Mantener actualizada la información del lead
- Revisar el historial antes de cada interacción

### Para Administradores
- Monitorear tiempos de respuesta
- Revisar calificaciones regularmente
- Verificar sincronización con CRM externo
- Analizar métricas de conversión

## Soporte Técnico

Para problemas técnicos o dudas sobre el sistema:
- Revisar los logs en la sección CRM
- Verificar el status de respuesta de integraciones
- Consultar el historial para trazabilidad de errores
