# proyecto-dwes-2
## Proyecto Fin de Grado Técnico Superior en Desarrollo de Aplicaciones Web
### Descripción
Aplicación web para votaciones simultáneas en procesos asamblearios
### Introducción del proyecto:
La aplicación pretende simplificar los procesos de voto tradicionales de "a mano alzada" y/o de "viva voz" que ralentizan la adopción de acuerdos en actos asamblearios.
### Finalidad
Facilitar la gestión de votaciones en procesos asamblearios poniendo a disposición de asociaciones, comunidades, juntas y asambleas de un sistema para que los delegados, asistentes o compromisarios con derecho a voto puedan ejercerlo desde sus dispositivos móviles, en tiempo real y de manera simultánea evitando así que en cada una de las ponencias a debatir tengan que ser llamados en el orden que hayan establecido para recabar su voto públicamente.
### Objetivos
El sistema debe ser configurado de antemano para que el día del acto se hayan introducido todas las ponencias que han de ser sometidas a votación, así como correctamente identificados los usuarios con derecho a voto. El día de celebración, desde la administración del sistema, se habilitarán una a una cada ponencia, momento en el que los delegados podrán ejercer su voto **sólo a la ponencia activa**. En el momento que se detecte que todos ellos han ejercido el voto, o en su defecto, se de por finalizdo un tiempo límite marcado para ejercerlo, desde la administración se detendrá la votación y se mostrarán los resultados, que podrá ser proyectado en pantalla hacía los asistentes a fin de que puedan verificarlos y comprobar que su voto ha sido contabilizado.
Crear un front-end en función del rol del usuario. Para los usuarios llamados a votación, después de la autenticación, el sistema les mostrará la ponencia en curso y con las opciones SI/NO/ABSTENCIÓN, así como otras opciones para el caso de que la votación requiera otro tipo de decisiones. La opción de votación sólo estará visible mientras una ponencia se encuentre activa. En los momentos en los que no hay votaciones activas, el usuario contará con opciones para revisar resultados de votaciones ya finalizadas mediante un sistema de navegación por menú. La parte de administración 
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
    - Desarrollo vista de administrador
    - Desarrollo vista de usuario
    - Diseño de tests
    - Fase de testeo/subsanación de errores
- Fase de Despliegue
    - Acceso a ssh a un servidor
    - Creación de un entorno virtual
    - Instalación de la aplicación
    - Instalación de certificado Let’s Encrypt usando Certbot (importante para el acceso seguro desde la página web)

Teniendo hasta la entrega y presentación del proyecto 12 semanas, el tiempo disponible se reparte de la siguiente manera:

- Planificación y Diseño: 2 semanas
- Desarrollo: 8 semanas
- Despliegue: 2 semanas
