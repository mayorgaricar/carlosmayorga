# carlosmayorga
Desarrollar el Ejercicio de Clase

 ![image](https://github.com/user-attachments/assets/ae007692-d639-488e-ac5d-b270d1f4798d)


Se requiere Docker para ejecutar los servicios dentro de los contenedores. Docker se puede instalar ejecutando los siguientes comandos (tomados de la guía de instalación de Docker Engine ):

 ![image](https://github.com/user-attachments/assets/43cd8cdb-8932-456c-8c83-fd171497eee7)


Configurar el repositorio de Docker¶
 
 ![image](https://github.com/user-attachments/assets/72a0a534-bc77-42a2-917b-e7ef46c1fad0)

 
 
Instalar paquetes Docker de Ubuntu
 
 ![image](https://github.com/user-attachments/assets/a4915b57-76bf-4e84-92b8-47f3a6613a96)

 
 
Configuración 
Para permitir que el usuario actual ejecute Docker y, por lo tanto, inicie los contenedores, se lo debe agregar al grupo de usuarios de Docker . Para que el cambio de grupo sea efectivo, cierre la sesión y vuelva a iniciarla o use su .
Agregue el usuario actual al grupo de Docker y aplique los cambios del grupo para el entorno de shell actual¶
 ![image](https://github.com/user-attachments/assets/5110925a-6685-4eb8-9629-5ab84fa7eec2)

 
Para descargar el archivo docker compose de Greenbone Community Edition, se debe crear un directorio de destino.
Crear directorio de descarga
 ![image](https://github.com/user-attachments/assets/6c56fdd2-1da6-4748-a003-fd2e2c1940f9)

Archivo Docker Compose 
Para ejecutar Greenbone Community Edition con contenedores, se debe utilizar el siguiente archivo de composición:
Archivo Docker Compose
 ![image](https://github.com/user-attachments/assets/956a7162-cb40-4254-b8d0-ba349ac78282)

Bajo Linux
 ![image](https://github.com/user-attachments/assets/0509b70e-9057-4ac0-858c-5d0381224f98)

 
Iniciando los contenedores comunitarios de Greenbone 
Usando el archivo docker compose, se pueden descargar ( extraer ) las imágenes del contenedor y se pueden iniciar los contenedores en segundo plano.
Descarga de los contenedores de la comunidad Greenbone
 ![image](https://github.com/user-attachments/assets/6321d392-a72e-4d81-81a1-ea84f27025bb)

 
Puesta en marcha de los contenedores comunitarios Greenbone
docker compose -f $DOWNLOAD_DIR/docker-compose.yml -p greenbone-community-edition up -d
 ![image](https://github.com/user-attachments/assets/50755113-9de1-4baf-9af5-3acfc24aa7da)

Para obtener un flujo continuo de la salida del registro de todos los servicios, ejecute el siguiente comando:
Mostrar mensajes de registro de todos los servicios de los contenedores en ejecución¶
 
 ![image](https://github.com/user-attachments/assets/58f93e77-061c-459c-a3bc-32b9c740faf8)

 
 
Configurar un usuario administrador 
Advertencia
De forma predeterminada, se crea un usuario admin con la contraseña admin . Esto no es seguro y se recomienda encarecidamente establecer una nueva contraseña.
Para actualizar el usuario administrador con una contraseña de su elección en lugar de la contraseña generada, se puede utilizar el siguiente comando:
Actualizar contraseña del usuario administrador
 
![image](https://github.com/user-attachments/assets/870e1275-244d-4b70-ad9a-9d1e663cec11)

Iniciando la Gestión de Vulnerabilidades 
Una vez iniciados los servicios y cargados todos los datos de las fuentes , se puede abrir la interfaz web de Greenbone Security Assistant (GSA) en el navegador.
Cómo abrir Greenbone Security Assistant en el navegador¶
 
 
![image](https://github.com/user-attachments/assets/75040be1-83d5-4051-b9ce-a07b9159c772)

 ![image](https://github.com/user-attachments/assets/8546ec71-b8b6-4bf6-bc82-4be4b3883980)

Configuración y secuencia de comandos de inicio 
Nota
Recuerde seguir primero las instrucciones descritas en los Requisitos previos .
Como solución rápida, proporcionamos todos los comandos anteriores en un solo script. Este script se puede descargar directamente con el siguiente comando:
Descargar el script de instalación e inicio al directorio de trabajo actual¶
 ![image](https://github.com/user-attachments/assets/0284b27e-9c5f-4cd9-beee-9c8307dfea23)

Para ejecutar el script se debe ejecutar el siguiente comando
Ejecutar la configuración y comenzar el script
 
 ![image](https://github.com/user-attachments/assets/1f326774-810c-48ad-9d1d-1b7f3c5c149e)

  ![image](https://github.com/user-attachments/assets/27b0955a-45d2-4e12-893e-34b00b163c01)

 ![image](https://github.com/user-attachments/assets/e2e2a109-7894-44eb-a372-37137ee59db9)

 ![image](https://github.com/user-attachments/assets/3ced379e-319b-42d4-9462-25bfb5e50767)

 ![image](https://github.com/user-attachments/assets/8f11470e-0f69-452d-bf63-d312db3f6145)

 ![image](https://github.com/user-attachments/assets/df2cbf34-a7fc-4c71-beea-88c5d933a16d)

 ![image](https://github.com/user-attachments/assets/495681bc-c1fa-41ce-98f8-98814c92a953)

 ![image](https://github.com/user-attachments/assets/8b015844-a4c7-486d-a25b-f10584eaa6f8)

 ![image](https://github.com/user-attachments/assets/94f6612b-c114-4c29-987b-637c1472559e)

 ![image](https://github.com/user-attachments/assets/6c5c4607-f023-4ee6-9885-3eed3d02fe3f)

![image](https://github.com/user-attachments/assets/e5439718-f7a9-47e2-9df3-5087162f3b76)

![image](https://github.com/user-attachments/assets/30f51ccd-740f-425b-8db7-e3725308e44b)
