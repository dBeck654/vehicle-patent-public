# vehicle-patent-public

**vehicle-patent-public** es un servicio para buscar información de un vehículo a partir de su patente, utilizando la API de GetAPI.

## Enlace de la API

- [GetAPI - Búsqueda por patente](https://www.getapi.cl/patente/)

## Ejemplo de Uso

A continuación, un ejemplo de cómo hacer una solicitud `GET` a la API para obtener información de un vehículo por su patente:

<pre>
<code>
curl --request GET \
  --url https://chile.getapi.cl/v1/vehicles/plate/SGXR50 \
  --header 'accept: application/json'
</code>
</pre>

## Descripción

Este servicio permite obtener datos detallados de un vehículo utilizando su número de patente. Es útil para integraciones en aplicaciones que requieran acceder a información vehicular, como registros automotrices, consultas de historial, o verificación de vehículos.
