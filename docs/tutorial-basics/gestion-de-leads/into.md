---
sidebar_position: 1
---

# Introducción

El módulo de Leads permite gestionar y dar seguimiento a los prospesctos de ventas, desde su captura inicial hasta su calificación y posible conversión en clientes.

![Vista general del módulo de Leads](https://xperience-docs-prod.s3.us-east-2.amazonaws.com/Manuales_devs/documentation/leads/leads-view.png)

## Características Principales

- **Calificación de Leads**: Sistema de puntuación para evaluar la calidad de los prospectos
- **Asignación de Vendedores**: Distribución automática o manual de leads al equipo de ventas
- **Seguimiento de Llamadas**: Registro de interacciones telefónicas
- **Gestión de Spam**: Identificación y manejo de leads no válidos
- **Integración con CRM**: Envío directo de leads calificados al sistema CRM

## Vista Principal de Leads

### Panel de Control

La vista principal muestra:

- **Gráfico de Leads**: Visualización temporal de leads totales vs leads duplicados
- **Filtros**: Por fecha, producto, campaña y usuario
- **Opciones de Exportación**: 
  - Exportación personalizada
  - Exportar todas las páginas
  - Exportar página actual
  - Exportar filas seleccionadas

![Panel de control principal](https://xperience-docs-prod.s3.us-east-2.amazonaws.com/Manuales_devs/documentation/leads/leads-controls.png)

![Panel de control principal](https://xperience-docs-prod.s3.us-east-2.amazonaws.com/Manuales_devs/documentation/leads/leads-exports.png)
s
### Lista de Leads

Cada lead muestra la siguiente información:

| Campo | Descripción |
|-------|-------------|
| **Detalles** | Vissualizar los detalles del lead |
| **ID** | Identificador único del lead |
| **Fecha** | Fecha y hora de creación |
| **Producto/Campaña** | Origen del lead (ej: "Xperience Demo", "Facebook Ads") |
| **Nombre/Correo/Teléfono** | Información de contacto |
| **Vendedor** | Representante asignado |
| **Tipo** | Clasificación del lead |
| **Calificación** | Estado de calificación |
| **iScore** | Puntuación de calidad |
| **Bandeja** | Número de intentos de contacto |
| **Envio CRM** | Botón para enviar a CRM | 


## Calificación de Leads

### Sistema de Puntuación (iScore / Sellser Score)

El sistema utiliza un algoritmo de calificación que asigna puntuaciones basadas en:

- Calidad de la información proporcionada
- Fuente del lead
- Comportamiento del prospecto
- Historial de interacciones
- Si se le da seguimiento al leads

**Rangos de Puntuación:**

- **0-20**: Baja calidad
- **21-40**: Calidad media
- **41-60**: Buena calidad
- **61-80**: Muy buena calidad
- **81-100**: Excelente calidad

![Sistema de puntuación iScore](https://xperience-docs-prod.s3.us-east-2.amazonaws.com/Manuales_devs/documentation/leads/leads-score.png)

### Estados de Calificación

- **Sin Calificar**: Lead recién ingresado

**Nota** las campañas por defecto cuentan con **5** calificaciones por defecto las cuales son: 

- **Alto Interess**
- **Interés Medio** 
- **Interés Bajo**
- **No interesado**
- **No Localizable**

Para más informacion puedes ingresar al siguiente enlace [Campañas - Calificaciones](https://dulcet-rabanadas-f3e5b8.netlify.app/docs/tutorial-basics/campaings/#gesti%C3%B3n-de-calificaciones)


![Estados de calificación de leads](https://xperience-docs-prod.s3.us-east-2.amazonaws.com/Manuales_devs/documentation/leads/leads-qualification.png)


## Asignación de Vendedores

### Seller Score

Sistema de puntuación para vendedores basado en:

- Número de leads asignados
- Tasa de conversión
- Calidad de seguimiento
- Resultados de ventas

![Sistema de puntuación de vendedores](https://xperience-docs-prod.s3.us-east-2.amazonaws.com/Manuales_devs/documentation/leads/leads-seller-score.png)

### Tipos de Asignación

- **Asignación directa**
- **Re-Asignación manual** 
- **Rol de producto**
- **Rol de campaña**
- **Duplicado en producto**
- **Duplicado en campaña**
- **Duplicado en compañía** 
- **Duplicado en marca**

![Tipos de asignación de vendedores](https://xperience-docs-prod.s3.us-east-2.amazonaws.com/Manuales_devs/documentation/leads/leads-assignment-types.png)

## Gestión de Spam

### Identificación de Spam

El sistema cuenta con una sección dedicada para manejar leads marcados como spam, permitiendo:

- Revisión manual de leads sospechosos
- Configuración de filtros automáticos
- Gestión de leads incorrectamente marcados

![Gestión de spam](https://xperience-docs-prod.s3.us-east-2.amazonaws.com/Manuales_devs/documentation/leads/leads-spam-management.png)

### Estado de Spam

- **Total de leads en spam**: Contador actual
- **Acciones**: Revisión y reclasificación de leads

![Estado de leads en spam](https://xperience-docs-prod.s3.us-east-2.amazonaws.com/Manuales_devs/documentation/leads/leads-spam-status.png)

## Integración con CRM

### Envío a CRM

Los leads calificados pueden ser enviados al CRM con un solo clic:

- **Enviar a CRM**: Botón de acción rápida
- **Sincronización automática**: Actualización en tiempo real
- **Historial de envíos**: Registro de leads transferidos

![Integración con CRM](https://xperience-docs-prod.s3.us-east-2.amazonaws.com/Manuales_devs/documentation/leads/leads-crm-integration.png)

### Datos Transferidos

- Información completa del lead
- Historial de interacciones
- Puntuación de calificación
- Notas y comentarios

![Datos transferidos al CRM](https://xperience-docs-prod.s3.us-east-2.amazonaws.com/Manuales_devs/documentation/leads/leads-crm-data-transfer.png)

## Reportes y Analytics

### Métricas Principales

- **Leads Totales**: Número total de leads recibidos
- **Leads Duplicados**: Cantidad de leads repetidos
- **Tasa de Conversión**: Porcentaje de leads convertidos
- **Rendimiento por Vendedor**: Estadísticas individuales

![Métricas principales](https://xperience-docs-prod.s3.us-east-2.amazonaws.com/Manuales_devs/documentation/leads/leads-main-metrics.png)

### Visualizaciones

- Gráficos de barras temporales
- Tendencias de generación de leads
- Distribución por fuente
- Análisis de calidad

![Visualizaciones y gráficos](https://xperience-docs-prod.s3.us-east-2.amazonaws.com/Manuales_devs/documentation/leads/leads-visualizations.png)

## Mejores Prácticas

### Para Administradores

1. **Monitoreo Regular**: Revisar diariamente los nuevos leads
2. **Calificación Rápida**: Procesar leads dentro de las primeras 24 horas
3. **Distribución Equitativa**: Balancear la carga entre vendedores
4. **Limpieza de Datos**: Eliminar regularmente leads spam

![Mejores prácticas para administradores](https://xperience-docs-prod.s3.us-east-2.amazonaws.com/Manuales_devs/documentation/leads/leads-admin-best-practices.png)

### Para Vendedores

1. **Seguimiento Oportuno**: Contactar leads en las primeras 2 horas
2. **Registro Completo**: Documentar todas las interacciones
3. **Actualización de Estado**: Mantener actualizada la calificación
4. **Notas Detalladas**: Incluir información relevante de cada contacto

![Mejores prácticas para vendedores](https://xperience-docs-prod.s3.us-east-2.amazonaws.com/Manuales_devs/documentation/leads/leads-sales-best-practices.png)

## Configuración del Sistema

### Parámetros Configurables

- **Algoritmo de Puntuación**: Ajuste de criterios de iScore
- **Reglas de Asignación**: Configuración de distribución automática
- **Filtros de Spam**: Criterios de identificación
- **Campos Personalizados**: Adaptación a necesidades específicas

![Configuración del sistema](https://xperience-docs-prod.s3.us-east-2.amazonaws.com/Manuales_devs/documentation/leads/leads-system-config.png)

### Integraciones

- **Facebook Ads**: Captura automática de leads
- **Formularios Web**: Integración con sitios web
- **APIs**: Conexión con sistemas externos
- **Webhooks**: Notificaciones automáticas

![Integraciones disponibles](https://xperience-docs-prod.s3.us-east-2.amazonaws.com/Manuales_devs/documentation/leads/leads-integrations.png)