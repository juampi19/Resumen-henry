# Express II

## Servicios
Segmentos especificos de lógica de negocio, a defirencia de los controladores de manejar las solicitudes y respuesta, los servicios se centran en tareas más amplias, desde la autentificación al manejo de bases de datos.


## Middleware
Un middleware es una función que tiene acceso a los objetos:
- REQ: Solicitud
- SEND: Respuesta
- NEXT: Siguiente funcion en el flujo de solicitud y respuesta
Funcion que esta en el medio de tu solicitud y respuesta.

Se pueden dividir en dos categorias principales:
- Pre-built: Componentes listos para user ofreciendo distintas funcionalidades, especificas para cada tarea en express:

 + Morgana: Middleware HTTP para facilitar el seguimiento y detalles de la informacion de las solicitudes, como el metodo HTTP utilizado, ruta solicitada, tiempo que tarda en obtener una respuesta.

 + express.json(): Combierte automaticamente los cuerpos de las solicitudes en formato JSON. En terminos simples convierte los datos JSON enviados en el cuerpo de la solicitus en objetos javascript faciles de manipulas.

 + CORS: Permite o restringe acceeso a recursos, para la seguridad en las solicitudes desde el navegador.

- Personalizados: Funciones que uno mismo crea para el manejo especifico de solicitudes en tu aplicacion, como la manipulación de datos, validar información, entre otros.
Su beneficios son los siguientes:

+ Adaptabilidad: Personaliza la lógica de las solicitudes de acuerdo a los requisitos de tu aplicación.

+ Reutilización de código: Las funciones pueden ser reutilizables en distintas partes de tu aplicacón.

+ Mejora la mantenibilidad: Al tener la lógica de forma separada, el código se vuelve más facil de mantener.


## Validaciones
Las validaciones son esenciales para garantizar la seguridad y eficiencia del sistema.
Al validar los objetos de entrada, puedes verificar que cumpan con las condiciones antes de procesarlas, evitando errores y protegiendo tu aplicación. Brindando una buena experiencia de usuario.

Una de las estrategias para validaciones es utilizar middleware. Creando middleware personalizados para la verificación de datos de entrada para que cumplan con los criterios antes de pasarlo a la logica principal, tambien puedes utilizar middleware pre-construidor que se especializan en validaciones.
