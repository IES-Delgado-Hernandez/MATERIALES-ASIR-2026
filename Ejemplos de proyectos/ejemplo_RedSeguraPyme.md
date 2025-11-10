---
titulo: Ejemplo de Proyecto Intermodular - RedSegura Pyme
autor: Ejemplo de referencia docente
modulo: Proyecto Intermodular (2º ASIR)
version: 1.0
objetivo: Servir de guía de referencia para comprender el alcance completo de un proyecto intermodular en ASIR.
---

# Proyecto de referencia: "RedSegura Pyme"
## Ejemplo completo de proyecto intermodular para 2.º ASIR

---

## 1. Contexto general

**Empresa simulada:** Bodega Digital S.L.  
**Sector:** Agroalimentario – Producción y distribución vinícola.  
**Ubicación:** Bollullos Par del Condado (Huelva).  
**Tamaño:** Pyme con 15 empleados.  
**Infraestructura actual:**  
- Red local desorganizada sin segmentación.  
- Servidor NAS sin copias automatizadas.  
- Uso de routers domésticos y contraseñas por defecto.  
- Sin control de usuarios ni políticas de acceso.  

La dirección de la empresa busca **modernizar su infraestructura tecnológica**, mejorar la **seguridad de la información** y **aumentar la eficiencia interna**.

---

## 2. Título del proyecto

**"RedSegura Pyme: Implantación de una infraestructura de red, servidores y políticas de seguridad para Bodega Digital S.L."**

---

## 3. Objetivo general

Diseñar, implementar y documentar una **infraestructura tecnológica completa** que garantice la seguridad, estabilidad y eficiencia de las operaciones de la empresa, incluyendo red local, servidores, copias de seguridad y control de accesos.

---

## 4. Objetivos específicos

- Diseñar una **red segmentada por VLAN** que separe las áreas administrativa, técnica y de invitados.  
- Instalar un **servidor central** que actúe como controlador de dominio, DNS, DHCP y servidor de archivos.  
- Implementar un sistema de **copias de seguridad automatizadas** y restauración.  
- Establecer **políticas de seguridad y contraseñas**, junto con auditorías básicas de red.  
- Elaborar una **documentación técnica completa** y un **manual de usuario**.  

---

## 5. Alcance del proyecto

### 5.1 Alcance incluido
- Diseño lógico y físico de red local.  
- Configuración de switches gestionables con VLAN.  
- Implementación de servicios esenciales (DHCP, DNS, AD, Samba).  
- Configuración de servidor de copias (Bacula o rsnapshot).  
- Creación de scripts de automatización de mantenimiento.  
- Elaboración de documentación técnica y presentación final.  

### 5.2 Fuera de alcance
- Instalación física de cableado.  
- Certificación de red profesional.  
- Servicios de alta disponibilidad (clúster, replicación).  
- Integración con aplicaciones externas (ERP, CRM).

---

## 6. Requisitos del proyecto

### 6.1 Requisitos funcionales
| ID | Descripción |
|----|--------------|
| RF1 | Implementar VLANs para separar tráfico administrativo, técnico y de invitados. |
| RF2 | Instalar y configurar un servidor central con DNS, DHCP y control de dominio. |
| RF3 | Crear y gestionar usuarios y permisos según departamento. |
| RF4 | Automatizar copias de seguridad diarias del servidor y las estaciones. |
| RF5 | Documentar toda la configuración en formato profesional (Markdown + PDF). |

### 6.2 Requisitos no funcionales
| ID | Descripción |
|----|--------------|
| RNF1 | Disponibilidad de red ≥ 99 % durante pruebas. |
| RNF2 | Restauración completa en < 2 h. |
| RNF3 | Contraseñas seguras con longitud mínima de 10 caracteres. |
| RNF4 | Protocolos cifrados en servicios de acceso remoto. |
| RNF5 | Documentación validada por el tutor. |

---

## 7. Recursos necesarios

### 7.1 Materiales y técnicos
- 2 switches gestionables.  
- 1 router/firewall (pfSense o similar).  
- 3 equipos virtualizados (servidor, cliente 1, cliente 2).  
- Software: Ubuntu Server / Windows Server / pfSense / Bacula / WireGuard.  
- Herramientas: Draw.io, GitHub, Markdown, VirtualBox, Wireshark.

### 7.2 Humanos
| Rol | Responsable | Funciones |
|------|--------------|-----------|
| Admin. de sistemas | Alumno | Configuración de red, servidores y copias. |
| Técnico de soporte | Alumno | Pruebas, simulación de fallos y restauración. |
| Documentador | Alumno | Creación de manuales y evidencias. |

---

## 8. Restricciones

- Presupuesto máximo: 600 €.  
- Duración del proyecto: 8 semanas lectivas.  
- Infraestructura simulada en entorno virtual.  
- Se prioriza el uso de software libre y entornos educativos.

---

## 9. Beneficios esperados

- Mejora del rendimiento de red y seguridad.  
- Reducción del tiempo de recuperación ante fallos.  
- Incremento del control sobre usuarios y recursos compartidos.  
- Transferencia de conocimiento tecnológico a entornos reales.  

---

## 10. WBS (Estructura de Desglose del Trabajo)

    Análisis
    1.1 Evaluación del entorno y detección de necesidades
    1.2 Requisitos funcionales y no funcionales
    
    Diseño
    2.1 Topología de red y direccionamiento IP
    2.2 Diseño de VLAN y servidores
    
    Implementación
    3.1 Configuración de switches y router
    3.2 Instalación de servicios DNS, DHCP, AD
    3.3 Configuración de copias automatizadas
    
    Pruebas y validación
    4.1 Comprobación de conectividad y VLAN
    4.2 Restauración de copias y pruebas de seguridad
    
    Documentación y entrega
    5.1 Manual técnico
    5.2 Presentación final del proyecto

---

## 11. Cronograma (8 semanas)

| Fase | S1 | S2 | S3 | S4 | S5 | S6 | S7 | S8 |
|------|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|
| Análisis | █ | █ |  |  |  |  |  |  |
| Diseño |  | █ | █ |  |  |  |  |  |
| Implementación |  |  | █ | █ | █ |  |  |  |
| Pruebas |  |  |  | █ | █ | █ |  |  |
| Documentación |  |  |  |  | █ | █ | █ | █ |

---

## 12. Gestión de riesgos

| Riesgo | Prob./Impacto | Prevención | Contingencia |
|--------|----------------|-------------|---------------|
| Fallo de configuración VLAN | Media/Alta | Copia de seguridad del switch | Restauración de config inicial |
| Incompatibilidad software | Media/Media | Pruebas previas en VM | Sustituir por alternativa libre |
| Retraso de ejecución | Alta/Media | Planificación semanal | Ajustar alcance del proyecto |
| Errores en backups | Media/Alta | Test diario de logs | Copias redundantes locales |
| Pérdida de documentación | Baja/Alta | Uso de GitHub | Clonado semanal y backup externo |

---

## 13. Plan de comunicación

- **Revisión semanal con el tutor.**  
- **Registro de progreso en repositorio GitHub.**  
- **Acta semanal** con avances, bloqueos y decisiones.  
- **Presentación final** con defensa oral (10 minutos).

---

## 14. Entregables finales

| Entregable | Descripción | Formato |
|-------------|--------------|----------|
| Documento de análisis | Requisitos, diagnóstico y objetivos. | PDF |
| Diseño de red y servidores | Diagramas, esquemas y direccionamiento. | Draw.io / PDF |
| Implementación y scripts | Configuración técnica y scripts. | Markdown / .sh |
| Pruebas y resultados | Logs, capturas y validaciones. | PDF |
| Manual técnico y de usuario | Instrucciones y guía de mantenimiento. | PDF |
| Presentación final | Resumen del proyecto. | PowerPoint / Genially |

---

## 15. Conclusión

El proyecto **RedSegura Pyme** integra todas las competencias del ciclo formativo de ASIR:
- Administración de sistemas operativos.  
- Servicios de red e Internet.  
- Seguridad y alta disponibilidad.  
- Planificación y documentación profesional.  

Este ejemplo muestra la **dimensión real** de un **proyecto intermodular completo**, en el que el alumno debe asumir el rol de **administrador de sistemas**, planificar, ejecutar y documentar una **solución técnica completa** aplicable a un entorno empresarial real o simulado.

---

## 16. Extensiones posibles (para alumnos avanzados)
- Integración de un sistema de tickets (GLPI).  
- Implementación de autenticación multifactor (MFA).  
- Centralización de logs mediante Graylog o ELK.  
- Monitorización avanzada con Zabbix.  
- Despliegue híbrido con Proxmox y contenedores Docker.

---
