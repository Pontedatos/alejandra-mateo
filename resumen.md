# Resumen de la asignatura

## Explicación detallada del contenido de Periodismo de Datos ##

En esta última parte del trabajo final de Periodismo de Datos comentamos los aprendizajes que hemos realizado a lo largo del curso, en el cual hemos trabajado con la terminal del ordenador para realizar acciones desde ahí y vincularlas con Github. Tanto de forma práctica como teórica, hemos adquiridio conocimientos sobre el uso de diferentes comandos, lenguajes informáticos y programas para trabajar con datos y analizarlos de manera sencilla y visual.

## Instalación del programa de emulación de la terminal

Para comenzar a trabajar en esta asignatura, hace falta poder hacer uso de la terminal del ordenador para poder realizar las prácticas y aprender comandos. La mayoría de las compañeras tuvieron que descargarse Ubuntu, en un primer momento, y Cygwig posteriormente. Para descargar Ubuntu los pasos a relalizar eran: Entrar en la Windows Power Shell (ya que prácticamente toda la clase tiene Windows) y emplear el comando wsl con la opción y argumentos –install -d Ubuntu. Cygwyg, no obstante, funciona de manera un tanto diferente y se descarga directamente desde la web. En mi caso, no tuve que descargar ninguno de estos emuladores de terminal ya que, al utilizar Mac, ya tenía la terminal por defecto en el ordenador, puesto que esta está presente en todas las versiones de OS X. Dentro de la terminal de Mac, me dirigí a la carpeta “ Aplicaciones” del ordenador y ahí descargué y activé posteriormente XCode. Ejecutando el comando xcode-select - -install, ya concluí el proceso.

## Configuración de un programa de edición de texto

En clase utilizamos nano como editor de texto para trabajar con él desde la terminal. Para instalarlo hemos procedido con brew install nano. Para que se ajuste el texto a la pantalla (en nano, por defecto, cada línea es un párrafo, lo que resulta incómodo), así como conseguir la numeración de las líneas, fue necesario ejecutar nano $HOME/.nanorc + # Ajustar el texto a pantalla set softwrap # Numerar las líneas set linenumbers. Guardamos los cambios con ctrl+o.

## Configuración y funcionamiento de un gestor de paquetes del emulador de la terminal

En las clases de Periodismo de datos nos encontramos habitualmente con problemas de desconocimiento terminológico ya que, en muchas ocasiones, trabajamos con conceptos que ni siquiera conocemos debido a nuestras pocas nociones previas de informática. Por tanto, cuando en clase explicó el profesor como funcionan los gestores de paquetes, la mayoría tuvimos que buscar en Internet precisamente qué significa este término. Según Debian.org, un gestor de paquetes mantiene un registro del software que está instalado en su ordenador, y le permite instalar software nuevo, actualizarlo a versiones más recientes, o eliminar software de una manera sencilla. Una vez sabemos de qué estamos hablando, podemos proceder a instalar el gestor que se adecúe a nuestro ordenador. Para la mayoría de compañeras que usan Windows, el de Ubuntu es apty el de Cygwin apt-cyg. Para mi, que utilizo Mac OS X, el administrador de paquetes más popular es Homebrew. En la terminal, realizamos la siguente acción de cara a poder instalarlo correctamente:/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
