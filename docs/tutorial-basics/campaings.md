---
sidebar_position: 5
---

# Gestión de Campañas

En Xperience, los **Desarrollos** pueden tener asociadas diferentes campañas para la gestión de leads y la automatización de procesos comerciales. A continuación, se describe el funcionamiento de la tabla de campañas y las acciones disponibles.

---

## Vista general de campañas

Dentro de cada desarrollo, encontrarás una sección de **Campañas**. Aquí se listan todas las campañas asociadas al desarrollo, mostrando información relevante como el nombre, canal, estado y tipo.

La interfaz principal muestra:
- **Leads generados:** Contador total de leads obtenidos
- **Campañas creadas:** Número total de campañas configuradas
- **Filtros de estado:** Todos, Activos, Inactivos
- **Tabla de campañas** con columnas para ID, Estado, Nombre/Canal, y Tipo

![Vista general de campañas](https://xperience-docs-prod.s3.us-east-2.amazonaws.com/Manuales_devs/documentation/campaigns/campaigns-view.png)

---

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

## Acciones disponibles en la tabla de campañas

En la columna de **Acciones** de la tabla de campañas, encontrarás los siguientes iconos:

- ⭐ **Estrellita:** Permite acceder y gestionar las **calificaciones** asociadas a la campaña
- ✏️ **Pluma:** Permite **editar** la configuración y detalles de la campaña seleccionada
- 🔄 **Switch (interruptor):** Permite **activar o desactivar** la campaña
  - Si la campaña está **apagada**, **no podrá recibir leads** hasta que se vuelva a activar

---

## Edición de producto

Desde la vista de campañas también puedes acceder a la edición del producto asociado, donde puedes configurar:

### Información básica:
- **Nombre del producto**
- **Tipo de producto** (Casas y Departamentos, etc.)

### Dirección:
- **País:** Selección del país
- **Estado:** Ingreso del estado
- **Ciudad:** Especificación de la ciudad
- **Delegación o Municipio**

### Enlaces y configuración:
- **Dirección Google Maps**
- **Dirección Waze**
- **Dirección Recorrido Virtual**
- **Dirección Web**
- **CRM:** Configuración del sistema CRM
- **WAB'S:** Configuración de WhatsApp Business
- **Precio:** Configuración de precios
- **Aviso de privacidad:** Enlaces legales

![Edición de producto](https://xperience-docs-prod.s3.us-east-2.amazonaws.com/Manuales_devs/documentation/campaigns/campaigns-product-form.png)

---

## Gestión de archivos

Cada campaña puede tener archivos asociados organizados en tres categorías:

### Tipos de archivos disponibles:
1. **Imagen Producto:** Imágenes del desarrollo/producto
2. **WhatsApp Imagen:** Imágenes específicas para WhatsApp
3. **Brochure:** Documentos PDF informativos

![Archivos de campaña](https://xperience-docs-prod.s3.us-east-2.amazonaws.com/Manuales_devs/documentation/campaigns/campaigns-fiels.png)

Para cada tipo de archivo puedes:
- Seleccionar archivos existentes
- Subir nuevos archivos usando el botón **"Subir Archivo"**

---

## Panel de configuración de campaña

El panel lateral derecho permite configurar aspectos específicos de cada campaña:

### Información general:
- **Nombre:** Identificador de la campaña
- **Canal:** Medio de comunicación (Ferias, etc.)
- **Fecha Alta:** Fecha de creación
- **ID y Token:** Identificadores únicos
- **Caller ID:** Número de contacto
- **CRM ID:** Identificador en el CRM
- **CRM ID Canal:** Canal específico del CRM

### Configuración técnica:
- **Api SetUp:** Configuración de APIs
- **Twilio Number:** Número de Twilio asociado
- **Horario de llamadas:** Horarios permitidos para contacto
- **Perfil WAB:** Perfil de WhatsApp Business
- **Mensaje detonante:** Mensaje inicial automático
- **Bot Lead y Bot Seller:** Configuración de bots

### Templates:
- **Template Inicial**: Es el que le llega al lead por primera vez.
- **Template Quality**: Es el que le llega después de 12 horas para que pueda calificar la atención del cliente.
- **Template Reasignación**: Le llega al seller para informarle que se le reasignó un lead.
- **Template Asesor**: Es para notificar al asesor que le llegó un nuevo lead.
- **Template Recordatorio**: Cuando el asesor crea un recordatorio en una fecha específica, Xperience le notifica mediante un mensaje de WhatsApp.

## Duplicidad:

Existen diferentes tipos de duplicidad para la gestión de leads, siendo la configuración por defecto "Por Producto". Si necesitas alguna otra que se ajuste mejor a tus necesidades, a continuación se detallan las opciones disponibles:

### Tipos de Duplicidad:

* **Bloqueada:**
    Cuando un lead duplicado intenta solicitar información o registrarse, si previamente ya había interactuado con otra campaña o producto de la misma empresa, el registro existente "SE ACTUALIZARÁ". No se creará un registro múltiple y se asignará un nuevo asesor solo si la fecha de su último ingreso es superior a 30 días (este período es configurable).

* **Producto:**
    Si un lead duplicado intenta solicitar información o registrarse y ya había interactuado con el mismo producto, "SE CREARÁ" un nuevo registro. Se le asignará un nuevo asesor solo si la fecha de su último ingreso es superior a 30 días (este período es configurable).

* **Campaña:**
    En caso de que un lead duplicado intente solicitar información o registrarse y ya había interactuado con la misma campaña, "SE CREARÁ" un nuevo registro. Se asignará un nuevo asesor solo si la fecha de su último ingreso es superior a 30 días (este período es configurable).

* **Compañía:**
    Cuando un lead duplicado intenta solicitar información o registrarse, y ya había interactuado con alguna otra campaña o producto de la empresa, "SE CREARÁ" un nuevo registro. Se asignará un nuevo asesor solo si la fecha de su último ingreso es superior a 30 días (este período es configurable).

* **Marca:**
    La duplicidad por marca gestiona leads dentro de un conjunto definido de productos asociados a una misma marca. A diferencia de las duplicidades por producto o por compañía, esta opción restringe la búsqueda de leads existentes a los productos pertenecientes exclusivamente a la marca en cuestión.

    * **Funcionamiento:** Si un lead ingresa y ya existe un registro previo en cualquiera de los productos dentro de la misma marca, el sistema lo identifica como duplicado y la asignación del lead se mantiene dentro de la marca.

    * **Ejemplo:**
        Considere las marcas "Sabrosa" (Productos 1, 2, 3) y "Patito" (Productos A, B, C).
        1.  Si un lead solicita información del "Producto 3" (Marca Sabrosa) habiendo solicitado previamente del "Producto B" (Marca Patito), para la "Marca Sabrosa" se considera un lead nuevo, ya que la interacción anterior fue de una marca diferente.
        2.  Si el mismo lead solicita posteriormente información del "Producto 1" (Marca Sabrosa), el sistema detecta un registro previo dentro de "Marca Sabrosa". Se gestiona como duplicado y se mantiene la asignación anterior dentro de la marca (o se asigna un nuevo asesor si excede el período configurable de asignación).

### Notificaciones:

Existen cuatro tipos de notificaciones que se pueden configurar, permitiendo automatizar la comunicación con los leads y los asesores:

* **Correo a Lead:** Envío de un correo electrónico inicial al lead en el momento en que solicita información.
* **Correo al Vendedor:** Notificación por correo electrónico al asesor asignado cuando un nuevo lead ha solicitado información.
* **WhatsApp al Vendedor:** Envío de un mensaje de WhatsApp al asesor asignado para notificarle sobre un nuevo lead.
* **WhatsApp al Lead:** Envío de un mensaje de WhatsApp al lead como parte de la comunicación inicial tras su solicitud de información.

### Quality:

Esta opción permite activar o desactivar el envío de un mensaje de seguimiento al lead después de 12 horas de su contacto inicial, con el objetivo de retomar la comunicación.

### Llamada:

Esta funcionalidad se puede activar o desactivar. Al activarla, en el momento en que un lead solicita información, se detona una llamada automática que lo enlaza directamente con el asesor asignado.

### Creación de Leads Manuales:

Por defecto, esta opción se encuentra desactivada. Al activarla, se permite la creación directa de leads desde la sección de leads en Xperience, sin que provengan de una solicitud de información.

### Días para Detectar Duplicidad:

Este campo establece el período de tiempo en días para la detección de leads duplicados. Por defecto, está configurado en 30 días, lo que significa que un lead será considerado duplicado si vuelve a solicitar información dentro de ese rango de días. Este valor es configurable.


![Panel de campaña](https://xperience-docs-prod.s3.us-east-2.amazonaws.com/Manuales_devs/documentation/campaigns/campaigns-details-form.png)

---

## Asignación de asesores

En la sección **"Asignación por Campaña"** puedes gestionar qué asesores tendrán acceso a los leads de cada campaña:

### Opciones de asignación:
- **Campaña:** Asignación general por campaña
- **Producto:** Asignación específica por producto

### Lista de asesores disponibles:

Cada asesor puede ser activado o desactivado mediante el switch correspondiente.

![Asignación de asesores](https://xperience-docs-prod.s3.us-east-2.amazonaws.com/Manuales_devs/documentation/campaigns/campaigns-details-assigments.png)

---

## Gestión de calificaciones

Al hacer clic en la estrella (⭐) de una campaña, accedes al sistema de **Calificaciones**, donde puedes:

### Agregar nueva calificación:
- **Nombre:** Descripción de la calificación
- **Valor:** Valor numérico asociado

### Calificaciones predefinidas:
- **Se le hace muy caro:** Valor 6
- **Alto Interés:** Valor 5
- **Interés Medio:** Valor 4
- **Interés Bajo:** Valor 3
- **No Interesado:** Valor 2
- **No le gustó la zona:** Valor 1

Cada calificación puede ser **editada** individualmente según las necesidades de la campaña.

![Gestión de calificaciones](https://xperience-docs-prod.s3.us-east-2.amazonaws.com/Manuales_devs/documentation/campaigns/campaigns-grades.png)

---

## Consideraciones importantes

> **Nota:** Es importante mantener activas solo las campañas que estén en operación para asegurar la correcta recepción de leads y evitar confusiones en la gestión comercial.

### Mejores prácticas:
1. **Configura templates personalizados** para cada tipo de comunicación
2. **Asigna asesores específicos** según la naturaleza de cada campaña
3. **Mantén actualizadas las calificaciones** según los criterios comerciales
4. **Revisa regularmente el estado** de las campañas activas
5. **Utiliza las keywords dinámicas** para personalizar la comunicación

### Flujo de trabajo recomendado:
1. Crear la campaña con la configuración básica
2. Configurar templates personalizados
3. Asignar asesores correspondientes
4. Definir calificaciones específicas
5. Subir archivos necesarios (imágenes, brochures)
6. Activar la campaña
7. Monitorear el rendimiento regularmente