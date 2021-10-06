# [SRI] - Ejercicios unidad 1: Vagrant y Ansible: Programando infraestructura en la nube

Ejercicio 1: Playbook sencillo
1. 1.-Prepara una máquina virtual en KVM que es la que vamos a configurar de forma automática con ansible.
2. 2.-Debes crear un playbook que realice las siguientes tareas de forma automática:

Crear un usuario en el servidor remoto que tenga tu nombre.
Descarga el fichero desde la url https://wordpress.org/latest.zip.
Descomprime ese fichero en el home del usuario creado anteriormente.
Instala el paquete mariadb.
Crea una base de datos que se llame tunombre_wordpress.
Crea un usuario que se llame my_nombre que tenga privilegios sobre la base de datos.
Clona el repositorio: https://github.com/josedom24/ansible_ejemplos.git en el home del usuario que hemos creado en el primer punto.

Para cada uno de estas tareas tienes que usar un módulo especifico de ansible. Entrega la url del repositorio donde has guardado el playbook y también la salida de la ejecución del playbook.


Ejercicio 2: vagrant. Crear un router-nat

Queremos automatizar la creación de la siguiente infraestructura usando Vagrant, el esquema que queremos desarrollar, que vemos en la imagen, tiene las siguientes características:

El escenario tiene dos máquinas:
1.-router, que está conectada a una red publica y a una red privada (muy aislada). La interfaz de red en la red privada se configura con la IP 10.0.0.1.
2.-cliente: Esta máquina está conectada a la misma red privada que la máquina anterior, en este caso su direccionamiento es 10.0.0.2.

En este ejercicio sólo vamos a construir el escenario. No vamos a configurarlo.

Entregaremos:
1.-El fichero Vagrantfile que construya el escenario.
2.-Una captura de pantalla donde se vea un ping de la máquina cliente a la máquina router.
