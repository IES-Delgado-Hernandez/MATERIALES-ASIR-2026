# Los Anexos en el Proyecto Intermodular

## 1. ¿Qué son los Anexos?
Los anexos son secciones adicionales al final del proyecto que contienen información detallada, técnica o extensa. Su función principal es evitar que el cuerpo del documento se vuelva ilegible con tablas gigantes, códigos interminables o capturas de pantalla repetitivas.

> **Regla de oro:** El tribunal debería poder leer el cuerpo del proyecto y entenderlo perfectamente sin necesidad de abrir los anexos. Los anexos son para quien quiera profundizar en el "cómo" técnico.

---

## 2. ¿Para qué sirven?
* **Limpieza:** Mantienen el hilo argumental del proyecto fluido.
* **Justificación:** Aportan pruebas de que el sistema funciona (logs, capturas de pruebas).
* **Documentación técnica:** Guardan configuraciones detalladas que un administrador de sistemas necesitaría para replicar el entorno.
* **Cumplimiento legal:** Almacenan contratos, licencias o presupuestos detallados.

---

## 3. ¿Qué DEBE incluirse en los Anexos?
En un proyecto de **ASIR**, lo habitual es incluir:

1.  **Configuraciones de red completas:** Tablas de direccionamiento IP detalladas, reglas de firewall (`iptables`/`nftables`) o scripts de enrutamiento.
2.  **Código fuente y Scripts:** Scripts de Bash, Python, Ansible Playbooks o archivos YAML de Docker Compose.
3.  **Manuales de Usuario/Instalación:** Si el proyecto requiere que un tercero lo use o lo instale desde cero.
4.  **Presupuestos Detallados:** Listado de hardware, licencias de software y costes de horas/hombre.
5.  **Evidencias de Pruebas:** Capturas de pantalla de pings, trazas, escaneos de Nmap o pruebas de carga que confirmen que el despliegue es correcto.
6.  **Documentación de terceros:** Datasheets de hardware específico o licencias (GPL, MIT, etc.).

---

## 4. ¿Qué NO debe ir en los Anexos?
* **Conceptos teóricos básicos:** No incluyas una definición de qué es el protocolo TCP/IP o qué es un servidor. Se asume que el alumno ya conoce la base del ciclo.
* **Gráficos o tablas esenciales:** Si una tabla es necesaria para entender una decisión de diseño, debe ir en el cuerpo principal.
* **Páginas en blanco o material irrelevante:** Cada anexo debe estar referenciado al menos una vez en el texto principal.
* **Manuales oficiales de fabricantes:** No copies el manual de Cisco; pon un enlace o cita la fuente. Solo incluye lo que tú hayas configurado.

---

## 5. Estructura y Formato
Para que los anexos sean profesionales, deben seguir este orden:

* **Enumeración:** Anexo I, Anexo II, etc.
* **Índice de Anexos:** Al principio de la sección de anexos o en el índice general.
* **Referencias cruzadas:** En el cuerpo del texto se debe indicar: *(Ver Anexo III: Script de automatización de copias de seguridad)*.

> [!TIP]
> **Consejo para el alumno:** Si un script tiene más de 10 líneas, mándalo al anexo. Si una captura de pantalla no es vital para entender el paso actual, mándala al anexo.
