---
title: GraphQl Introspection, Mutations e IDORs
---
**GraphQL** es un lenguaje de consulta para **APIs** (**Application Programming Interfaces**) que se ha vuelto cada vez más popular en los últimos años. A diferencia de las APIs tradicionales que tienen endpoints fijos, GraphQL permite a los clientes solicitar sólo la información que necesitan y obtener una respuesta personalizada en función de sus necesidades.

**Introspection** en GraphQL es un mecanismo que permite a los clientes **obtener información** sobre el esquema GraphQL de una API. Esto significa que los clientes pueden explorar y descubrir los tipos de datos, los campos y las relaciones que existen en la API, lo que puede ser muy útil para los desarrolladores que necesitan construir clientes GraphQL. Sin embargo, la introspección también puede ser utilizada por los atacantes para obtener información sensible sobre la estructura y los datos que existen en la API, lo que puede ser utilizado para llevar a cabo ataques más sofisticados.

Por otro lado, las **Mutations** en GraphQL son operaciones que permiten a los clientes **modificar los datos** en la API. A diferencia de las consultas, que sólo permiten la lectura de datos, las mutaciones permiten a los clientes agregar, actualizar o eliminar datos. Esto significa que las mutaciones tienen el potencial de ser utilizadas para realizar cambios importantes en la base de datos subyacente de la API. Si no se protegen adecuadamente, las mutaciones pueden ser explotadas por los atacantes para realizar cambios malintencionados en la API, como la eliminación de datos importantes o la creación de nuevos registros.

En el contexto de GraphQL, los **IDORs** pueden ocurrir cuando un atacante es capaz de adivinar o enumerar identificadores (**IDs**) de objetos dentro de la API, y puede utilizar esos IDs para acceder a objetos a los que no debería tener acceso. Esto puede ocurrir porque los desarrolladores de la API pueden no haber implementado adecuadamente los mecanismos de autenticación y autorización en su API.

Por ejemplo, supongamos que una API GraphQL permite a los usuarios acceder a información sobre sus propios pedidos utilizando el ID de pedido. Si el desarrollador de la API no ha implementado la autorización adecuada, un atacante podría utilizar la introspección de GraphQL para descubrir todos los IDs de pedido existentes en la API, incluyendo los pedidos de otros usuarios. El atacante podría luego utilizar estos IDs para acceder a los pedidos de otros usuarios sin la debida autorización, lo que constituye un IDOR.

Los atacantes también pueden utilizar las Mutaciones de GraphQL para llevar a cabo ataques IDOR. Por ejemplo, supongamos que una API GraphQL permite a los usuarios actualizar la información de sus propios pedidos. Si el desarrollador de la API no ha implementado adecuadamente la autorización, un atacante podría utilizar una mutación para actualizar los datos de los pedidos de otros usuarios, utilizando los IDs de pedido que ha descubierto mediante la introspección.

En resumen, GraphQL es un lenguaje de consulta para APIs que permite a los clientes solicitar sólo la información que necesitan. Es importante que los desarrolladores de APIs protejan adecuadamente la introspección y las mutaciones para evitar ataques maliciosos por parte de los atacantes.

A continuación, se os proporciona el enlace directo a los distintos proyectos de Github los cuales empleamos en esta clase para enumerar y abusar del GraphQL:

-   **GraphQL Introspection**: [https://github.com/blabla1337/skf-labs/tree/master/nodeJs/Graphql-Introspection](https://github.com/blabla1337/skf-labs/tree/master/nodeJs/Graphql-Introspection)
-   **GraphQL Mutations**: [https://github.com/blabla1337/skf-labs/tree/master/nodeJs/Graphql-Mutations](https://github.com/blabla1337/skf-labs/tree/master/nodeJs/Graphql-Mutations)
-   **GraphQL Injection**: [https://github.com/blabla1337/skf-labs/tree/master/nodeJs/Graphql-Injection](https://github.com/blabla1337/skf-labs/tree/master/nodeJs/Graphql-Injection)
-   **GraphQL IDOR**: [https://github.com/blabla1337/skf-labs/tree/master/nodeJs/Graphql-IDOR](https://github.com/blabla1337/skf-labs/tree/master/nodeJs/Graphql-IDOR)