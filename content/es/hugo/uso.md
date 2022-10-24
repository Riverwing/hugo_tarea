+++
title = "Práctica de Hugo"
tags = ["hugo","practica"]
banner = "../img/hugo.png"
authors = ["Andrés"]
+++

[theme]:https://themes.gohugo.io/
[md]:https://es.wikipedia.org/wiki/Markdown
[img1]: /img/capVSC.png "Visual Studio sin theme"
[img2]: /img/capUNI.png "Universal"
[img3]: /img/capCONFIG.png "config.toml"
## Objetivos

En este práctica usaremos la herramienta Hugo para crear una página estática gracias a una plantilla que nos descargaremos desde la [web de Hugo][theme]. 
La práctica consistirá de usar todas las posibilidades que nos de la plantilla para generar contenido gracias al [lenguaje Markdown][md] sobre diferentes apartados vistos en el inicio de curso.  



### Primeros pasos

Una vez instalado Hugo en el sistema operativo, continuamos creando un directorio local con el comando:
~~~
mkdir Hugo/Proyectos -p
~~~
Crearemos el sitio estático:
~~~
hugo new site hugo_tarea
~~~
Para poder trabajar con él de una manera gráfica vemos conveniente el uso del IDE Visual Studio Code.
Lo podemos instalar con el siguiente comando:
~~~
sudo snap install code --classic
~~~
Abrimos el proyecto para visualizarlo:


![img1]


Como podemos observar podriamos generar un nuevo tema creando nuestras propias plantillas pero en este caso vamos a optar por instalar un tema ya creado y trabajar desde él. Para ello nos dirigimos a los [temas de Hugo][theme] y nos decantamos por el tema [Universal](https://themes.gohugo.io/themes/hugo-universal-theme/).


![img2]


Instalaremos el tema dentro de la carpeta theme del proyecto con el comando:
~~~
git clone https://github.com/dewcows/hugo-universal-theme
~~~
Finalmente para poder usar este tema como plantilla para nuestro proyecto tendremos que ir al archivo de configuración _config.toml_ y pondremos en theme el nombre de la plantilla que nos hemos descargado:


![img3]







