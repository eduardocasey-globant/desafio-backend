# Desafio para desarrollador Backend

## Objetivo del desafío

1. Resolver una situación desconocida desde un enfoque algorítmico.
2. Publicar la solución através de una API REST.
3. Publicar solución a través de socket.io.
4. Plantear una solución que contenga pruebas.
5. Utilizar ecosistema Node.js
6. Mandar el link al repo en github con la resolución por mail y __no crear__ un PR a este repo.

## Pedido del cliente
Mengenlehreuhr Inc. creadores del reloj [Berlin Clock](https://en.wikipedia.org/wiki/Mengenlehreuhr) necesita brindar los siguientes servicios:

1. Conocer el horario actual, pero expresandolo en el formato *Berlin Clock*
2. Dado un horario expresado en format [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) conocer su correspondiente *Berlin Clock*

Para llevar a cabo esta tarea necesitarían definir un formato estructurado de respuesta (JSON). Adicionalmente la empresa Mengenlehreuhr Inc. valorará que este servicio cuente con end-points en los cuales se puedan consultar estos horarios obteniendo una representación gráfica.  **_Esta última característica es opcional_**

## Objetivo técnico del desafío

Construir una servicio REST que permita:

1. Consultar la hora actual, 
2. Convertir un horario expresado en formato ISO 8601.

En ambos casos respondiendo un json o una imagen (renderizar la imagen es **opcional**) generada por el servidor. 

Queda a juicio del postulante como estructurar los datos así como también como renderizar la imagen.

El cliente requiere que esta funcionalidad este testeada con una cobertura que permita garantizar una calidad que se considere prudente.

### Bonus track 1

**Generar un endpoint de socket.io** que pushea el horario actual cada `n` segundos a una app conectado por socket.io. El cliente reconoce que eso es un 'nice to have' y tecnicamente no tiene mucho sentido, pero quiere ser parte del ilustre *realtime web*. 

### Bonus track 2

**Generar una imagen docker** y registrarla en [DockerRegistry](https://hub.docker.com/) de forma publica para poder desplegar el servicio (el despliegue queda a cargo de la empresa).


## Tips

1. Para crear el servicio REST es conveniente [RESTify](http://restify.com/) si bien se puede utilizar [Express](https://expressjs.com/)
2. Para escribir las pruebas [Mocha](https://mochajs.org/)
