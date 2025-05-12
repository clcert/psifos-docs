---
title: "Estadísticas e Información Pública"
slug: public-info
description: ""
summary: ""
date: 2023-09-07T16:04:48+02:00
lastmod: 2023-09-07T16:04:48+02:00
draft: false
weight: 102
toc: true
seo:
  title: "" # custom title (optional)
  description: "" # custom description (recommended)
  canonical: "" # custom canonical URL (optional)
  noindex: false # false (default) or true
---
El sistema despliega información pública, tanto durante el transcurso 
de una elección, denominada "Información En Vivo", y una vez terminada 
la elección a través de un archivo JSON, denominado "Archivo de Verificación".

**1. Información En Vivo:** una vez que la elección es abierta, se disponibiliza 
el **Portal de Información**. Este portal, que está asociado a una elección 
específica, posee las siguientes secciones:
  - **Urna Electrónica:** en la Urna Electrónica se despliegan los votos 
  encriptados que va recibiendo el servidor. Si bien los votos encriptados 
  están asociados a un votante en particular, por simplicidad, la plataforma 
  despliega los votos encriptados de manera anónima. La urna electrónica 
  se va actualizando a medida que el sistema va recibiendo nuevos votos 
  encriptados. Además, si un votante reemplaza su voto, solo se muestra 
  en la urna electrónica el último voto encriptado válido enviado por 
  cada votante.
  - **Estadísticas:** en la sección de Estadísticas se muestra el número 
  de votos recibidos, junto con la tasa de participación respectiva 
  (pestaña de *Participación*). Además, en la pestaña de *Distribución de 
  los votos en el tiempo* se despliegan dos gráficos, con respecto a la hora 
  de llegada de los votos. En uno, se despliega el número de votos recibidos 
  cada cierta ventana de tiempo (30 minutos, 1 hora, 2 horas, 4 horas o 1 día). 
  En el otro, se muestre el número acumulado de votos en esa misma ventaba 
  de tiempo establecido. 
  - **Eventos:** en la sección Eventos se despliegan todos los eventos 
  importantes sucedidos en una elección, los cuales se transparentan 
  a cualquier observador externo. Entre otros eventos, se encuentran: 
  creación de clave pública de los custodios, inicio y cierre de elección, 
  modificaciones al padrón durante la jornada de elección y publicación 
  de los resultados.
  - **Resultados:** una vez publicados los resultados de la elección, estos 
  se despliegan en la sección Resultados, la cual se abre por defecto si 
  se accede al Portal de Información con los resultados ya publicados. Además 
  de mostrar el número de votos recibidos por cada opción, en cada pregunta, 
  se despliega el número total de votos recibidos, la tasa de participación, 
  y la distribución de votos por grupo o ponderación (si corresponde).
  - **Verificación:** en la sección Verificación se muestra un paso a paso 
  de como verificar una elección, una vez que los resultados hayan sido 
  publicados. Además de poder descargar el Archivo de Verificación, se puede 
  descargar el script de verificación, con el objetivo de poder verificar 
  la elección de manera local en el dispositivo del observador externo.

**2. Archivo de Verificación:** el Archivo de Verificación se disponibiliza 
una vez que los resultados de la elección hayan sido publicados. Este archivo 
se encuentra en formato JSON, además de estar codificado en base64, con el objetivo 
de comprimir la información. Este archivo puede ser leído por el script de verificación 
y tiene como objetivo almacenar todos los datos necesarios para que cualquier 
persona pueda convencerse de que el proceso electoral fue desarrollado correctamente, 
y, entre otras cosas, validar el resultado publicado. El archivo de verificación 
contiene las siguientes secciones:
  - Datos generales de la elección.
  - Datos de los votantes.
  - Datos de los votos encriptados recibidos.
  - Datos de la información de los custodios de claves.
  - Datos del resultado de la elección.
