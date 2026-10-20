# Cómo instalar MySQL Server y MySQL Workbench en Windows

MySQL Server y MySQL Workbench tienen propósitos diferentes:

Mientras que MySQL Server se encarga de almacenar bases de datos, procesar consultas y aceptar conexiones desde una terminal... Con MySQL Workbench podemos acceder a dicha información desde una interfaz gráfica.

Primero vamos a ver cómo instalar MySQL Server y después veremos como instalar MySQL Workbench de forma sencilla.

## Cómo instalar MySQL Server

![Portada MySQL Server](Imagenes/portadaServer.jpg)

El primer paso para instalar MySQL Server será ir a la web oficial de MySQL, en el apartado **Community Downloads**: https://dev.mysql.com/downloads/mysql/

Luego, descargamos el MSI Installer:

![Paso 1](Imagenes/imagen01.png)

Pulsamos en "No thanks, just start my download" y la descarga se iniciará:

![Paso 2](Imagenes/imagen02.png)

Ejecutamos el fichero .msi que se ha descargado y nos aparecerá la siguiente pantalla:

![Paso 3](Imagenes/imagen03.png)

Pulsamos en "Next" y aceptamos los términos y condiciones:

![Paso 4](Imagenes/imagen04.png)

A continuación, seleccionamos la opción "Complete":

![Paso 5](Imagenes/imagen05.png)

Y pulsamos en "Install"

![Paso 6](Imagenes/imagen06.png)

Esperamos a que termine de instalarse y pulsamos en "Finish":

![Paso 7](Imagenes/imagen07.png)

Aparecerá otra ventana para configurar MySQL:

![Paso 8](Imagenes/imagen08.png)

Seleccionamos la segunda opción "Configure this server instance as a side-by-side installation":

![Paso 9](Imagenes/imagen09.png)

Establecemos un puerto que esté libre. En mi caso, he puesto **3305** porque el **3306** estaba ocupado:

![Paso 10](Imagenes/imagen10.png)

El siguiente paso será establecer la contraseña de acceso a la base de datos. Luego pulsaremos en el botón **Add User**:

![Paso 11](Imagenes/imagen11.png)

Escribimos el nombre de usuario que queramos para nosotros, indicando "All Host (%)" y role "DB Admin" y establecemos una contraseña segura.

![Paso 12](Imagenes/imagen12.png)

Tras crear el usuario, nos quedará algo como esto:

![Paso 13](Imagenes/imagen13.png)

En la siguiente ventana, lo dejamos todo como está para que MySQL arranque automáticamente al encender nuestro servidor:

![Paso 14](Imagenes/imagen14.png)

Dejamos la opción que viene por defecto:

![Paso 15](Imagenes/imagen15.png)

Como no queremos crear ninguna base de datos de ejemplo, no marcamos ninguna de las siguientes opciones:

![Paso 16](Imagenes/imagen16.png)

Pulsamos en el botón "Execute" para que se aplique la configuración:

![Paso 17](Imagenes/imagen17.png)
![Paso 18](Imagenes/imagen18.png)

Por último, y para completar la configuración, pulsamos en "Finish":

![Paso 19](Imagenes/imagen19.png)

Para comprobar que MySQL Server funciona correctamente, podemos ejecutar terminal **MySQL Command Line Client**. Nos pedirá la contraseña de acceso a la base de datos. Tras ponerla, nos mostrará la versión actual.

Y si ponemos el comando `show databases;` nos mostrará las bases de datos creadas:

![Paso 20](Imagenes/imagen20.png)

## Cómo instalar MySQL Workbench

![Portada MySQL Workbench](Imagenes/portadaWorkbench.jpg)

Entraremos al enlace oficial de descarga: https://dev.mysql.com/downloads/workbench/

Descargamos el fichero .msi:

![Paso 21](Imagenes/imagen21.png)

Pulsamos en "No thanks, just start my download":

![Paso 22](Imagenes/imagen22.png)

Ejecutamos el fichero que se ha descargado para iniciar la instalación:

![Paso 23](Imagenes/imagen23.png)

Instalamos solo para el usuario que estamos usando:

![Paso 24](Imagenes/imagen24.png)

Pulsamos en "Install":

![Paso 25](Imagenes/imagen25.png)

Dejamos marcada la opción "Run MySQL Workbench" y pulsamos en "Finish":

![Paso 26](Imagenes/imagen26.png)

Una vez finalizada la instalación se nos abrirá la interfaz gráfica y veremos algo como esto:

![Paso 27](Imagenes/imagen27.png)

