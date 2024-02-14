# Proyecto Full Stack

## FrontEnd

Esta enfocada en la interacción con el usuario, el objetivo es presentar información util, definir visualizaciones y gestionar las interacciones con la aplicación

### Tecnologias comunes

El frontend viene acompañado de tecnologias especificas que solo sirves para el desarrollo del front, agrupadas en 4 categorias:

- **Lenguaje:** Sintaxis de codigo que pueden ser ejecudadas por una computador, tales como JavaScript, TypeScript, Python entre otros...
- **Frameworks:** Grupo de herramientas que ofrecen una estructura de trabaja para poder desarrollar software, simplificando el desarrollo al ofrecer soluciones, encontramos a Angular, Vue, etc.
- **Librerias:**: No nos proporciona una estructura general de la aplicación, si no que nos ofrece herramienta especificas, podemos encontrar JQuery o React.
- **Preprocesadores:** Facilitan la estructura de estilos y diseño de nuestra aplicación, resaltando Sass y Less.

## BackEnd

Es la encargada de la logica, gestiona la funcionalidad de la página y la gestión de bases de datos. Hace posible que una aplicación funcones correctamente, manipulando y disponiendo de la información necesaria.

### Tecnologias comunes

De la misma manera del frontend encontramos herramientas especificas para poder desarrollar funcionalidades en esta parte de la aplicación:

- **Entorno de ejecución:** Incluyen servicios y recursos que permiten la ejecución de programas y aplicaciones. Donde podemos encotrar a Node, Deno y Bun.
- **Framework:** Igual que en el lado del frontend tambien podemos encontrarlos de este lado de la aplicación donde los más destacados son Express, Koa y NestJS.
- **ORMS:** Herramientas que facilitan la comunicación entre bases de datos y los lenguajes de programación. Dentro de los más destacados podemos encotrar a Mongoose, TypeORM, sequelize y Prisma.


## API

Una API **(Application Programming Interface)** define las reglas y protocolos que permiten la comunicación entre dos sistemas, independiente de las tecnologias utilizadas.Es una forma de estructurar el codigo para estandarizar la comunicación entre dos o más sistemas.

```
Las APIs dictac como debe realizarse la solicitud de información de un cliente a un servidor, y come este debera estructuras la respuestas.
```

Las APIs pueden seguir distintos patrones y diseños dependiendo de las necesidades que detecte el equipo de desarrollo, Veremos uno de ellos:

### API Restful
El patron Restful es un estilo para diseñar una API. Se basa en principios fundamentales, simplicidad y escalabilidad de la API. Los pricipios de las API Restful:

- **Recursos:** Todo es considerado como un recurso que puede ser cualquier información que tenga sentido para el sistema.
- **Operaciones CRUD:** Se definen las operaciones CRUD en el sistema para interactuar con los recursos.
- **Estado Representacional:** El recurso que se tranfiere entre cliente y servidor es comunmente un archivo formato JSON o XML.
- **Identificadores unicos:** Cada recurso tiene un identificador unico **(URI)** para poder acceder y manipular recursos especificos
- **Sin estado:** La comunicacion entre ambos sistemas es sin estado, lo que significa que cada solicitud del cliente al servidor contiene toda la información necesario para entender y procesar la solicitud


## Protocolo HTTP
Es el protocolo de comunicación entre el cliente y el servidor. Es el principal protocolo para transferencia de información en internet, opera sobre el conjunto de protocolos TCP/IP.


### Protocolo de red
Entorno donde las computadoras comparten recursos e información utilizando protocolos que facilitan la comunicación entre ellas.

Se creo un modelo llamado OSI, permite que estos protocolos de comunicación se organicen segun su funcionalidad

### Metodos HTTP
El protocolo HTTP define un status del proceso que vamos a procesar en el servidor, estos son llamados Métodos HTTP:

- **GET:** Utilizado para obtener información de un recurso, corresponde a la operación *Read*
- **POST:** Se utiliza para enviar datos al servidor y crear un nuevo recurso, corresponde a la operación *Create*
- **PUT:** Se utiliza para enviar datos al servidor para actualizar un recurso, corresponde al metodo *Update*
- **DELETE:** Se utiliza para solicitar al servidor que elimine un recurso, Corresponde a la operación *Delete*
