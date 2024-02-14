## Introducción 

Las bases de datos desempeñan un papel importante en el mundo de la tecnologia, para poder gestionar datos de manera organizada, son la columna vertebral de numerosas aplicaciones y sistemas.


Su importancia radica en la capacidad de entragar grandes volúmenes de información, permitiendo el desarrollo de aplicaciones escalables

- Datos: Representaciones simbolicas de un hecho o concepte, pueden ser numeros, cadenas de texto que se puedan almacenar y ser procesados.

- Información: Cuando los datos se organizan y adquieren un contexto y significado especifico.

- Base de datos: Conjunto organizado de datos para poder gestionarlos de manera eficiente.

El objetivo es poder almacenar datos de manera estructurada, mediante un procesamiento adecuado podriamos obtener información especifica de los datos.

### Entidades y atributos
Entidad represente un objeto o concepto del mundo real que podemos almacenar en la base de datos para poder ser almacenado en una base de datos.
Los atributos describen las caracteristicas especificas de la entidad.

### Normalización de datos
La normalizacion busca organizar la información de manera mas eficiente y reducir la redundancia.Implica dividir las tablas para evitar la repeticion de informacion y garantizar su coherencia.

Las reglas para realizar este proceso esta definida por las formas normales, son niveles de organización de una BDD con reglas especificas a cumplir.


## Persistencia de datos
Nos permite almacenar y recuperar información incluso cuando la app haya terminado su ejecucion o se cierre. Podemos trabajar con distintas formas para persistir datos, como las base de datos que pueden ser relacionales(SQL) o no relacionales(NoSQL). La persistencia nos permite almancenar datos de manera duradera

### Sitemas de archivos y almacenamiento local.

- Sistema de archivos: Utilizada por sistemas operativos para guardar en dispositivos como discos duros, carpetas , archivos, entre otros..

**Ventajas:**
+ Simple de entender y usar.
+ Cada aplicación puede tener su propio archivo de datos.

**Desventajas:**
+ Puede volverse desordenadi si hay muchas aplicaciones
+ No es eficienta para buscar y organizar grandes cantidades de datos

- Localhost: Los navegadores nos ofrecen una herramienta que nos permite tener almacenamiento de forma local y sesiones mediante la API web Storage Native. Permitiendo almacenar datos en el lado del cliente.

**Ventajas:**
+ Facil de utilizar, pocas lineas de código.
+ Más capacidad de almacenaje que otras herramientas del navegador.
+ Seguridad del usuario, ya que no son enviados al servidor.
+ Disponible de forma rápida y accecible de forma sincronica.

**Desventajas:**
+ Puede ser limitado dependiendo del navegador.
+ Capacidad de almacenamiento muy limitada.
+ Al ser sincronico, puede llegar a bloquear otras tareas.
+ Almacena datos como cadenas de texto, dificilmente puedes trabajar con datos más complejos
+ No es seguro para datos sensibles como contraseña, no cuenta con expiracion automática.


### Formato de almacenamiento
**XML:** Lenguaje que utiliza etiquetas para almacenar datos que se pueden almacenar.

**CSV:** Formato que utiliza tabulaciones utilizando comas para separar campos.

**YAML:** Es un formato de datos legible por humanos y facil de escribir. utilizando sangrias para su legibilidad.

**BSON:** Representación binaria de un JSON añadiendo fechas y binarios. Utilizada principalmente para datos NOSQL.

**Protobuf:** Formato de datos desarrollado por Goolge. Utiliza un sistema binario siendo eficiente en espacio y velocidad.

Uno de los formatos más comunes son los JSON, Porporcionando una estructura clara y legible, lo hace ideal para almacenar informacion en el desarrollo web. Esta basado en paras clave-valor y es facil de entender para humanos y maquinas. Ampliamente utilizado en la comunicación entre cliente y servidores.

```
{
  "nombre": "Juan",
  "edad": 30,
  "ciudad": "Ciudad de Ejemplo",
  "contacto": {
    "email": "juan@example.com",
    "telefono": "+123456789"
  },
  "intereses": ["programación", "viajes", "lectura"]
}
```
El uso de formatos adecuados es esencial para garantizar que los datos se guardes y recuperer de manera eficiente.