# vehicle-patent-public

**vehicle-patent-public** es un servicio para buscar información de un vehículo a partir de su patente, utilizando la API de GetAPI.

## Enlace de la API

- [GetAPI - Búsqueda por patente](https://www.getapi.cl/patente/)

## Ejemplo de Uso

A continuación, un ejemplo de cómo hacer una solicitud `GET` a la API para obtener la tasación de un vehículo por su patente:

<pre>
<code>
curl --request GET \
  --url https://chile.getapi.cl/v1/vehicles/plate/SGXR50 \
  --header 'accept: application/json'
</code>
</pre>

## Descripción

Este servicio permite obtener datos detallados de un vehículo utilizando su número de patente. Es útil para integraciones en aplicaciones que requieran acceder a información vehicular, como registros automotrices, consultas de historial, o verificación de vehículos.

# Tasación

**tasación** Consulta la tasación de un vehículo sólo con su patente.

## Enlace de la API

- [Tasación](https://getapi.cl/tasacion/)

## Ejemplo de Uso

A continuación, un ejemplo de cómo hacer una solicitud `GET` a la API para obtener la tasación de un vehículo por su patente:

<pre>
<code>
curl --request GET \
  --url https://chile.getapi.cl/v1/vehicles/appraisal/${patente} \
  --header 'accept: application/json'
</code>
</pre>

## Descripción
Esta API cuenta con ratelimit para la version gratis de 5 consultas por dia.

Parametros que podras obtener:
* precio usado
* precio retoma
* información fiscal
* color
* tipo de bencina
* marca
* modelo
* otros
