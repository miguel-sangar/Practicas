# 07 - Cómo degradar un servidor a cliente de dominio

Para degradar un servidor a cliente de dominio, dentro del **Administrador del servidor** haremos lo siguiente:

**Administrar** → **Quitar roles y funciones**

![Paso 1](Imagenes/imagen01.png)
![Paso 2](Imagenes/imagen02.png)
![Paso 3](Imagenes/imagen03.png)

En la siguiente ventana deseleccionaremos la opción **Servicios de dominio de Active Directory**:

![Paso 4](Imagenes/imagen04.png)

Y se nos abrirá una ventana en la que pulsaremos en **Quitar características**:

![Paso 5](Imagenes/imagen05.png)

Pulsaremos en Disminuir el nivel de este controlador de dominio:

![Paso 6](Imagenes/imagen06.png)

Pulsamos en **Cambiar**:

![Paso 7](Imagenes/imagen07.png)

Escribimos las credenciales de administrador:

![Paso 8](Imagenes/imagen08.png)

Marcamos el check **Forzar la eliminación de este controlador de dominio**:

![Paso 9](Imagenes/imagen09.png)

Marcamos **Continuar con la eliminación**:

![Paso 10](Imagenes/imagen10.png)

Ponemos la contraseña:

![Paso 11](Imagenes/imagen11.png)
![Paso 12](Imagenes/imagen12.png)

Tras pulsar **Disminuir nivel**, se abrirá otra ventana y el sistema nos pedirá reiniciar el equipo

Una vez hayamos iniciado sesión de nuevo, podremos comprobar que el nombre del grupo de trabajo ha cambiado, ya no se llama **asir.local**

![Paso 13](Imagenes/imagen13.png)