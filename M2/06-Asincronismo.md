# Asincronismo

## Peticiones HTTP desde el navegador
Es un protocolo de comunicacion entre un cliente y un servidor, HTTP solo establece las reglas como se dara la comunicación.

### Cliente y Servidor
Siempre que hacemos una solicitud a una pagina web, es una solicitud bajo el protocolo http, el navegador seria el cliente, y el servidor es quien recibe esta solicitud y responde al cliente con la informacion solicitada

### API Testing tools
Existen herramientas para realizar solicitudes HTTPa un servidor, para determinar que las respuestas funcionen correctamente

## Operaciones Asincronicas

### ¿Qué es?
Son aquellas en las que el script no espera a que una tarea se complete antes de pasar a la siguiente, no bloqueando la ejecución del código.
Javascript cuanta con distintas herramientas que le permiten dejar de lado su naturaleza sincrona.
- Callback
- Promesas
- Async/Await

## Promesas

En javascript una promesa son estructura de datos, que representa el resultado eventual de una operacion asincronica. Dicha respues puede ser exitoxa o ser un fracaso.

Una promesa va a reservar un lugar en mi código para una accion que aun no ocurre, pero una vez ocurra el código sabra que hacer.

Para crear una promesa debemos utilizas una estructura llamada Promise e instanciarla con la palabra clave new.

### Estados de una promesa
- **Pending:** Corresponde al estado inicial de una promesa, todas las promesas mantienen este estado hasta que se ejecute la operación asincronica.

- **Fulfilled:** Una vez se complete la operacion y sea exitosa la promesa se resuelve y el estado cambia a 'fulfilled'.

- **Rejected:** En caso de fallar al operacion, la promesa se rechaza y el estado cambia a 'rejected'

Para poder manejar el valor al que se resuelve o rechaza un promesa, usamos dos metodos:

- **THEN:** Maneja la logica en caso que una promesa se haya resuelto. Recibiendo una función con el valor de la resolución, ejecutandose cuando la promesa se complete.

- **CATHC:** Maneja la logica en caso que una promesa sea rechazada.Recibe una función con la razón del rechazo de la promesa.

## ASYNC AWAIT

### ¿Qué es?
Caracteristica de javascript para simplificar el código asincrono, viene a reemplaza las promesas, evitando la encadenacion de metodos como then y catch.

La funcion debe anteponer la palabra clave **async** y dentro del bloque accedemos a el operador especial **await**

### Try/Catch
Para el manejo de errores al utilizar async/await, este bloque se utiliza para capturar y manejar los errores que podrian ocurrir
- **TRY:** Código que queremos ejecutar
- **CATCH:** En caso de ocurrir algun error ejecutamos el bloque catch

## AXIOS

Asi como fetch, axios es utilizado para realizar solicitudes HTTP en javascript de forma mucho mas simple.

- Sintaxis simple y consistencia: Proporciona una escritura simple para realizar solicitudes
- Manejo de promesas: Axios esta basodo en promesas, lo que facilita su integración con async/await

Algunos de los metodos:
- axios.get(url) o axios(url): Realiza una solicitud tipo GET permitiendo obtener los datos de una API.

- axios.post(url): Ejecuta una solicitud tipo POST, permitiendo enviar datos en el cuerpo de la solicitud.

- axios.put(url): Ejecuta una solicitud PUT para enviar datos al servidor y actualizar un recurso existente.

-axios.delete(url): Ejecuta una solicitud DELETE para eleminar un recurso existente

## Operaciones de naturaleza asincrona

Otras de las operaciones asincronas que podemos encontrar en javascript, es trabajar con archivos con la herramiente file system

### File System
El module fs es nativo de node y facilita la interaccion con el sistema de archivos de un dispositivo, que nos permite realizar operaciones como leer, escribir y eliminar archivos


## Debugging

Existen tres formas en las que pueden presentar un error en nuestro codigo

- Explicito: Lo podemos ver en la terminar, por ejemplo un error de sintaxis.

- Resultados inesperado: Nuestro codigo funciona correctamente. Ya qeu el error se encuentra en la lógica.

- Sin resultados: Casos en donde no tenemos un error explicito y tampoco un resultado inesperado