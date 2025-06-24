---
sidebar_position: 2
---

# Admistración

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