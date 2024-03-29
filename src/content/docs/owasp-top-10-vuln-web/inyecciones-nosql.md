---
title: Injecciones NoSQL
---
Las **inyecciones NoSQL** son una vulnerabilidad de seguridad en las aplicaciones web que utilizan bases de datos NoSQL, como MongoDB, Cassandra y CouchDB, entre otras. Estas inyecciones se producen cuando una aplicación web permite que un atacante envíe datos maliciosos a través de una consulta a la base de datos, que luego puede ser ejecutada por la aplicación sin la debida validación o sanitización.

La inyección NoSQL funciona de manera similar a la inyección SQL, pero se enfoca en las vulnerabilidades específicas de las bases de datos NoSQL. En una inyección NoSQL, el atacante aprovecha las consultas de la base de datos que se basan en **documentos** en lugar de tablas relacionales, para enviar datos maliciosos que pueden manipular la consulta de la base de datos y obtener información confidencial o realizar acciones no autorizadas.

A diferencia de las inyecciones SQL, las inyecciones NoSQL explotan la falta de validación de los datos en una consulta a la base de datos NoSQL, en lugar de explotar las debilidades de las consultas SQL en las **bases de datos relacionales**.

A continuación, se proporciona el enlace al proyecto de Github que nos descargamos para poner en práctica esta vulnerabilidad:

-   **Vulnerable-Node-App**: [https://github.com/Charlie-belmer/vulnerable-node-app](https://github.com/Charlie-belmer/vulnerable-node-app)

FORMA DE PODER LLEGAR A DESCUBRIR MAS USUARIOS:
```json
{"username" : {"$regex" : "^an"},"password":("$ne":"admin")}
```
---------

``` json
Normal sql: ' or 1=1-- -
Mongo sql: ' || 1==1//    or    ' || 1==1%00
```