---
sidebar_position: 3
---

# Creacion de Campañas

## Creación de nueva campaña

Para crear una nueva campaña, haz clic en el botón **"+ Campaña"**. Se abrirá un formulario modal con los siguientes campos:

### Campos principales:
- **Nombre de la campaña:** Identificador único de la campaña
- **Canal:** Selección del canal de comunicación (WhatsApp, Facebook, etc.)
- **Caller ID:** Número de teléfono asociado
- **Template Inicial:** Plantilla de mensaje inicial
- **Template de Quality:** Plantilla para control de calidad
- **Template de Reasignación:** Plantilla para reasignación de leads
- **Template de Asesor:** Plantilla para asesores
- **Template de Recordatorio:** Plantilla para recordatorios
- **Horario de llamadas:** Configuración de horarios permitidos
- **Twilio Number:** Configuración del número de Twilio
- **Perfil WAB:** Perfil de WhatsApp Business
- **Bot Lead:** Configuración del bot para leads
- **Bot Seller:** Configuración del bot para vendedores

![Crear campaña](https://xperience-docs-prod.s3.us-east-2.amazonaws.com/Manuales_devs/documentation/campaigns/campaigns-form.png)

### Selección de templates

Al configurar una campaña, puedes seleccionar entre diferentes templates predefinidos:

![Selección de templates](https://xperience-docs-prod.s3.us-east-2.amazonaws.com/Manuales_devs/documentation/campaigns/campaigns-form-templates.png)

---

## Configuración de templates

### Datos de template

Los templates permiten personalizar los mensajes utilizando **KeyWords** dinámicos:

**Keywords disponibles:**
- `%leadId:` Agrega el ID del lead
- `%leadName:` Agrega el nombre del lead
- `%leadEmail:` Agrega el email del lead
- `%leadPhone:` Agrega el teléfono del lead
- `%productName:` Agrega el nombre del producto
- `%sellerName:` Agrega el nombre del asesor
- `%channelName:` Agrega el nombre del canal
- `%campaignName:` Agrega el nombre de campaña
- `%typeChannelName:` Agrega el medio

### Configuración de valores

En la sección **"Rellenar valores"** puedes asignar valores específicos a cada keyword:
- **{1}:** `%leadName`
- **{2}:** `%productName`

El sistema incluye un **Preview** que muestra cómo se verá el mensaje final con los datos dinámicos.

![Configuración de template](https://xperience-docs-prod.s3.us-east-2.amazonaws.com/Manuales_devs/documentation/campaigns/campaigns-form-templates-edit.png)

### Confirmación de cambios

Al realizar cambios en un template, el sistema solicitará confirmación:

![Confirmación de salida](https://xperience-docs-prod.s3.us-east-2.amazonaws.com/Manuales_devs/documentation/campaigns/campaigns-form-templates-warning.png)

---