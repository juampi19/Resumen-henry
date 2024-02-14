# Asincronismo

## ¿Qué es?

En los años 2000 la forma de programar cambio, las aplicaciones que antes estaban unicamente de forma local en el dispositivo, ahora deben contemplat la posibilidad de enviar y recibir informacion de manera remota entre cliente y servidor.
Este proceso requiere de un manejo de procesos asincronicos

- **Sincronismo:** Las tareas que lleva un dispositivo se ejecutan de forma secuencial, es decir, un proceso detras de otro. Javascript es sincronico por naturaleza

- **Asincronismo:** La capacidad de un lenguaje de realizar operaciones mientras una operacion se ejecuta en segundo plano

El objetivo del asincronismo es mejorar la eficiencia y capacidad de un programa, evitando codigo bloqueante

### Manejo de asincronismo en Javascript

Javascript es de naturaleza sincrona, pero podemos darle un comportamiento asincrono mediante el uso de algunas herramientas
- Callbacks
- Promesas
-Async/Await


## AJAX

Debido a la necesidad de manejar solicitudes y respuesta en el manejo de informacion, se implemento una tecnica de desarrollo denominada AJAX(Asynchronous Javascript and XML).

XML son las siglas de **extensible markup language** es un lenguaje de marcado similar a HTML, usado para el intercambio de informacion

AJAX se utiliza para darle funcionalidad y permitir interaccion en una página web, permitiendo realizar procesos sincronos.

```
¡AJAX NO es una tecnología por sí misma! Es un término que describe un modo de utilizar varias tecnologías existentes, incluyendo HTML, DOM, CSS, JavaScript, XML y el objeto XMLHttpRequest, del cual hablaremos más adelante.
```

Otro formato para realizar en intercambio de datos es JSON **Javascript Object Notation** como los objetos en javascript

Las aplicaciones web tradicionales solian requerir una recarga completa de la pagina para realizar una solicitud, AJAX permite enviar y recibir datos del servidor en segundo plano, sin interferir con el usuario en la página mejorando su experiencia.


Ahora es momento de realizar una solicitud AJAX utilizando el signo $ que nos proporciona JQuery. Es importante mencionar que este signo nos proporciona las funcionalidades necesarias para realizar peticiones asíncronas desde nuestro código, en este caso, utilizando el método GET


## Callbacks

Son funciones que se pasan como argumentos a otras funciones, ejecutandose despues de que se complete alguna operación.



### Conclusion

Hemos comprendido el proceso fundamental para el intercambio de información dentro de una página y trabajar solicitudes asincronicas en javascript

- Asincronismo: Tareas que no bloquean el flujo principal de la aplicación.

- AJAX: Tecnica para realizar solicitudes asincronicas desde un navegador sin recargar la pagina, mejorando la experiencia del usuario.

- Callbacks: funciones que se pasan como argumento de otra funcion y se ejecutan despues de que se complete alguna operacion