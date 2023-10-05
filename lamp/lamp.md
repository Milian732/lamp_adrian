# Tarea 1 - LAMP en Ubuntu

## 1. Servidor Web Apache

Instalar el servicio apache

![texto_alternativo](entorno_web/apache_1.PNG)

Para comprobar que funciona hay que ir al navegador y poner **http://localhost**

![texto_alternativo](entorno_web/apache_2.PNG)

esto mostrará la pagina por defecto de apache

## 2. MySql

Instalar el servicio mysql

![texto_alternativo](entorno_web/mysql_1.PNG)

Luego entramos en mysql como root

![texto_alternativo](entorno_web/mysql_2.PNG)

Ahora crear una base de datos y con una tabla y insertar algunos datos

![texto_alternativo](entorno_web/mysql_3.PNG)

![texto_alternativo](entorno_web/mysql_4.PNG)

![texto_alternativo](entorno_web/mysql_5.PNG)

![texto_alternativo](entorno_web/mysql_6.PNG)

Comprobar que se han insertado datos en la tabla

![texto_alternativo](entorno_web/mysql_7.PNG)

Aqui he creado el nuevo usuario al que le he otorgado todos los privilegios 

![texto_alternativo](entorno_web/mysql_8.PNG)


## 3. Php

Instalar PHP 

![texto_alternativo](entorno_web/php_1.PNG)

Una vez instalado en en la ruta **/var/www/html** creas el archivo **info.php**

![texto_alternativo](entorno_web/php_2.PNG)

Esto mostrará en el navegador lo siguiente poniendo **http://tu_IP/info.php**

![texto_alternativo](entorno_web/php_3.PNG)

Ahora hay que crear otro .php el cual contendrá una conexion a la base de datos y haga una consulta

a mi no me funcionó con localhost en la parte de **$servidor** y tuve que poner la IP **127.0.0.1**

![texto_alternativo](entorno_web/php_4.PNG)

Una vez lo tienes hecho y modificado a tu gusto, vas al navegador y pones **http://localhost/nombre_del_php**

![texto_alternativo](entorno_web/php_5.PNG)

Aqui mostrará la consulta

## 4. Gestor web de Base de datos

### PHPMYADMIN

Instalar phpmyadmin

![texto_alternativo](entorno_web/phpmyadmin_1.PNG)

Al instalar tendremos que comprobar en el fichero **apache2.conf** de la ruta **/etc/apache2** que la siguiente linea existe, sino hay que añadirla

![texto_alternativo](entorno_web/phpmyadmin_2.PNG)

Vamos al navegador y ponemos **http://localhost/phpmyadmin** y te enviará al login de phpmyadmin


![texto_alternativo](entorno_web/phpmyadmin_3.PNG)


### ADMINER

Instalar adminer

![texto_alternativo](entorno_web/adminer_1.PNG)

Creamos un enlace simbolico desde las rutas especificadas en la imagen y reiniciamos servicio

![texto_alternativo](entorno_web/adminer_2.PNG)

Vamos al navegador y ponemos **http://localhost/adminer**, esto llevará a un login y cuando entremos saldrá lo siguiente:

![texto_alternativo](entorno_web/adminer_3.PNG)

## 5. Analizar los logs de Apache

Instalar GoAccess

![texto_alternativo](entorno_web/goaccess_1.PNG)

El siguiente comando lo que hará es entrar al log de apache y darle un formato de fecha para poder entrar

![texto_alternativo](entorno_web/goaccess_3.PNG)

Al ejecutar el comando entrarás en el panel de control de goaccess y podrás ver todos los logs de apache

![texto_alternativo](entorno_web/goaccess_2.PNG)





