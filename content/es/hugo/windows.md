+++
title = "Instalación en Windows"
tags = ["hugo","instalación","windows"]
categories=["hugo"]
banner = "../img/windows.jpeg"
authors = ["Andrés"]
+++
[choco]:https://desarrolloweb.com/home/chocolatey
## Paso a paso

Para instalar Hugo dentro de un sistema operativo [Windows](https://es.wikipedia.org/wiki/Microsoft_Windows) lo más conveniente será instalarse un gestor de paquetes para poder instalarlo tan solo con un comando. El gestor de paquetes escogido es [Chocolatey][choco].


Primero de todo debemos validar que las políticas de ejecución estén habilitadas. Accedemos como administradores a PowerShell y escribimos lo 
siguiente:
~~~
Get-ExecutionPolicy
~~~
Si el resultador es Restricted tendremos que habilitarlas y confirmarlas :
~~~
Set-ExecutionPolicy AllSigned
~~~
~~~
Get-ExecutionPolicy
~~~
Si has seguido con los pasos anteriores, no tendrías ninguna a instalar [Chocolatey][choco] con la siguiente instrucción:
~~~
Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))
~~~
Finalmente instalamos Hugo sobre Windows:
~~~
choco install hugo -confirm
~~~

Aquí os dejo un video para la instalación de Hugo en Windows:

{{< youtube l7PHRA8t4Bw >}}


#### Para la instalación en linux pulsa [aqui]({{< ref "linux.md" >}}).
