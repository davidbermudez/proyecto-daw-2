# proyecto-dwes-2
## Proyecto Fin de Grado Técnico Superior en Desarrollo de Aplicaciones Web
### Descripción
Aplicación web para votaciones simultáneas en procesos asamblearios
### Introducción del proyecto:
La aplicación pretende simplificar los procesos de voto tradicionales de "a mano alzada" y/o de "viva voz" que ralentizan la adopción de acuerdos en actos asamblearios.
### Finalidad
Facilitar la gestión de votaciones en procesos asamblearios poniendo a disposición de las organizaciones un sistema para que los delegados o compromisarios con derecho a voto puedan ejercerlo desde sus dispositivos móviles, en tiempo real y de manera simultánea evitando así que cada una de las ponencias tengan que ser llamados en orden secuencial para recabar su voto públicamente.
El sistema debe ser configurado de antemano para que el día de la asamblea estén preparadas todas las ponencias que han de ser sometidas a votación, así como correctamente identificados los usuarios con derecho a voto. El día de la Asamblea, desde la administración del sistema, se habilitarán una a una cada ponencia, momento en el que los delegados podrán ejercer su voto **sólo a la ponencia activa**. En el momento que se detecte que todos ellos han ejercido el voto, o en su defecto, se de por terminado el tiempo marcado para ejercerlo, desde la parte de administración se mostrarán los resultados, que podrá ser proyectado en pantalla hacía los asistentes a fin de que puedan verificarlos, así como comprobar que su voto a sido contabilizado.
### Objetivos
Crear un front-end en función del rol del usuario. Para los usuarios llamados a votación, tendrán sus opciones visibles a través de sus dispositivos móviles con las opciones SI/NO/ABSTENCIÓN, así como otras opciones para el caso de que la votación requiera otro tipo de decisiones. La opción de votación sólo estará visible mientras una ponencia se encuentre activa, ofreciendo un mensaje de espera, además de opciones para revisar resultados de votaciones ya finalizadas.
### Medios hardware y software a utilizar

Para el desarrollo de la aplicación web se pretende utilizar el framework Django, conectado a una base de datos MySql. El entorno de desarrollo que se utilizará será Visual Studio Code, con los plugins necesarios para trabajar con Python. Como entorno de pruebas se utilizará un servidor remoto dentro de una red local (una pequeña máquina conectada al router de casa) con las siguientes características:

- Intel(R) Celeron(R) CPU J1800 @ 2.41 GHz
- SO: Linux 5.9.0-0.bpo.2-amd64
- RAM: 8Gb
### Planificación
Si se aprueba el anteproyecto se comenzará con el desarrollo en varias fases:

- Fase de planificación y diseño:
    - Planificación diseño y estructura de la Web
    - Planificación y diseño base de datos
- Fase de desarrollo:
    - Esta aplicación no contiene un front-end propiamente dicho. Todo es back-end, desplegando ante el usuario un panel de control con los correspondientes menús y accesos directos. No obstante se prevé que el uso de CSS/Javascript sea generosa
    - Utilización de Django para desarrollar la web
- Fase de Despliegue
    - Acceso a ssh a un servidor
    - Creación de un entorno virtual
    - Clone de la aplicación
    - Instalación de certificado Let’s Encrypt usando Certbot (importante para el acceso seguro desde la página web)

Teniendo hasta la entrega y presentación del proyecto 12 semanas, el tiempo disponible se reparte de la siguiente manera:

- Planificación y Diseño: 2 semanas
- Desarrollo: 8 semanas
- Despliegue: 2 semanas
