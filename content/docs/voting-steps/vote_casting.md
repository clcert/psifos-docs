---
title: "Envío de Votos"
slug: vote-casting
description: ""
summary: ""
date: 2023-09-07T16:04:48+02:00
lastmod: 2023-09-07T16:04:48+02:00
draft: false
weight: 220
toc: true
seo:
  title: "" # custom title (optional)
  description: "" # custom description (recommended)
  canonical: "" # custom canonical URL (optional)
  noindex: false # false (default) or true
---

## Apertura de Elección

Para poder abrir la elección, es necesario que se haya completado
el proceso de Configuración y Creación de Claves. La apertura de la
elección se realiza de manera manual por parte del administrador
del sistema. Una vez abierta la elección, los votantes que se
encuentran en el padrón de la elección podrán ingresar y realizar
sus respectivos sufragios.

## Procedimiento de Votación

Cada votante, mientras esté abierta la elección, podrá ingresar al
enlace correspondiente de la elección, para poder enviar su sufragio.
Los votantes podrán ingresar a votar las veces que ellos estimen necesario
durante la jornada, pero solamente se contabilizará el último voto
emitido.

El Procedimiento de Votación que deberá realizar cada votante es el
siguiente:

1. Al entrar al enlace de votación, deberán ingresar sus credenciales
   en el sitio de autentificación. Una vez validadas las credenciales, el
   sistema verificará si dicha persona está habilitada, o no, para votar.
   Si está habilitada, se le redirigirá a la Cabina de Votación. En cambio,
   si no lo está, a la persona le aparecerá un mensaje de que no está
   habilitada para votar, y se desplegarán los puntos de contacto de la
   Mesa de Ayuda, para que pueda resolver alguna duda sobre su designación.
2. Dentro de la Cabina de Votación, lo primero que deberá realizar el
   votante será la Selección de preferencias. Por cada pregunta en la elección,
   el votante deberá seleccionar la(s) preferencia(s) que desee escoger. Si 
   la votación lo requiere, el
   sistema ofrece la opción de agregar las opciones "Voto Blanco" y
   "Voto Nulo", las cuáles aparecerán de manera explícita entre las opciones
   disponibles.
3. Luego de seleccionar las preferencias, el sistema, utilizando la
   clave públcia de la elección, va a _encriptar el voto_, es decir, va a
   transformar las preferencias seleccionadas, de tal manera, que ninguna persona
   pueda conocerlas (manteniendo así el secreto del voto).
4. Una vez que finalice el proceso de _encriptación_, el votante deberá
   realizar la Revisión de preferencias. El sistema le mostrará las preferencias
   seleccionadas al votante, y le permitirá cambiar las respuestas, si así lo desee.
   Si elige cambiar una respuesta, el sistema lo deriviará nuevamente al paso de
   Selección de preferencias, y deberá _reencriptar_ el voto.
5. Al estar conforme con las preferencias seleccionadas, el votante enviará
   su _voto encriptado_ al servidor. Una vez que el servidor verifique que el voto
   enviado (que sigue siendo secreto) es válido, le desplegará un mensaje al
   votante informándole que el voto fue recibido correctamente y que el proceso
   de votación ha finalizado correctamente. El sistema le permitirá al votante
   poder descargar un Certificado de Votación, que acredita que el servidor
   recibió éxitosamente el voto encriptado enviado por el votante. Este
   certificado no revela las preferencias seleccionadas por el votante.

### ¿Quiéres saber más?

Además de la encriptación realizada, los votos van acompañados de una
demostración de correctitud llamada _Zero-Knowledge Proof (ZKP)_. Para
conocer los detalles de ambos procesos criptográficos puedes revisar
la sección Criptografía.

## Almacenamiento de Votos Encriptados

A lo largo de la jornada de elección, el servidor irá recibiendo cada uno
de los votos enviados por los votantes, y se almacenarán los votos encriptados
en el servidor. Es decir, ni el servidor, ni niguna persona, puede conocer
el contenido de esos votos.

Los votos encriptados son desplegados de manera pública en la Urna Electrónica.
La Urna Electrónica es una sección del Portal de Información, donde se muestran
cada uno de los votos encriptados recibidos por el servidor. Cada votante puede
verificar, en cualquier momento de la jornada electoral, que su voto
encriptado enviado se encuentra almacenado en la Urna Electrónica. Si un voto
está desplegado en la Urna Electrónica, entonces deberá ser contabilizado al
momento de realizar el escrutinio de la elección.
