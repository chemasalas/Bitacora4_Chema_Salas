# MEMORIA TÉCNICA
## Infraestructura Docker y Apache Guacamole

### Autor
Chema Salas Galan

### Ciclo
DAW 1

### Fecha
15 de mayo de 2026

---

# Índice

(1) Análisis de Necesidades
 
  1.1 Contexto y Problemática Actual
  
  1.2 Solución Propuesta: Infraestructura Docker-Guacamole

  1.3 Justificación Técnica y Beneficios

(2) Referencias

---

# 1. Análisis de Necesidades

## 1.1 Contexto y Problemática Actual

La empresa necesitaba una forma más segura y sencilla de acceder a los servidores internos y a los entornos de desarrollo. Al principio, los técnicos se conectaban directamente a cada equipo mediante distintas conexiones remotas, lo que hacía más complicada la gestión y aumentaba los riesgos de seguridad.

Además, tener varios accesos abiertos hacia los servidores suponía una posible vulnerabilidad para la infraestructura de la empresa. También resultaba difícil controlar quién accedía a cada sistema y llevar un seguimiento adecuado de los permisos y credenciales utilizados.

Por ello, se vio la necesidad de implantar una solución centralizada que permitiera facilitar la administración remota, reforzar la seguridad y simplificar el mantenimiento de los servicios corporativos.

---

## 1.2 Solución Propuesta: Infraestructura Docker-Guacamole

Tras analizar las necesidades de acceso, seguridad y crecimiento del sistema, se decidió implementar una solución basada en Apache Guacamole utilizando contenedores Docker.

Apache Guacamole permite acceder de forma remota a los servidores desde un navegador web, sin necesidad de instalar programas adicionales en los equipos de los usuarios. Gracias a ello, el acceso resulta más cómodo, sencillo y seguro para los técnicos.

Por otro lado, el uso de Docker facilita la organización de los distintos servicios del sistema. Cada elemento, como la base de datos, Guacamole o el servicio SSH, funciona de manera independiente dentro de su propio contenedor, lo que simplifica la instalación, el mantenimiento y futuras ampliaciones.

Además, esta estructura permite gestionar de forma centralizada los accesos y conexiones de los usuarios, mejorando el control, la supervisión y el seguimiento de la actividad dentro del sistema.

---

## 1.3 Justificación Técnica y Beneficios

La solución implantada aporta varias ventajas tanto a nivel técnico como económico para la organización. En primer lugar, al centralizar el acceso remoto, se reduce la exposición directa de los servidores y servicios internos a Internet, mejorando así la seguridad general de la infraestructura.

Además, el uso de herramientas de código abierto evita tener que pagar licencias comerciales, lo que permite reducir costes y mantener una solución más sostenible a largo plazo.

Por otro lado, Docker facilita que el sistema pueda instalarse y ponerse en marcha rápidamente en diferentes entornos, sin necesidad de realizar configuraciones complicadas. Esto también ayuda a simplificar el mantenimiento y mejora la capacidad de recuperación ante posibles fallos.

En conjunto, la combinación de Docker y Apache Guacamole proporciona una solución moderna, flexible y fácil de administrar, adaptada a las necesidades actuales de gestión y acceso remoto.

---

# 1.4 Referencias

[1] Apache Guacamole Project. Disponible en: https://guacamole.apache.org/

[2] Docker Documentation. Disponible en: https://docs.docker.com/

[3] PostgreSQL Documentation. Disponible en: https://www.postgresql.org/docs/

[4] García Notario, D. “Análisis de requisitos en el desarrollo del software”.

[5] Drake, J. M. “Análisis de requisitos y especificación de una aplicación”.

## 2. Estimación de Costes de Infraestructura

<img width="837" height="207" alt="image" src="https://github.com/user-attachments/assets/830ef5bf-3f73-4106-b644-85d977987e41" />

## 3. Estrategia de Despliegue y Comunicación

Para subir los archivos de la aplicación al servidor se usará SFTP, que es como el FTP de toda la vida pero seguro. La diferencia es que SFTP cifra los datos, así que nadie puede ver las contraseñas ni los archivos mientras viajan por Internet. Esto hace que el proceso sea mucho más fiable.

El método será muy simple: conectarse al servidor con SFTP, subir los archivos y reiniciar los servicios que hagan falta. Es un proceso fácil y seguro.

Para comunicarnos dentro del equipo usaremos Discord, porque permite avisar rápido si hay un problema, mandar mensajes cortos y recibir alertas si el servidor se cae. Así todos pueden enterarse al momento.

## 4. Justificación Científica

He visto este artículo académico reciente sobre el uso de Docker. El estudio explica que Docker ayuda a que las aplicaciones funcionen siempre igual, evita errores al moverlas entre equipos y hace que todo sea más rápido de instalar. Esto encaja perfectamente con el proyecto, ya que necesitamos algo fácil de mantener y que no dé problemas al desplegarlo.

### Referencia IEEE
J. Martínez y L. Robles, “Evaluación de la seguridad y rendimiento en entornos basados en contenedores Docker,” Revista Iberoamericana de Tecnologías Avanzadas, vol. 6, no. 1, pp. 22–34, 2023.

