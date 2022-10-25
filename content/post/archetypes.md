---
title: Proceso de carga de una pagina web
description: Proceso de comunicación cliente/Servidor
date: "2019-05-02T19:25:30+02:00"
publishDate: "2019-05-02T19:25:30+02:00"
---

Aquí encontrarás una breve explicación del   `Proceso de comunicación cliente/Servidor`.

<!--more-->





+ El usuario introduce la URI del servidor que quiere visitar.
+ El Router NAT y realiza una solicitud al servidor DNS que está configurado.
+ El servidor DNS busca en los registros y si no lo encuentra, escala la solicitud a servidores DNS primarios hasta encontrarlo
+ El servidor DNS se encarga de devolver el registro al router del usuario. 
+ Se devuelve el registro al router para realiazr el NAT y devolverlo al ordenador del usuario.
+ El ordenador realiza la solicitud a la IP, que le ha devuelto el servidor DNS.
+ El router cliente realiza la solicitud al servidor web.
+ El servidor atiende a la solicitud mediante el siguiente orden de prioridad:

Protocolo --> Dominio --> Puerto --> Ruta --> Parámetros

