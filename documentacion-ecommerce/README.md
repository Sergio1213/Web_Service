# Proyecto Ecommerce Strapi

Este proyecto es un sistema de gestión de contenido (CMS) basado en Strapi, diseñado para impulsar un ecommerce. Utiliza Strapi para gestionar cuatro tipos principales de contenido: categoría, pedido, usuario y producto. A través de estos content types, puedes administrar y organizar eficientemente la información esencial para tu tienda en línea.

## Contenido del Proyecto

El proyecto incluye los siguientes content types:

1. **Categoría:** Define las categorías de productos para organizar y etiquetar los productos de tu tienda.

2. **Pedido:** Permite el seguimiento y la gestión de los pedidos realizados por los clientes.

3. **Usuario:** Gestiona la información de los usuarios, como nombres, direcciones y datos de contacto.

4. **Producto:** Contiene detalles sobre los productos disponibles en tu tienda, como nombre, descripción, precio, etc.

## Requisitos

Asegúrate de tener instaladas las siguientes herramientas antes de comenzar:

- [Node.js](https://nodejs.org/) (versión 12 o superior)
- [npm](https://www.npmjs.com/) (viene con Node.js)
- [Strapi CLI](https://docs.strapi.io/dev-docs/installation/cli/)

## Instrucciones de Instalación y Configuración

1. **instalar xampp:**

Instalar Xampp para usar el servicio de Mysql, en este caso sera el sistema de base de datos que utilizaremos, ya que este instalado acceder a la ruta -[localhost/phpmyadmin](http://localhost/phpmyadmin/) para crear una base de datos, y recordar el nombre de esta, en mi caso sera ***ecommerce***

2. **instalar dependencias:**

instalar strapi en una ruta de tu preferencia con este comando en el cmd
```cmd
npx create-strapi-app@latest my-project
```

3. **Configuracion de strapi:**

En la parte de Configurar strapi casi es todo por defecto, aparecera si quieres la instalacion rapida o manual, en este caso sera la manual, la cual tendras que configurear como la siguiente imagen, en mi caso mi bd no tiene password asi que sera sin password y el nombre de la bd cambia

![IMAGEN DE CONSOLA](https://paper-attachments.dropbox.com/s_A5EC549F5DCFE83DF7D2FE709A683DD9CFC47F0DBC97DE20378C66D11C8AF933_1639474293482_image5_99a6d90dd9.png)


4. **Levantar el servidor**

Una vez terminada la configuracion y sin ningun error, se necesita levnatar el servidor con el siguiente comando 
```cmd
npm run develop
```
Si no hubo problemas te enviara a la interfazde resgistro de strapi que se encuentra en el puerto que la configuraste, en mi caso es en el puerto 1338 y la URL es esta http://localhost:1338/admin


![Imagen_inicio_strapi](https://paper-attachments.dropbox.com/s_A5EC549F5DCFE83DF7D2FE709A683DD9CFC47F0DBC97DE20378C66D11C8AF933_1639474895643_step+24.png)

Ya registrandote te aparecera el inicio de strapi y listo

![Alt text](https://paper-attachments.dropbox.com/s_A5EC549F5DCFE83DF7D2FE709A683DD9CFC47F0DBC97DE20378C66D11C8AF933_1639474955567_step+25.png)
