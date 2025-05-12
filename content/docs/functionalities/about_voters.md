---
title: "Caracterización de Votantes"
slug: about-voters
description: ""
summary: ""
date: 2023-09-07T16:04:48+02:00
lastmod: 2023-09-07T16:04:48+02:00
draft: false
weight: 104
toc: true
seo:
  title: "" # custom title (optional)
  description: "" # custom description (recommended)
  canonical: "" # custom canonical URL (optional)
  noindex: false # false (default) or true
---
La lista de votantes habilitados para votar se denomina padrón o 
claustro electoral. El sistema UParticipa requiere los siguientes 
datos de los votantes al momento de subir la lista a la plataforma: 
- Nombre de usuario en el portal de autentificación utilizado
- Nombre completo
- Ponderación
- Grupo (por defecto, sin grupo)

*Observaciones:* 
- Si todos los votantes tienen la misma ponderación, 
entonces se establece que todos los votantes tienen ponderación igual 
a 1.
- El grupo al que pertenece cada votante se utiliza para, al momento 
de calcular los resultados finales, calcular resultados segregados 
por grupo. De esta manera, además de conocer el resultado total, es 
posible conocer el resultado por grupo. Por ejemplo, se puede utilizar
como grupo la facultad o estamento al que pertenece cada votante. Solo 
se admite un grupo por votante.
- Está en desarrollo agregar categorías a las que pertenezca cada votante, 
que permita tener información detallada de participación por categoría. 
Por ejemplo, categorías referente al género, grupo etario o nivel socioeconómico. 
