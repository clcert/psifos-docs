---
title: "Envío de Desencriptaciones Parciales"
description: ""
summary: ""
date: 2023-09-07T16:04:48+02:00
lastmod: 2023-09-07T16:04:48+02:00
draft: false
weight: 240
toc: true
seo:
  title: "" # custom title (optional)
  description: "" # custom description (recommended)
  canonical: "" # custom canonical URL (optional)
  noindex: false # false (default) or true
---

## Cálculo de Desencriptación Parcial

Al momento de terminar el cálculo del precómputo, cada Custodio de
Clave puede calcular y enviar su desencriptación parcial.

Cada Custodio de Clave debe entrar al enlace del Portal de Custodio de
Clave. Luego de autentificarse y validar su identidad, el sistema
le dará la opción de enviar su desencriptación parcial. Para
poder calcular la desencriptación parcial, debe utilizar el
archivo que contiene su clave privada, el cual fue creado durante
la Ceremonia de Creación de Claves. Una vez validada su clave
privada, el sistema va a calcular la desencriptación parcial,
la cual se calcula sobre el precómputo de la elección. Luego de
calcular la desencriptación parcial, ese valor es enviado al servidor.
Con esto, finaliza la labor del Custodio de Clave en la respectiva
elección.

Cada Custodio de Clave debe enviar su respectiva desencriptación
parcial para poder gatillar el escrutinio de la elección, y poder
conocer el resultado final.

### ¿Quiéres saber más?

El proceso de cálculo, envío y combinación de desencriptaciones parciales se basa
en el algoritmo de *Distributed Key Generation (DKG)*, del cual puedes
conocer más en la sección Criptografía.
