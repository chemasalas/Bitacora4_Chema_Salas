# MEMORIA TÉCNICA
## Infraestructura Docker y Apache Guacamole

### Autor
Tu Nombre y Apellidos

### Ciclo
ASIR / DAM / DAW

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

La empresa objeto del presente proyecto requiere un sistema de acceso remoto seguro y centralizado para la administración de servidores internos y entornos de desarrollo. Inicialmente, los técnicos accedían directamente mediante conexiones RDP y SSH a múltiples máquinas, lo que suponía un incremento considerable de la superficie de ataque y una mayor complejidad administrativa.

Asimismo, la apertura de múltiples puertos en el firewall representaba un riesgo de seguridad crítico, ya que cualquier vulnerabilidad en los servicios expuestos podría comprometer la infraestructura corporativa. Del mismo modo, la gestión descentralizada de credenciales dificultaba las tareas de auditoría y control de accesos.

Por consiguiente, se identificó la necesidad de implantar una solución centralizada que permitiera simplificar la administración remota, mejorar la seguridad y optimizar el mantenimiento de los servicios corporativos.

---

## 1.2 Solución Propuesta: Infraestructura Docker-Guacamole

Tras analizar las necesidades de accesibilidad, seguridad y escalabilidad, se ha optado por implementar una solución basada en Apache Guacamole desplegada mediante contenedores Docker.

Apache Guacamole actúa como una puerta de acceso remota vía web, permitiendo conexiones SSH y RDP desde cualquier navegador sin necesidad de instalar clientes específicos en los equipos de los usuarios. Esta característica reduce considerablemente la complejidad operativa y facilita el acceso seguro a los recursos internos.

La utilización de Docker proporciona aislamiento entre servicios, evitando conflictos de dependencias y mejorando la portabilidad de la infraestructura. Cada componente del sistema, como PostgreSQL, Guacamole y OpenSSH, opera dentro de un contenedor independiente, permitiendo una gestión modular y profesional.

Además, esta arquitectura permite centralizar la autenticación y el control de conexiones, facilitando la auditoría y mejorando las capacidades de monitorización del sistema.

---

## 1.3 Justificación Técnica y Beneficios

La solución implementada ofrece importantes ventajas técnicas y económicas para la organización. En primer lugar, la centralización del acceso remoto reduce significativamente la exposición directa de servicios críticos a Internet, aumentando el nivel general de seguridad de la infraestructura.

Asimismo, el uso de tecnologías open source bajo licencias permisivas permite minimizar el Coste Total de Propiedad (TCO), evitando costes recurrentes de licencias comerciales y favoreciendo la sostenibilidad económica del proyecto.

Docker aporta además una elevada portabilidad, permitiendo desplegar la infraestructura rápidamente en distintos entornos sin necesidad de configuraciones complejas. Esto mejora los tiempos de recuperación ante desastres y simplifica las tareas de mantenimiento.

En consecuencia, la solución basada en Docker y Apache Guacamole representa una infraestructura moderna, escalable y alineada con las buenas prácticas profesionales de administración de sistemas.

---

# 2. Referencias

[1] Apache Guacamole Project. Disponible en: https://guacamole.apache.org/

[2] Docker Documentation. Disponible en: https://docs.docker.com/

[3] PostgreSQL Documentation. Disponible en: https://www.postgresql.org/docs/

[4] García Notario, D. “Análisis de requisitos en el desarrollo del software”.

[5] Drake, J. M. “Análisis de requisitos y especificación de una aplicación”.
