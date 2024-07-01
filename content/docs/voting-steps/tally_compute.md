---
title: "Cierre de Elección"
slug: tally-computing
description: ""
summary: ""
date: 2023-09-07T16:04:48+02:00
lastmod: 2023-09-07T16:04:48+02:00
draft: false
weight: 230
toc: true
seo:
  title: "" # custom title (optional)
  description: "" # custom description (recommended)
  canonical: "" # custom canonical URL (optional)
  noindex: false # false (default) or true
---

El cierre de la elección, al igual que la apertura, es un proceso
que se debe realizar de manera manual por parte del administrador. Una
vez que se cierra la elección, no se reciben más votos. Eso sí, el
Portal de Información aún está disponible para ser accedido.

Luego de cerrar la elección, es posible hacer modificaciones al
padrón electoral, en particular, a las ponderaciones de cada voto
recibido, ya que pueden existir instancias donde dicha ponderación
se deba modificar, en relación al total de votos recibidos durante
la jornada. También, es posible deshabilitar algunos votos recibidos,
pensando en el caso que se esté realizando una votación híbrida (modo
presencial y remoto), donde el voto presencial tiene mayor prioridad.

## Cálculo de Precómputo

Una vez que se hayan realizados las modificaciones necesarias, el sistema
calcula el precómputo (tally) de la elección. La manera de calcular
el precómputo varía dependiendo del tipo de votación que se esté realizando.
Por el momento, existen dos maneras de realizar este cálculo: (1) a través
de una suma homomórfica, y (2) utilizando una Mixnet. Ambos métodos
utilizan la totalidad de los votos encriptados que serán considerados para
realizar el escrutinio de la elección.

### ¿Quiéres saber más?

Ambos métodos mencionados para calcular el precómputo (suma homomórfica y Mixnet),
son herramientas criptográficas que permiten poder calcular el total, y
al mismo tiempo, mantener en secreto los votos emitidos, además de proveer
una demostración de la correctitud de este proceso. De esto puedes encontrar
más detalles en la sección Criptografía.
