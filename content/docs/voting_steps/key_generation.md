---
title: "Generación de Claves"
description: ""
summary: ""
date: 2023-09-07T16:04:48+02:00
lastmod: 2023-09-07T16:04:48+02:00
draft: false
weight: 210
toc: true
seo:
  title: "" # custom title (optional)
  description: "" # custom description (recommended)
  canonical: "" # custom canonical URL (optional)
  noindex: false # false (default) or true
---

Antes de iniciar la elección, es necesario generar las claves
de la elección. Al final del proceso, se generará una **clave
pública**, que será utilizada para poder encriptar los votos,
además de que cada Custodio de Clave contará con una **clave
privada**, la cual deberá utilizar para enviar su
desencriptación parcial al final de la elección.

## Designación de Custodio de Clave

Para cada elección, se deben designar a las personas que cumplan
el rol de Custodio de Clave. Por lo general, se recomienda que se
utilice un número impar y, al menos, tres (3) Custodios de Claves.
Las personas que cumplirán el rol de Custodio de Clave deben tener
independencia unas de otras, ya que se debe minimizar la posibilidad
de colusión entre ellas.

Las personas que sean designadas como Custodio de Clave poseerán la
responsabilidad (en otras palabras, el poder) de preservar, al menos,
dos propiedades inherentes a toda elección: (1) el secreto de los
votos, y (2) el cálculo del resultado final. Si los Custodios de Clave
no operan honesta y correctamente, es posible que las propiedades
antes mencionadas no se cumplan en su totalidad, lo cual es perjudicial
para el desarrollo de un correcto proceso de elección.

## Ceremonia de Creación de Claves

Para poder crear las claves de la elección, es necesario que las personas
que cumplen el rol de Custodio de Clave se reúnan en una Ceremonia de Creación
de Claves, la cual se debe realizar de manera síncrona entre todos los
Custodios, es decir, deben estar presentes al mismo tiempo.

La Ceremonia de Creación de Claves procede de la siguiente manera:
1. Cada Custodio de Clave deberá ingresar al enlace del Portal de
Custodio de Clave de la elección respectiva donde fue asignado.
2. Lo primero que deberá realizar será ingresar
sus credenciales del sitio de autentificación. Una vez validadas sus
credenciales, el sistema verificará si ha sido designado como
Custodio de Clave.
3. Una vez verificada su designación, el sistema le desplegará
la opción de generar su **clave privada**. Esta clave privada consiste
en un archivo `.key` que el Custodio de Clave deberá descargar y
almacenar hasta el escrutinio de la elección.
Ese archivo es *único, personal e intransferible*. Es por ello,
que se recomienda respaldar ese archivo en un dispositivo de almacenamiento
externo. Una vez descargada la clave privada, el sistema le solicitará
que pueda subir esa clave, con el objetivo de verificar que fue correctamente
descargada.
4. Al validar la correctitud de la clave privada, el sistema comienza el
proceso de Sincronización, entre los Custodios de Clave. Este proceso toma
algunos minutos, y tiene el objetivo de que todos los Custodios de Clave
intercambien valores para asegurar el correcto procedimiento de cada uno
de ellos.
5. Una vez finzalizado el proceso de Sincronización, la Ceremonia de Creación
de Claves habrá terminado. El servidor reúne la información enviada por
cada Custodio de Clave, y calculará la **clave pública** de la elección,
la cuál será utilizada para poder *encriptar* los votos, es decir, que
sean secretos.

*Nota: está en proceso de desarrollo una aplicación móvil para Custodios de
Clave, por lo que la Ceremonia de Creación de Claves se modificará una vez
que se lance la aplicación móvil mencionada*

### ¿Quiéres saber más?
El proceso matemático detrás de la Creación de Claves se llama *Distributed
Key Generation (DKG)*, del cual puedes encontrar más referencias en la sección
Criptografía.
