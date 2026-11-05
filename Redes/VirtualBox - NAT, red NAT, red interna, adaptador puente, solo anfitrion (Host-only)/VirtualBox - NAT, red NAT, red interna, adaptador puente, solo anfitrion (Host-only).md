# Diferencia entre NAT, red NAT, red interna, adaptador puente, solo anfitrion (Host-only)

A la hora de configurar una red de un sistema operativo en VirtualBox, debemos diferenciar entre distintos tipos de red.

Imaginemos que tenemos como sistema operativo principal Windows 11, y tenemos como máquina virtual Kali Linux.
Podemos configurar la red de esa máquina de las siguientes formas:

* **NAT**: Kali Linux tendría acceso a internet compartiendo la misma IP pública que Windows 11, pero cada sistema operativo tendría su propia IP privada.

* **Red NAT**: Kali Linux tendría acceso a internet compartiendo la misma IP pública que Windows 11, pero, a diferencia del modo NAT, podríamos conectar varias máquinas virtuales a una misma red NAT. De esta forma, las máquinas virtuales podrían comunicarse entre sí, además de tener acceso a internet. Cada máquina virtual tendría su propia IP privada dentro de esa red.

* **Red interna**: Kali Linux estaría conectado a una red privada que únicamente permitiría la comunicación entre las máquinas virtuales que estén conectadas a esa misma red interna. No tendría acceso a internet ni podría comunicarse directamente con Windows 11 (el sistema anfitrión). Es útil para crear laboratorios aislados en los que practicar con varias máquinas virtuales sin que exista comunicación con la red física.

* **Adaptador puente (Bridged)**: Kali Linux estaría conectado directamente a la misma red física que Windows 11, como si fuera otro ordenador conectado al router mediante un cable Ethernet o Wi-Fi. Por tanto, el router le asignaría una dirección IP propia, diferente de la de Windows 11. Ambos sistemas podrían comunicarse entre sí y con otros dispositivos de la red local, además de tener acceso a internet.

* **Solo anfitrión (Host-Only)**: Kali Linux podría comunicarse con Windows 11 y con otras máquinas virtuales conectadas a la misma red de solo anfitrión, pero no tendría acceso a internet de forma predeterminada. Se crea una red privada entre el sistema anfitrión y las máquinas virtuales, sin necesidad de conectarse a la red física. Es especialmente útil para realizar prácticas de ciberseguridad en un entorno controlado.