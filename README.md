# carlosmayorga
Desarrollar el Ejercicio de Clase

 ![image](https://github.com/user-attachments/assets/ae007692-d639-488e-ac5d-b270d1f4798d)


Se requiere Docker para ejecutar los servicios dentro de los contenedores. Docker se puede instalar ejecutando los siguientes comandos (tomados de la guía de instalación de Docker Engine ):

 

Configurar el repositorio de Docker¶
 
 
 
 
Instalar paquetes Docker de Ubuntu
 
 
 
 
Configuración 
Para permitir que el usuario actual ejecute Docker y, por lo tanto, inicie los contenedores, se lo debe agregar al grupo de usuarios de Docker . Para que el cambio de grupo sea efectivo, cierre la sesión y vuelva a iniciarla o use su .
Agregue el usuario actual al grupo de Docker y aplique los cambios del grupo para el entorno de shell actual¶
 
 
Para descargar el archivo docker compose de Greenbone Community Edition, se debe crear un directorio de destino.
Crear directorio de descarga
 
Archivo Docker Compose 
Para ejecutar Greenbone Community Edition con contenedores, se debe utilizar el siguiente archivo de composición:
Archivo Docker Compose
 
Bajo Linux
 
 
Iniciando los contenedores comunitarios de Greenbone 
Usando el archivo docker compose, se pueden descargar ( extraer ) las imágenes del contenedor y se pueden iniciar los contenedores en segundo plano.
Descarga de los contenedores de la comunidad Greenbone
 
 
Puesta en marcha de los contenedores comunitarios Greenbone
docker compose -f $DOWNLOAD_DIR/docker-compose.yml -p greenbone-community-edition up -d
 
Para obtener un flujo continuo de la salida del registro de todos los servicios, ejecute el siguiente comando:
Mostrar mensajes de registro de todos los servicios de los contenedores en ejecución¶
 
 
 
 
Configurar un usuario administrador 
Advertencia
De forma predeterminada, se crea un usuario admin con la contraseña admin . Esto no es seguro y se recomienda encarecidamente establecer una nueva contraseña.
Para actualizar el usuario administrador con una contraseña de su elección en lugar de la contraseña generada, se puede utilizar el siguiente comando:
Actualizar contraseña del usuario administrador
 

Iniciando la Gestión de Vulnerabilidades 
Una vez iniciados los servicios y cargados todos los datos de las fuentes , se puede abrir la interfaz web de Greenbone Security Assistant (GSA) en el navegador.
Cómo abrir Greenbone Security Assistant en el navegador¶
 
 

 
Configuración y secuencia de comandos de inicio 
Nota
Recuerde seguir primero las instrucciones descritas en los Requisitos previos .
Como solución rápida, proporcionamos todos los comandos anteriores en un solo script. Este script se puede descargar directamente con el siguiente comando:
Descargar el script de instalación e inicio al directorio de trabajo actual¶
 
Para ejecutar el script se debe ejecutar el siguiente comando
Ejecutar la configuración y comenzar el script
 
 
 
 
 
 
 
 
 
 
 
 

