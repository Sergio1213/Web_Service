# Configuracion de Endpoints

No olvidemos primero levantar el servidor con el siguiente comando, en la ruta de la carpeta donde se instalo el strapi
**Levantar el servidor**
```cmd
npm run develop
```
Par la configuracion de endpoint primero debes de crear los collection types que aparecen de Content type builder este lado de la interfaz, y poner crear new collection type para crear uno nuevo

![Alt text](https://github.com/Sergio1213/Web_Service/blob/main/documentacion-ecommerce/images/image1.png)

ahi configurar el nombre de tu api y los atributos que necesites 

![Alt text](https://github.com/Sergio1213/Web_Service/blob/main/documentacion-ecommerce/images/image2.png)

![Alt text](https://github.com/Sergio1213/Web_Service/blob/main/documentacion-ecommerce/images/image3.png)


![Alt text](https://github.com/Sergio1213/Web_Service/blob/main/documentacion-ecommerce/images/image4.png)


![Alt text](https://github.com/Sergio1213/Web_Service/blob/main/documentacion-ecommerce/images/image5.png)


una vez creada tienes que dar permiso de quien quieres que acceda, si quieres que sea publico o alguien autentificado, para eso vaz a la parte de settings, y en **USERS & PERMISSIONS PLUGIN** te vaz a roles, ahi seleccionas publico y te apareceran todos los collections types creados, seleccionas uno, mi caso es categoria y le doy el permiso de find

en la parte derecha aparece la ruta de la api y listo

En este caso la ruta es ***/api/categorias***, donde tienen que agregar el localhost y el puerto que en este caso quedaria asi ***"http://localhost:1338/api/categorias"***

y hace eso exactamente con todos los collections types que requieras

![Alt text](https://github.com/Sergio1213/Web_Service/blob/main/documentacion-ecommerce/images/image6.png)

![Alt text](https://github.com/Sergio1213/Web_Service/blob/main/documentacion-ecommerce/images/image7.png)

![Alt text](https://github.com/Sergio1213/Web_Service/blob/main/documentacion-ecommerce/images/image8.png)

En este caso estos serian la configuracion de mis endpoints 

Categoria

![Alt text](https://github.com/Sergio1213/Web_Service/blob/main/documentacion-ecommerce/images/imagen_2023-12-13_221823583.png)

![Alt text](https://github.com/Sergio1213/Web_Service/blob/main/documentacion-ecommerce/images/imagen_2023-12-13_222951199.png)

Pedido

![Alt text](https://github.com/Sergio1213/Web_Service/blob/main/documentacion-ecommerce/images/imagen_2023-12-13_221840672.png)

![Alt text](https://github.com/Sergio1213/Web_Service/blob/main/documentacion-ecommerce/images/imagen_2023-12-13_223003258.png)

Producto

![Alt text](https://github.com/Sergio1213/Web_Service/blob/main/documentacion-ecommerce/images/imagen_2023-12-13_221853018.png)

![Alt text](https://github.com/Sergio1213/Web_Service/blob/main/documentacion-ecommerce/images/imagen_2023-12-13_223019182.png)

Users

![Alt text](https://github.com/Sergio1213/Web_Service/blob/main/documentacion-ecommerce/images/imagen_2023-12-13_221904381.png)

![Alt text](https://github.com/Sergio1213/Web_Service/blob/main/documentacion-ecommerce/images/imagen_2023-12-13_223037529.png)


Si ponemos en el navegador la ruta de categorias con este url nos daria las categoria existentes http://localhost:1338/api/categorias

![alt img](https://github.com/Sergio1213/Web_Service/blob/main/documentacion-ecommerce/images/imagen_2023-12-13_222809616.png)

que podemos ver que si funcionan correctamente 

