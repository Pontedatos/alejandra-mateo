# Resumen de la asignatura

## Explicación detallada del contenido de Periodismo de Datos ##

En esta última parte del trabajo final de Periodismo de Datos comentamos **los aprendizajes que hemos realizado a lo largo del curso**, en el cual hemos trabajado con la terminal del ordenador para realizar acciones desde ahí y vincularlas con Github. Tanto de forma práctica como teórica, hemos adquiridio conocimientos sobre el uso de diferentes comandos, lenguajes informáticos y programas para trabajar con datos y analizarlos de manera sencilla y visual.

## Instalación del programa de emulación de la terminal

Para comenzar a trabajar en esta asignatura, hace falta poder hacer uso de la terminal del ordenador para poder realizar las prácticas y aprender comandos. La mayoría de las compañeras tuvieron que descargarse Ubuntu, en un primer momento, y Cygwig posteriormente. Para descargar Ubuntu los pasos a relalizar eran: Entrar en la Windows Power Shell (ya que prácticamente toda la clase tiene Windows) y emplear el comando wsl con la opción y argumentos –install -d Ubuntu. Cygwyg, no obstante, funciona de manera un tanto diferente y se descarga directamente desde la web. En mi caso, no tuve que descargar ninguno de estos emuladores de terminal ya que, al utilizar Mac, ya tenía la terminal por defecto en el ordenador, puesto que esta está presente en todas las versiones de OS X. Dentro de la terminal de Mac, me dirigí a la carpeta “ Aplicaciones” del ordenador y ahí descargué y activé posteriormente XCode. Ejecutando el comando xcode-select - -install, concluí el proceso.

## Trabajar desde la terminal: Explorar directorios y emplear comandos básicos

En primer término,  tenemos que saber dónde estamos (en qué carpeta), y saber dónde están los archivos a los que queremos acceder (en este caso, dónde están en nuestro ordenador los apuntes de la asignatura de Periodismo de datos). Para saber en qué carpeta (directorio) estamos, podemos usar el comando pwd, print workind directory, que nos devolverá una ruta (por ejemplo, /root). Este comando, que es uno de los más importantes, lo utilizamos cada vez que necesitamos saber dónde nos encontramos dentro de la terminal, ya que devuelve la ruta en la que estamos situados.
Si queremos listar (ver) qué archivos hay en la carpeta, usamos el comando ‘ls’. Este comando, además, se puede emplear añadiendo distintas opciones para diferentes resultados. Algunas de estas opciones las hemos explorado en clase a lo largo de la asignatura. Por ejemplo, con ls -a, nos muestra los archivos y directorios dentro del directorio actual, incluyendo los archivos y directorios ocultos. También podemos escribir ls / para listar el contenido del directorio raíz o  man ls, que viene de “ manual” y  nos muestra todos las opciones disponibles para el comando ls

También utilizamos el comando cd, esencial para poder trabajar con archivos y subirlos a Github. Sirve para cambiar de directorio, utilizando la fórmula *cd < RutaDirectorio >* para ir al directorio o carpeta concreta que le digas, o *cd..* (con dos puntos) para salir de una carpeta e ir al nivel superior o carpeta donde estaba alojada.

Asimismo, otros comandos básicos que hemos aprendido a utilizar han sido mkdir, para crear un directorio, por ejemplo, para crear una carpeta donde meteremos todos nuestros repositorios de GitHub: mkdir github. También estaría whoami, que nos devuelve nuestro usuario y resulta verdaderamente práctico cuando trabajamos desde la terminal.

Hemos trabajado en clase con otros comandos, muchos de ellos también muy interesantes y útiles, que se detallarán en el epígrafe último de esta práctica

## Trabajar con Github

Github es una de las principales plataformas para crear proyectos abiertos de herramientas y aplicaciones, y se caracteriza sobre todo por sus funciones colaborativas que ayudan a que todos puedan aportar su granito de arena para mejorar el código. En clase lo hemos utilizado como medio que nos permite subir y presentar nuestras prácticas, lo que resulta útil de cara al futuro para visibilizar nuestros proyectos. Por tanto, era esencial vincular nuestra carpeta local del ordenador individual de cada una con el repositorio en cuestión de Github, que se encuentra online. De esta forma, los cambios ejecutados en nuestro archivo local se añaden también al repositorio en línea.

El primer paso para conseguir esto reside en clonar nuestro repositorio. Entramos en la carpeta de nuestros apuntes que previamente habremos creado en el ordenador, copiamos el enlace de nuestro repositorio (icono verde situado arriba a la derecha, ‘Code’ que nos ofrece el enlace que buscamos). En la terminal, escribimos git clone y lo copiamos a continuación. También podemos especificar el nombre de la carpeta que se creará con los archivos del repositorio, escribiendo tal nombre al final de la línea. Hay que asegurarnos de que esto lo estamos haciendo en la carpeta que queremos, por tanto el comando pwd nos ayuda a asegurarnos situándonos y si quisiéramos cambiar de directorio, utilizaríamos cd para movernos.

Llegados a este punto, para configurar el usuario y el correo de Github en la terminal (de cara a vincular los cambios realizados), utilizaremos dos comandos: git config --global user.name nuestrousuario , y posteriormente git config --global user.email correogithub. Finalmente, necesitaremos vincular los archivos. Primero escribimos git status para ver que efectivamente se ha hecho una modificación y después utilizamos git add nombre-archivo o git add simplemente. De este modo, el comando indica a Git que quieres incluir actualizaciones en un archivo concreto en la próxima confirmación. Todavía nos faltan otros dos comandos imprescindibles para la actualización del directorio:  Para hacer el commit, tenemos que hacer un git commit -m “Mensaje del commit” . Entre comillas va el mensaje del cambio, que se verá en GitHub. Hechos todos los cambios y hechos los commits, hacemos un git push para que se suba a nuestro repositorio de GitHub. Para muchas personas, en este último paso ha sido necesario usar un token, no así en mi caso, probablemente porque mi ordenador es un Mac. Además, utilizaríamos git pull ya que permite actualizar el repositorio local con el contenido del remoto. En la asignatura hemos tenido [un repositorio en nuestro perfil de Github](https://github.com/Alejandraa98/practicas-periodismo-de-datos) en el que hemos ido depositando las prácticas realizadas a lo largo del curso, teniendo así los archivos ordenados y clasificados. 

## Configuración de un programa de edición de texto

En clase utilizamos nano como editor de texto para trabajar con él desde la terminal. Para instalarlo hemos procedido con brew install nano. Para que se ajuste el texto a la pantalla (en nano, por defecto, cada línea es un párrafo, lo que resulta incómodo), así como conseguir la numeración de las líneas, fue necesario ejecutar nano $HOME/.nanorc + # Ajustar el texto a pantalla set softwrap # Numerar las líneas set linenumbers. Guardamos los cambios con ctrl+o.

## Configuración y funcionamiento de un gestor de paquetes del emulador de la terminal

En las clases de Periodismo de datos nos encontramos habitualmente con problemas de desconocimiento terminológico ya que, en muchas ocasiones, trabajamos con conceptos que ni siquiera conocemos debido a nuestras pocas nociones previas de informática. Por tanto, cuando en clase explicó el profesor como funcionan los gestores de paquetes, la mayoría tuvimos que buscar en Internet precisamente qué significa este término. Según Debian.org, un gestor de paquetes mantiene un registro del software que está instalado en su ordenador, y le permite instalar software nuevo, actualizarlo a versiones más recientes, o eliminar software de una manera sencilla. Una vez sabemos de qué estamos hablando, podemos proceder a instalar el gestor que se adecúe a nuestro ordenador. Para la mayoría de compañeras que usan Windows, el de Ubuntu es apty el de Cygwin apt-cyg. Para mi, que utilizo Mac OS X, el administrador de paquetes más popular es Homebrew. En la terminal, realizamos la siguente acción de cara a poder instalarlo correctamente:/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

## Versión del lenguaje Shell utilizado

El lenguaje de Shell empleado ha sido Bash, que viene predeterminado en macOS. Para comprobar que funciona, ponemos echo $0 (eco para que devuelva el texto a la pantalla ya que $ es una variable de entorno (este concepto lo explicaré a continuación más detalladamente puesto que también lo hemos trabajado en numerosas sesiones de la asignatura). Desde la propia terminal el usuario puede pasar a zsh , ejecutando para ello chsh -s /bin/zsh. Para conocer la versión específica de Bash lo hacemos a través de Bash - - version.

## Las variables de entorno: El valor de la variable de entorno ' Path'

Lo primero que hicimos para trabajar con variables de entorno fue resolver la duda de qué significa este concepto exactamente: Según Genbeta, una variable de entorno es una cadena de texto que sistemas operativos como Windows, Linux o Mac usan para almacenar valores que pueden variar de un equipo a otro o de un usuario a otro pero que, sin embargo, necesitan de un modo unificado de acceder al mismo. Las variables de entorno empiezan por el símbolo del dólar $ (aunque no tiene que ver con el que aparece al principio de la línea cuando escribimos desde la terminal). Por ejemplo, $HOME significa la ruta de nuestro usuario (/mnt/c/Users/usuaria). $PATH nos muestra las rutas donde están los programas que se puedan ejecutar. Para consultar, usamos echo. echo $PATH nos muestra las rutas. Para saber el valor de PATH, indicamos a “echo” que se trata de una variable. Para ello, escribo en la terminal echo $PATH, donde el símbolo del dólar es lo que indica que se trata de una variable de entorno. Un ejemplo de una variable de entorno de usuario es %homepath%. 

## Python y Jupyer para trabajar el análisis y visualización de datos

En las últimas clases hemos trabajado con Python, un lenguaje informático que, a diferencia de otros como Java constituye un lenguaje interpretado que no es necesario ser compilado para ejecutar aplicaciones escritas, ya que estas se ejecutan directamente por el ordenador usando un programa concreto, de manera que no es necesario traducirlo. Se trata de un lenguaje sencillo de leer y escribir debido a su alta similitud con el lenguaje humano. Además, se trata de un lenguaje de código abierto y, por lo tanto, gratuito, lo que permite desarrollar software sin límites. Además, a nosotros como estudiantes de la asignatura de Periodismo de Datos nos resulta muy práctico debido que este lenguaje está muy extendido en el área del análisis de datos y el big data ya que permite gestionar una gran cantidad de datos en tiempo real. 

En clase hemos empleado Jupyter, una aplicación online que utiliza este lenguaje y en la que, por medio de sus notebooks o cuadernos, hemos podido desarrollar diferentes prácticas en las que trabajamos con apis o conjuntos de datos para después analizarlos y trabajar con librerías importadas para la visualización y presentación de datos. Los pasos a seguir para trabajar con datos dentro de estos cuadernos están detallados en las [prácticas 3](https://github.com/Pontedatos/alejandra-mateo/blob/master/python-api-covid19-pandas%20(1).ipynb) y [práctica 4](https://github.com/Pontedatos/alejandra-mateo/blob/master/Practica4%20(1).ipynb), donde aparece paso a paso la explicación sobre cómo hemos explorado las diferentes funciones y acciones a desarrollar.

## Comandos utilizados

Aunque gran parte de los comandos que hemos utilizado en clase y que hemos puesto en práctica en los distintos trabajos presentado en la asignatura ya figuran en los apartados anteriores de esta práctica final, aquí se presentan algunos no mencionados anteriormente y que han resultado de gran utilidad. Asimismo, los comandos que aparecen a continuación no figuran en orden de aprendizaje. Los comandos siguen una estructura de comando / opciones / argumentos.

**env** → Para visualizar en la pantalla la lista de variables de entorno

**touch [nombre del archivo]** → Crear un archivo nuevo

**whoami** → Nombre de usuario

**mkdir + nombre de carpeta** → Crear una carpeta o directorio

**Ctr + x** → Salir del editor de texto (nano)

**cat** → Concatenar varios archivos

**rm –help** → Ver las posibilidades de los comandos

**mv** → mover o las carpetas o archivos de sitio y también para renombrarlos

**cp [origen] [destino]** → para copiar y pegar carpetas y archivos

**nano [archivo]** → Editor de texto que usamos desde la terminal del ordenador

**tree** → Ofrece más opciones que ls para poder ver diferentes niveles

**wget [enlace]** → Para descargarnos un archivo o contenido de una web




