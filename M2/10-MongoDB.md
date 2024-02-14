# MongoDB

SQL es un lenguaje que se utiliza para trabajar en base de datos. NOSQL no utilizan el ese lenguaje para el manejo de base de datos.

## ¿CÓmo nos comunicamos en una base de datos NOSQL?
En base de datos SQL para poder realizar una consulta se debe hacer referencia a las columnas correspondientes para solicitar la información. En cambio con las NOSQL, se podria hacer una consulta simple.
```
database.libros.findOne({ titulo: "El principito" })
```

### Estructura de datos
MongoDB es un sistema de base de datos NOSQL, almacena los datos en un formato llamado BSON( binary JSON ), que es una representación binaria de un JSON.

Pricipales caracteristicas:
+ Esquema dinamico, trabaja con estructuras que pueden ser modificadas de formas dinamicas.
+ BSON formato creado por Mongo par mejorar la transferencia de datos

## Elementos Principales

+ **Documentos:** Es la unidad básica de almacenamiento, si guardamos la información especifica de un usuario, ese conjuto de datos sera un documento. Guardado en formato BSON y contiene clave-valor.

+ **Colecciones:** Una colección es un conjunto de documentos almacenados que estan relacionados entre sí.


+ **Referencia:** 
En muchas situaciones vamos a querer hacer una referencia entre documentos. Las referencias son conexiones entre dos documentos.

## Atlas
mongoDB atlas es una plataforma de base de datos en la nube para trabajar con mongoDB, este servicio nos permite deployar de manera sencilla nuestra base de datos. Realiza respaldo automáticos y recuperar datos en caso de pérdida.

## MongoDB compass
Es una interfaz por el cual podemos trabajar la base de datos en la nube. Nos permite trabajar sin tener que entrar a algun navegador