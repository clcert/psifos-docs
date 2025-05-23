---
title: "Verificación de la Elección"
slug: election-verification
description: ""
summary: ""
date: 2023-09-07T16:04:48+02:00
lastmod: 2023-09-07T16:04:48+02:00
draft: false
weight: 260
toc: true
seo:
  title: "" # custom title (optional)
  description: "" # custom description (recommended)
  canonical: "" # custom canonical URL (optional)
  noindex: false # false (default) or true
---

Una vez finalizada la elección, se habilita el proceso de verificación
de la elección, donde cualquier persona puede correr el software que
revisa que todos los valores fueron calculados correctamente, y convencerse
de que el resultado de la elección es el correcto, y que se condice con
cada uno de los votos enviados.

En el Portal de Información se encuentran las instrucciones necesarias
para poder verificar una elección. Actualmente, solamente existe un método
de verificación, que consiste en descargar un programa que lee los datos
de la elección y verifica todas las propiedades necesarias.

### Script de Verificación

El programa que lee el archivo de verificación realiza las siguientes verificaciones:
- Revisa las pruebas en cada uno de los votos encriptados recibidos.
- Revisa que todos los votos encriptados están asociados a un votante específico 
del padrón.
- Realiza un precómputo con la información pública, y chequea las pruebas 
enviadas por cada custodio de clave.
- Realiza una combinación de las desencriptaciones parciales, y chequea
que el resultado publicado es consistente y correcto.
