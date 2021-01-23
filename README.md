# proyecto-dwes-2
## Proyecto Fin de Grado Técnico Superior en Desarrollo de Aplicaciones Web
### Descripción
Aplicación web para la Gestión Remota de Sistemas
### Introducción del proyecto:
El proyecto pretende crear un entorno web amigable para la administración de un sistema Linux remoto. 
### Finalidad
Facilitar al usuario administrador las tareas habituales de gestión de servidores sin necesidad de acceder vía ssh o de tener que ser un especialista en el manejo de comandos. A través de la aplicación web, el usuario puede usar un navegador de internet para tener acceso al estado completo de su sistema, a la gestión de usuarios, configuración de red, instalación de aplicaciones, actualizaciones de sistema, y todo aquello que habitualmente puede hacerse desde la consola de comandos, pero en un entorno amigable e intuitivo que aspira a hacer más fácil la gestión de un servidor ubicado en cualquier parte del mundo.
### Objetivos
La aplicación permitirá a los administradores de sistemas actuar sobre las principales funciones del equipo:
- Gestión de Usuarios
    - Creación/Edición/Eliminación de Usuarios
    - Creación/Edición/Eliminación de Grupos
- Gestión de Apache/Nginx
    - Configuración de VirtualHost
    - Instalación de Certificados
- Gestión de Bases de Datos
    - Instalación y configuración del SGBD disponibles para el usuario
- Gestión de Servicios
    - Configuración FTP
    - Configuración SSH
    - Configuración Mail
- Gestión de Archivos
    - Configuración Permisos
    - Compartición de carpetas
    - Copiar/Mover/Eliminar archivos y/o directorios
- Gestión de Dispositivos
    - Configuración de Disco
- Gestión de Diagnóstico
    - Monitorización de sistema
    - Actualización de paquetes
### Medios hardware y software a utilizar
Este proyecto se encarga de la parte de diseño, desarrollo y despliegue de la aplicación web, que conectará las órdenes del usuario con un lanzador de scripts que se encargarán, en última instancia, de ejecutar los comandos necesarios sobre el sistema en el que se está ejecutando. 

Este proyecto es una parte de otro proyecto desarrollado conjuntamente con un alumno de Administración de Sistemas Informáticos en Red, por lo que no forma parte de él, la descripción sobre la ejecución de scripts, diseño de parámetros, y comprobación de errores, ya que la aplicación web, se limitará a recabar los posibles mensajes con el resultado obtenido para mostrarlo al usuario a través de la web.

Para el desarrollo de la aplicación web se pretende utilizar el framework Django, conectado a una base de datos MySql. El entorno de desarrollo que se utilizará será Visual Studio Code, con los plugins necesarios para trabajar con Python. Como entorno de pruebas se utilizará un servidor remoto dentro de una red local (una pequeña máquina conectada al router de casa) con las siguientes características:

- Intel(R) Celeron(R) CPU J1800 @ 2.41 GHz
- SO: Linux 5.9.0-0.bpo.2-amd64
- RAM: 8Gb
### Planificación
Si se aprueba el anteproyecto se comenzará con el desarrollo en varias fases:

- Fase de planificación y diseño:
-- Planificación diseño y estructura de la Web
-- Planificación y diseño base de datos
- Fase de desarrollo:
-- Esta aplicación no contiene un front-end propiamente dicho. Todo es back-end, desplegando ante el usuario un panel de control con los correspondientes menús y accesos directos. No obstante se prevé que el uso de CSS/Javascript sea generosa
-- Utilización de Django para desarrollar la web
- Fase de Despliegue
-- Acceso a ssh a un servidor
-- Creación de un entorno virtual
-- Clone de la aplicación
-- Instalación de certificado Let’s Encrypt usando Certbot (importante para el acceso seguro desde la página web)
Teniendo hasta la entrega y presentación del proyecto 12 semanas, el tiempo disponible se reparte de la siguiente manera:

- Planificación y Diseño: 2 semanas
- Desarrollo: 8 semanas
- Despliegue: 2 semanas