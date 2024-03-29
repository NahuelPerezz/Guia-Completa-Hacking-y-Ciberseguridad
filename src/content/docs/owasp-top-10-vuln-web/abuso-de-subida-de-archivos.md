---
title: Abuso de subida de archivos
---
El abuso de subidas de archivos es un tipo de ataque que se produce cuando un atacante aprovecha las vulnerabilidades en las aplicaciones web que permiten a los usuarios **cargar archivos** en el servidor. Este tipo de ataque se conoce comúnmente como un ataque de “**subida de archivos maliciosos**“.

En un ataque de subida de archivos maliciosos, un atacante carga un archivo malicioso en una aplicación web, que luego se almacena en el servidor. Si por ejemplo el atacante consigue subir un archivo PHP y el servidor web lo almacena, podría conseguir ejecución remota de comandos y tomar el control del servidor.

Los atacantes también pueden utilizar técnicas de “**falsificación de tipos de archivos**” para engañar a una aplicación web con el objetivo de que acepte un archivo malicioso como si fuera un archivo legítimo.

En esta clase, exploraremos algunas de las técnicas más utilizadas para explotar la fase de subida de archivos en aplicaciones web. Aprenderás cómo los atacantes pueden cargar contenido malicioso, además de eludir diferentes restricciones implementadas para lograrlo.

A continuación, se os comparte el enlace al proyecto de Github el cual estaremos empleando para desplegar un laboratorio práctico en Docker con el que poder practicar estos conceptos:

-   **File Upload Laboratory**: [https://github.com/moeinfatehi/file_upload_vulnerability_scenarios](https://github.com/moeinfatehi/file_upload_vulnerability_scenarios)****