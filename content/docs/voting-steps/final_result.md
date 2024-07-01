---
title: "Escrutinio de la Elección"
slug: final-result
description: ""
summary: ""
date: 2023-09-07T16:04:48+02:00
lastmod: 2023-09-07T16:04:48+02:00
draft: false
weight: 250
toc: true
seo:
  title: "" # custom title (optional)
  description: "" # custom description (recommended)
  canonical: "" # custom canonical URL (optional)
  noindex: false # false (default) or true
---

## Ceremonia de Escrutinio

La Ceremonia de Escrutinio de la elección se realiza con el
objetivo de transparentar el cálculo del resultado final, procurando
que sea lo más abierta posible, de tal manera que las personas
interesadas en la elección puedan presenciar la publicación
del conteo final. Se recomienda que en la Ceremonia de Escrutinio
estén presentes los miembros de la Junta Electoral, los Custodios
de Clave y los administradores del sistema.

## Combinación de Desencriptaciones Parciales

El sistema permite que no sea necesario contar con todas las desencriptaciones
parciales para poder calcular el resultado final de la elección.
Solamente es necesario contar con un número mayor que el umbral (_threshold_)
establecido al momento de configurar la elección. Se recomienda
que dicho umbral sea la mitad del número de custodios, más uno. Es decir,
si la elección tiene tres (3) Custodios de Clave, se puede calcular
el resultado final con solamente dos (2) desencriptaciones parciales
recibidas. Esta propiedad permite que se pueda calcular el resultado,
a pesar de que un cierto número de Custodios de Clave tenga algún
problema para poder enviar su desencriptación parcial.

Durante la Ceremonia de Escrutinio, se gatilla la combinación de las
desencriptaciones parciales recibidas, con lo cual se obtiene
el resultado final de la elección.

## Publicación de Resultado Final

Una vez combinadas las desencriptaciones parciales, el resultado
final está disponible para que cualquier persona pueda verlos a través
del Portal de Información. Durante la Ceremonia de Escrutinio, se
muestran los resultados finales de la elección realizada. El sistema
despliega el número de votos (ponderados, si fuera el caso) recibidos
por cada una de las candidaturas en carrera.
