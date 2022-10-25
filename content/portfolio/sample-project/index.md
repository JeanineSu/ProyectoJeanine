---
title: Instalación
description: This is the description of our sample project

jobDate: 2022
work: [Click aquí]

thumbnail: sample-project/sample.png
projectUrl: https://www.youtube.com/watch?v=6H0jLIKe0uw

---


<h3>Instalación Hugo en Linux</h3> <br/>

**Comprobar si tenemos instalado Snap**

Para instalar Hugo en Linux vamos a utilizar el gestor de paquetes Snap. Por ello lo primero que vamos a hacer es comprobar si tenemos este gestor instalado, para ello utilizaremos el siguiente comando:

```shell 
snap version
```
Este nos debería dar una respuesta como la siguiente:

```shell 
snap    2.55.3+22.04
snapd   2.55.3+22.04
series  16
ubuntu  22.04
kernel  5.15.0-48-generic
```
En ese caso significará que tenemos snap instalado. Entonces podemos empezar con la instalación.

**Instalar el paquete hugo-extended**

Utilizando el gestor Snap vamos a instalar el paquete hugo-extended.

```shell 
snap install hugo --channel=extended
```

<h3>Instalación Hugo en Windows</h3>

Para instalar la ultima versión de Hugo en Windows lo primero que deberemos hacer es ir al siguiente link.

Una vez aquí descargaremos la ultima versión que tenga un nombre del formato hugo_extended_x.x.x_windows-amd64.zip donde x.x.x corresponderá a la versión.

Este zip contendrá el CMS, pero la instalación tendremos que realizarla manualmente.

Extraeremos el zip y para mayor facilidad moveremos el archivo Hugo.exe resultante a la ruta C:\Hugo\bin la cual crearemos.

Una vez lo tengamos, en el buscador de Windows, accederemos a Editar las variables de entorno del sistema buscando esto en el.

Se nos abrirá una ventana llamada Propiedades del sistema y en esta volveremos a pulsar en Variables de entorno.

En la lista que nos mostrará buscaremos la variable PATH, y al final de esta añadiremos ‘;C:\Hugo\bin’.

Con esto reiniciando el sistema tendremos hugo instalado y accesible en nuestro sistema.

