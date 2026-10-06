# api-warsmiks
Nuestro proyecto en API WARS
# POS El Rápido

Caja registradora web para tiendas de barrio que permite registrar una venta
y emitir la factura electrónica DIAN con la API de Factus.

## Equipo Miks

## Tecnologías
- HTML, CSS y JavaScript (página del POS)
- Node.js (servidor)
- API de Factus (ambiente sandbox)

## Cómo correrlo
1. Instala las dependencias: `npm install`
2. Copia el archivo `.env.example` como `.env` y escribe tus llaves de prueba (sandbox) de Factus.
3. Inicia el servidor: `node server.js`
4. Abre en el navegador: http://localhost:3000

## Cómo funciona
1. El vendedor llena los datos del cliente y de la venta en la página.
2. La página calcula el IVA (19 %) y envía la venta al servidor.
3. El servidor se comunica con Factus y crea la factura.
4. La página muestra el número de la factura, la referencia y el código QR.

## Nota de seguridad
Las llaves reales nunca se suben al repositorio. Este proyecto usa solo el
ambiente de pruebas (sandbox) de Factus.
