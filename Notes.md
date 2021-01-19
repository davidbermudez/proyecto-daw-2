# Anotaciones

## Creación de un entorno virtual

Creamos un directorio de trabajo y en él un entorno virtual de desarrollo.

```
$ mkdir proyecto-dwes-2
$ cd proyecto-dwes-2
$ pipenv shell
```

Una vez dentro del entorno virtual instalamos **django**
```
$ pipenv install django
```
Esta instrucción produce la siguiente salida:
```
Installing django...
Adding django to Pipfile's [packages]...
✔ Installation Succeeded  
Pipfile.lock not found, creating...
Locking [dev-packages] dependencies...
Locking [packages] dependencies...
Building requirements...
Resolving dependencies...
✔ Success!  
Updated Pipfile.lock (06f36b)!
Installing dependencies from Pipfile.lock (06f36b)...
    ▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉ 0/0 — 00:00:00
```

Creamos un nuevo proyecto:
```
$ django-admin startproject project
```

Para verificar que ha creado la estructura necesaria de todo proyecto djando, examinamos archivos y directorios
```
$ tree
```

El resultado es el siguiente:

```
$ tree  
.
├── Pipfile
├── Pipfile.lock
└── project
   ├── manage.py
   └── project
       ├── asgi.py
       ├── __init__.py
       ├── settings.py
       ├── urls.py
       └── wsgi.py

2 directories, 8 files
```
Nos movemos a la carpeta del proyecto (*project*) y lo ejecutamos con python
```
$ python3 manage.py runserver
```
Este comando lanza el código de python contenido en el archivo manage.py y pone en marcha un servidor web virtual accesible en el puerto 8000. La salida del comando es la siguiente:
```
Watching for file changes with StatReloader
Performing system checks...

System check identified no issues (0 silenced).

You have 18 unapplied migration(s). Your project may not work properly until you apply the 
migrations for app(s): admin, auth, contenttypes, sessions.                                   
Run 'python manage.py migrate' to apply them.
January 19, 2021 - 17:57:08
Django version 3.1.5, using settings 'project.settings'
Starting development server at http://127.0.0.1:8000/
Quit the server with CONTROL-C.
[19/Jan/2021 17:57:24] "GET / HTTP/1.1" 200 16351
[19/Jan/2021 17:57:25] "GET /static/admin/css/fonts.css HTTP/1.1" 200 423
Not Found: /favicon.ico
[19/Jan/2021 17:57:25] "GET /favicon.ico HTTP/1.1" 404 1973
[19/Jan/2021 17:57:25] "GET /static/admin/fonts/Roboto-Regular-webfont.woff HTTP/1.1" 200 85
876
[19/Jan/2021 17:57:25] "GET /static/admin/fonts/Roboto-Bold-webfont.woff HTTP/1.1" 200 86184
[19/Jan/2021 17:57:25] "GET /static/admin/fonts/Roboto-Light-webfont.woff HTTP/1.1" 200 8569
```
El server se mantendrá activo hasta que interrumpamos la ejecución del comando

