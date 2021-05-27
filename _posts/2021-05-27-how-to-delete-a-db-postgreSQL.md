---
title:  "Cómo elíminar una Base de Datos en PostgreSQL"
header:
  teaser: "/assets/images/500x300.png"
categories: 
  - Data Bases
tags:
  - PostgreSQL
---

La forma mas sencilla es darle click derecho sobre la base de dato en cuestión y darle clic en Delete/Drop y aceptar la operación, y simplemente se va a eliminar.

La otra forma de eliminar es escribiendo el codigo

`drop database if exists "NOMBRE_DB"`

Si nos aparece un error al intentar eliminarla le damos clic derecho a la base de datos en la barra lateral izquierda y desconectamos la base de datos, y luego lo intentamos nuevamente para eliminar.