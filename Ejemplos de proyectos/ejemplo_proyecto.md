# 🚀 Proyecto Intermodular ASIR – Ejemplo de referencia

Este es un ejemplo de **Proyecto Intermodular para 2º ASIR**.  
El objetivo es mostrar cómo un único proyecto integra los aprendizajes de todos los módulos del ciclo, con un caso realista y profesional.

---

## Descripción del proyecto
Diseño, implantación y documentación de una **infraestructura híbrida segura para una empresa tecnológica**, que combine servicios **on-premise** y **cloud**, garantizando seguridad, disponibilidad y escalabilidad.

El escenario ficticio es la empresa *TechSolutions S.L.*, con unos 50 empleados, que necesita:
- Control centralizado de usuarios y grupos.
- Red segmentada y segura.
- Servicios internos (ficheros, web, BBDD).
- Servicios externos en la nube (correo, backups, web pública).
- Soluciones de monitorización y alta disponibilidad.
- Documentación completa y defensa pública.

---

## 🏗️ Alcance técnico del proyecto
- **Red local segmentada** con VLANs y firewall perimetral (pfSense).
- **Virtualización** con Proxmox o VMware ESXi.
- **Windows Server** con Active Directory y GPO.
- **Linux** con servicios web, correo y base de datos.
- **Servicios cloud**: correo corporativo (Microsoft 365 o Google Workspace), web en AWS/Azure, backups en la nube.
- **Seguridad avanzada**: VPN, políticas de contraseñas, firewall, auditoría de logs.
- **Monitorización** con Zabbix o Grafana.
- **Automatización** mediante scripts en Bash y PowerShell.
- **Documentación técnica profesional**: memoria, anexos, manuales y presupuesto.

---

## 📚 Qué incluye de cada módulo de ASIR

### 🖥️ Implantación de sistemas operativos
- Instalación y configuración de Windows Server y Linux en entornos virtualizados.
- Creación de imágenes y snapshots.

### 🌐 Planificación y administración de redes
- Diseño lógico y físico de la red (diagramas).
- Segmentación mediante VLANs y subredes.
- Configuración de routers, switches virtuales y direccionamiento IP.

### 🔧 Fundamentos de hardware
- Selección y dimensionamiento del hardware necesario para servidores.
- Justificación de equipos físicos y requisitos de virtualización.

### 🗄️ Gestión de bases de datos
- Diseño de una base de datos corporativa.
- Consultas SQL básicas para explotación de datos.

### 🏷️ Lenguajes de marcas y sistemas de gestión de información
- Creación de documentación en Markdown (README, guías).
- Uso de XML/HTML para describir configuraciones y plantillas.

### ⚙️ Administración de sistemas operativos
- Administración de usuarios, permisos y políticas en Windows y Linux.
- Automatización de tareas con scripts de sistema.

### 🌍 Servicios de red e Internet
- Configuración de DNS, DHCP, Proxy y VPN.
- Servicios web internos y externos (Nginx/Apache).
- Servidor de correo electrónico.

### 💻 Implantación de aplicaciones web
- Despliegue de una aplicación web en servidor Linux.
- Configuración de un CMS o aplicación personalizada.

### 🛠️ Administración de sistemas gestores de bases de datos
- Instalación y administración de MariaDB/PostgreSQL.
- Gestión de usuarios, roles, copias y restauración de BBDD.

### 🔐 Seguridad y alta disponibilidad
- Implementación de firewall perimetral.
- Políticas de seguridad (contraseñas, roles, accesos).
- Estrategia de copias de seguridad 3-2-1.
- Simulación de recuperación ante desastres.

### 🌎 0179. Inglés Profesional (Grado Superior)
- Documentación técnica en inglés (resumen ejecutivo, manual de instalación).
- Uso de terminología técnica internacional.

### 👔 1709 / 1710. Itinerario personal para la empleabilidad I y II
- Trabajo individual con planificación y gestión de tiempos.
- Desarrollo de competencias transversales (autonomía, responsabilidad, comunicación).

### 💡 1665. Digitalización aplicada a los sectores productivos
- Integración de servicios cloud (AWS/Azure).
- Uso de herramientas digitales para la gestión de proyectos.

### 🌱 1708. Sostenibilidad aplicada al sistema productivo
- Optimización de recursos en servidores virtualizados.
- Propuesta de reducción del consumo energético mediante consolidación de servicios.

### 🗂️ Módulo profesional optativo 
- Ejemplo: integración de un servicio o herramienta específica (p. ej. Nextcloud, GitLab local, servicio de ticketing).

---

## 📊 Documentación del proyecto
1. **Memoria técnica** (índice oficial con alcance, diseño, implementación y conclusiones).
2. **Anexos**: acta de constitución, cronograma, WBS, plan de pruebas, scripts, evidencias.
3. **Diagramas**: red lógica y física, flujos de datos, esquema de seguridad.
4. **Manual de usuario y manual de administrador**.
5. **Presupuesto y comparativa de alternativas**.

---

## 🎤 Defensa final
- Presentación oral.
- Demo en directo o vídeo mostrando:  
  - Login en Active Directory.  
  - Acceso seguro mediante VPN.  
  - Monitorización con alertas activas.  
  - Ejecución de un script de automatización.  

---

📌 Este proyecto integra todos los módulos de ASIR y demuestra competencias técnicas, organizativas y comunicativas.

----------------------------------------------------------------------------------------------------------
# 📅 Fases del Diagrama de Gantt – Proyecto Intermodular ASIR

| Fase | Subfases principales | Dependencias |
|------|----------------------|--------------|
| **1. Inicio del proyecto** | - Acta de constitución<br>- Definición de objetivos y alcance<br>- Identificación de recursos y roles<br>- Planificación inicial | Ninguna |
| **2. Análisis y diseño** | - Estudio de requisitos<br>- Diseño de la infraestructura (red lógica y física)<br>- Selección de hardware y software<br>- Diseño de políticas de seguridad y HA<br>- Elaboración de diagramas (UML, ER, arquitectura, flujos) | F1 |
| **3. Preparación de entornos** | - Montaje de entornos de virtualización (Proxmox/VMware)<br>- Instalación base de Windows Server y Linux<br>- Creación de snapshots e imágenes iniciales | F2 |
| **4. Implementación** | - Redes: VLANs, direccionamiento, firewall, VPN<br>- Windows Server: AD, GPO, permisos<br>- Linux: servicios web, correo, BBDD<br>- Aplicaciones web: despliegue CMS/app<br>- BBDD: diseño, creación y administración<br>- Cloud: correo, web pública, backups<br>- Monitorización: Zabbix/Grafana<br>- Automatización: scripts en Bash/PowerShell | F3 |
| **5. Pruebas y validación** | - Pruebas unitarias por servicio<br>- Pruebas de integración<br>- Pruebas de seguridad (roles, accesos, auditorías)<br>- Validación de alta disponibilidad<br>- Informe de resultados | F4 |
| **6. Documentación** | - Memoria técnica (índice oficial)<br>- Manual de usuario y administrador<br>- Presupuesto y comparativas<br>- Anexos (scripts, evidencias, capturas, acta, WBS)<br>- Documentación técnica en inglés | F5 |
| **7. Defensa final** | - Preparación de la presentación oral<br>- Elaboración de diapositivas<br>- Ensayo de demo (AD, VPN, monitorización, automatización)<br>- Defensa pública | F6 |

