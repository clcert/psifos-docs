---
title: "Medidas Anti Coerción"
slug: anti-coercion
description: ""
summary: ""
date: 2023-09-07T16:04:48+02:00
lastmod: 2023-09-07T16:04:48+02:00
draft: false
weight: 103
toc: true
seo:
  title: "" # custom title (optional)
  description: "" # custom description (recommended)
  canonical: "" # custom canonical URL (optional)
  noindex: false # false (default) or true
---
La coerción tiene relación con una presión que se ejerce sobre 
una persona para votar por alguna opción en contra de su 
voluntad, o bien, para que revele su opción escogida. Todos 
los sistemas de votación remotos sufren de posibilidad de coerción, 
ya que no existe una manera en que la autoridad electoral 
pueda asegurar que los votantes realizan su votación 
en un entorno seguro. 

Existen sistemas que poseen la propiedad de ser resistentes a la 
coerción. Por lo general, estos sistemas incorporan mecanismos 
para que los votantes puedan emitir "votos falsos", lo que 
les permite realizar su votación real en un momento que no 
estén recibiendo la presión indebida. Esto implica, en la 
gran mayoría de los casos, problemas de usabilidad y dificultad 
para poder realizar el sufragio.

UParticipa ha adoptado un mecanismo que es heredado del sistema 
Helios. En UParticipa es posible votar más de una vez. Cada vez 
que un voto nuevo es emitido, este voto *reemplaza* al voto enviado 
anteriormente. De esta manera, solamente se contabilizará el 
último voto enviado por cada votante. Esta es una medida de 
mitigación frente a la coerción. Además, este mecanismo le permite 
a los votantes rectificar su votación, si es que llegara a 
suceder de que envió su voto de manera equivocada.
