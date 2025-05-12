---
title: "Autentificación Externa"
slug: external-auth
description: ""
summary: ""
date: 2023-09-07T16:04:48+02:00
lastmod: 2023-09-07T16:04:48+02:00
draft: false
weight: 105
toc: true
seo:
  title: "" # custom title (optional)
  description: "" # custom description (recommended)
  canonical: "" # custom canonical URL (optional)
  noindex: false # false (default) or true
---
El sistema UParticipa opera únicamente con un servidor 
externo de autentificación de votantes. Esto se basa en 
un paradigma de separación de responsabilidades. De 
esta manera, se asegura que la autentificación de los 
votantes se realiza por un servicio aparte del servidor 
que recibe y procesa los votos. 

Para realizar el proceso de autentificación, UParticipa 
está implementado para ser un cliente del protocolo 
(OpenID Connect)[https://openid.net/]. Por lo tanto, es 
necesario que el servidor de autentificación esté implementado 
como un servidor de OIDC. El sistema posee la capacidad 
de utilizar Google como servidor de autentificación.

El proceso de autentificación opera anteriormente al 
proceso de revisión de si el votante está habilitado (o no) 
para votar. 
