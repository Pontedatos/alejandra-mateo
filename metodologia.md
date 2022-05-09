# Metodología utilizada en la práctica final de Periodismo de datos

En esta última práctica de la asignatura Periodismo de Datos hemos creado, en la organización Pontedatos, un repositorio nuevo en el que hemos introducido todas las prácticas llevado a cabo a lo largo del curso. Estas prácticas están explicadas en distintos archivos de github que figuran en esta práctica final.
También hemos creado una página web desde Github, dotando de una estructura web a la información.

## 1. Crear un nuevo repositorio y recopilar ahi los trabajos de la asignatura

En primer lugar, **creamos un repositorio común** para todas las práctias de la asignatura desde nuestro perfil personal de Github (Repositories-New). Después de aceptar la invitación del usuario Pontedatos, establecemos a este como creador, por tanto el Owner o propietario será Pontedatos y no nuestro propio perfil o usuario personal. Por lo tanto en el perfil de Pontedatos podremos ver tanto los repositorios que hemos subido las alumnas individualmente como también los repositorios que las compañeras han subido ya que todas tenemos acceso a este perfil que nos ha facilitado el profesor.
En el nombre del repositorio escribimos **nuestro nombre de usuario** (yo he puesto alejandra-mateo), como ha especificado el profesor, evitando mayúsculas, acentos o espacios que no deben ponerse nunca en nombres de archivos en Github. En enlace final del repositorio será, por tanto, https://github.com/Pontedatos/alejandra-mateo.

Ahora **vinculamos el repositorio recién creado con nuestro ordenador**. Para vincularlo a nuestro ordenador para que la carpeta local esté conectada al repositorio, empleamos el comando git clone y a continuación, mediante cd en nuestra terminal, cambiamos de directorio, yendo hasta aquel en el que queremos que se clone el repositorio. Lo guardamos todo en una carpeta y comprobamos que está todo bien con git remote-v.

En el siguiente paso tenemos que volcar el contenido de las prácticas anteriores en el repositorio de Github y en local. Con cp, estableciendo como origen las prácticas guardadas en el repositorio anterior y como destino la nueva carpeta del repositorio Pontedatos. Cambiamos en nano los enlaces absolutos de las prácticas 3 y 4, incluido el README, para que sean relativos, ya que es necesario a la hora de dotar de una estructura web al repositorio final. Ejecutamos git add ., git commit -m "practicas-nuevo-repositorio" y git push.

## 2. Crear una estructura para la web

Por último, cuando ya hemos conseguido tener todos los archivos en nuestro repositorio, **creamos una página web** con una estructura adecuada que permita poder visualizar todos los archivos, a través de Github y las opciones que ofrece. En el repositorio están todos los archivos al mismo nivel, podría haber carpetas pero eso dificultaría la visualización del contenido. El siguiente paso es ir a *Settings* y seleccionar *Pages*, activándola previamente y eligiendo como fuente la rama main del repositorio como /root. Guardamos los cambios y **elegimos el tema del diseño web** en el apartado de *Theme Chooser*. En mi caso he optado por usar el Slate theme, sobrio pero elegante. 

Cuando Github Pages ha creado nuestra web, nos quedaría el enlace https://pontedatos.github.io/alejandra-mateo/. Cuando entramos, vemos al visitar la web que Github ha convertido el archivo README.md en la pag. de inicio, que al ser HTML es index.html, como ocurre con el resto de documentos escritos en Markdown.
