---
title: Proceso de carga de una pagina web
description: Proceso de comunicación cliente/Servidor
date: "2019-05-02T19:25:30+02:00"
publishDate: "2019-05-02T19:25:30+02:00"
---

Aquí encontrarás una breve explicación del   `Proceso de comunicación cliente/Servidor`.

<!--more-->


PC CLIENTE introduce la URI del servidor que quiere visitar

PC CLIENTE manda solicitud al NAT del ROUTER CLIENTE

ROUTER CLIENTE hace NAT y realiza una solicitud al SERVIDOR DNS que esta configurado

SERVIDOR DNS busca en los registros y si no lo encuentra en sus registros, escala la solicitud a servidores DNS primarios hasta encontrarlo

El SERVIDOR DNS se encarga de devolver el registro al ROUTER CLIENTE (Este registro ha podido ser encontrado en el mismo servidor o puede ser el que le han devuelto los otros servidores DNS).

Se devuelve el registro al ROUTER CLIENTE.

El ROUTER CLIENTE realiza el NAT y se lo devuelve al PC CLIENTE.

El PC CLIENTE realiza la solicitud a la IP, que le ha devuelto el Servidor DNS, correspondiente al servidor del recurso solicitado.

Se vuelve a mandar la solicitud al ROUTER CLIENTE que vuelve a hacer NAT.

El ROUTER CLIENTE realiza la solicitud al SERVIDOR WEB.

El SERVIDOR atiende a la solicitud mediante el siguiente orden de prioridad:

Protocolo
Dominio
Puerto
Ruta
Parámetros

El servidor devuelve el recurso solicitado al ROUTER CLIENTE

El ROUTER CLIENTE vuelve a realizar NAT

El ROUTER CLIENTE devuelve la petición al PC CLIENTE

For example:

```YAML
---
title: title
description: desc
date: "2019-05-02T19:47:09+02:00"
---
```

to

```TOML
+++
title = "title"
description: "desc"
date: "2019-05-02T19:47:09+02:00"
+++
```