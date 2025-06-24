---
sidebar_position: 1
---

# Introducción

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