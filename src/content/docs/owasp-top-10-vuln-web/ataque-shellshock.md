---
title: Ataque ShellShock
---
Un ataque **Shellshock** es un tipo de ataque informático que aprovecha una vulnerabilidad en el **intérprete de comandos Bash** en sistemas operativos basados en Unix y Linux. Esta vulnerabilidad se descubrió en 2014 y se considera uno de los ataques más grandes y generalizados en la historia de la informática.

Esta vulnerabilidad en Bash permite a los atacantes ejecutar comandos maliciosos en el sistema afectado, lo que les permite tomar el control del sistema y acceder a información confidencial, modificar archivos, instalar programas maliciosos, etc.

La vulnerabilidad Shellshock se produce en el intérprete de comandos Bash, que es utilizado por muchos sistemas operativos Unix y Linux para ejecutar scripts de shell. El problema radica en la forma en que Bash maneja las variables de entorno. Los atacantes pueden inyectar código malicioso en estas variables de entorno, las cuales Bash ejecuta sin cuestionar su origen o contenido.

Los atacantes pueden explotar esta vulnerabilidad a través de diferentes vectores de ataque. Uno de ellos es a través del **User-Agent**, que es la información que el navegador web envía al servidor web para identificar el tipo de navegador y sistema operativo que se está utilizando. Los atacantes pueden manipular el User-Agent para incluir comandos maliciosos, que el servidor web ejecutará al recibir la solicitud.

A continuación se proporciona el enlace directo para la descarga de la máquina ‘**SickOs 1.1**‘. Esta máquina corresponde a la misma que estuvimos enumerando en la clase anterior, solo que en este caso procederemos con la fase de explotación haciendo uso de esta técnica:

-   **SickOs 1.1**: [https://www.vulnhub.com/entry/sickos-11,132/](https://www.vulnhub.com/entry/sickos-11,132/)