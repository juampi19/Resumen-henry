# EXPRESS

## Estructura basica de servidor
- **Host y puerto:** El localhost es un ubicador de un recuros en la red, puede ser una dirección IP o un nombre de dominio.
El host indica donde se encuentra el servidor que aloja la aplicación.
El puerto, es como una puerte especifica en el servidor, para distingir tu aplicacion de los diferentes servicios que ahí en el host

- **Controladores:** Encargados de recibir la consulta y dar la respuesta al cliente

- **Servicios:** Tiene su propia responsabilidad en la aplicación como solicitudes de usuario, autenticación, interacción con la base de datos

- **Middlewares:** Dentro de un servicio podemos encotrar esto , por ejemplo mandar una seria de datos al cliente de una forma distinta como esta en la base de datos

## Scaffolding de proyecto
Una de las caracteristicas de express es su flexibilidad para la estructura de carpetas.
Nos enfocaremos en dar forma nuestro proyecto a través del scaffolding. Estructura que se basara en la creación de 3 carpetas

- Rutas

- Controladores

- Servicios

### Variante de enfoque
Existen variantes de como estructurar carpetas y archivos en nuestros proyectos

- Enfoque funcional: Organizacion las carpetas que representan caracteristicas especificas del proyecto. Las carpetas representan una caracteristica principal de la aplicacion y dentro se encuentras sus rutas, controladores y servicios-

- Enfoque Modular: Las carpetas estas organizadas por roles, rutas, controladores y servicios.


## Creación del servidor

+ ¿Por qué aprender express?

- Facilita el manejo de rutas: Simplifica y gestiona la creacion de rutas, permitiéndonos organizar nuestro código de forma más organizada

- Middleware para funcionalidades adicionales: Nos brinda una forma de incorporar funciones adicionales a nuestras rutas, como la autentificacion o gestion de errores

- Ahorro de tiempo con middleware integrados: trabaja con estos middleware para el manejo de sesiones, cookies

- Amplia comunidad y documentación: Uno de los framework web más populares para Node.js. Tiene una amplia comunidad y una documentación solida

- Escalabilidad y flexibilidad: A medida que nuestro proyecto crecen, nos brinda la flexibilidad y escalibilidad para desarrollar nuestra aplicación de modo eficiente.


## Controladores

Un controlador es una funcion que maneja las solicitudes  HTTP, lleva la logica necesaria y envia una respuesta al cliente, los controladores están ligados a una o mas rutas.

- Procesamiento de datos: Un controlador puede procesar datos de la solicitud.

- Interaccion con modelos: Puede interactuar con los modelos para hacer las operaciones a la base de datos.

- Generacion de respuesta: Crea y envia la respuesta al cliente como html, JSON u otro formato.

- Manejo de errores: Puede contener logica para el manejo de errores y enviar las respues adecuadas.

- Redirecciones: Puede redirigir a otras rutas o URL

## Enrutado
Componenete en express encargado de gestionar las rutas de nuestra aplicación dirigiendolos hacia el controlador especifico para entregar la respuesta.

- Enrutado: creamos el enrutado utilizando express.Routes(), encargado de manejar las rutas.

- Rutas: asociamos una ruta especifica con un metodo HTTP y su controlador correspondiente.

- Enrutador principal: Agregamos la rutas hijas el enrutador principal

- req y res: abreviaturas de request y response. Request contiene la informacion de la solicitud del cliente y response la respuesta del servidor.

- Send: Metodo de respuesta para enviar al cliente.

- express.Router(): El enrutador de express, utilizado para definir las rutas y middleware.

- Numero de rutas y metodos HTTP: se pueden crear tantas rutas como necesitemos y pueden utilizar los distintos metodos HTTP vistos anteriormente.
