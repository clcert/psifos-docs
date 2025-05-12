---
title: "Tipos de Votación"
slug: election-types
description: ""
summary: ""
date: 2023-09-07T16:04:48+02:00
lastmod: 2023-09-07T16:04:48+02:00
draft: false
weight: 101
toc: true
seo:
  title: "" # custom title (optional)
  description: "" # custom description (recommended)
  canonical: "" # custom canonical URL (optional)
  noindex: false # false (default) or true
---
En la plataforma existen 3 tipos de votación, que se diferencian con respecto 
a la manera matemática en que son contados los votos, como en la manera que se 
presentan en la interfaz del votante.
**1. Votación Simple:** en una Votación Simple, los votantes pueden escoger m opciones de n candidaturas 
disponibles. Se le llama Votación Simple debido a que solamente admite una 
cantidad limitada de candidaturas (aprox. 12 candidaturas máximo). Este tipo de 
votación utiliza conteo vía Suma Homomórfica, lo que limita la cantidad máxima de 
candidaturas posibles. 

**2. Votación Masiva:** en una Votación Masiva, de misma manera que la Votación Simple, 
los votantes pueden escoger m opciones de n candidaturas disponibles, pero no 
existe límite máximo para el número de candidaturas. Este tipo de votación utiliza 
conteo vía Mixnet, lo que permite quitar el límite máximo de candidaturas. La 
interfaz de votación también es distinta a la Votación Simple, ya que al 
haber un número grande de opciones, es necesario agregar un buscador y una 
lista desplegable para no colapsar la interfaz, y así facilitarle la labor al 
votante.

**3. Votación por Ranking:** en la Votación por Ranking, los votantes deben enviar 
un orden de las candidaturas disponibles. No es necesario que sea un orden 
total, ya que pueden rankear solamente un subconjunto de las candidaturas 
disponibles. El conteo también se realiza vía Mixnet, y por el momento, está 
implementado solamente el algoritmo *Single Transferable Vote (STV)*.