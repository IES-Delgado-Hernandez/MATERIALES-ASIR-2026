# Ayuda para la realización de la Tarea 5 (Proyecto Intermodular – 2.º ASIR)
> - **NOTA**: AL FINAL DE ESTE ARCHIVO SE ENCUENTRA UN RESUMEN RÁPIDO DE TODA LA INFORMACIÓN

> **Propósito de este documento**  
> Esta guía te explica **cómo preparar la Tarea 5** paso a paso, con ejemplos y plantillas listas para copiar/pegar. Está organizada en dos grandes bloques que coinciden con lo que se evalúa:
> - **Criterio (f):** Determinar las **características específicas** del proyecto según los requerimientos → **Pre-anteproyecto**.  
> - **Criterio (i):** Elaborar el **guion de trabajo** que se seguirá para la elaboración del proyecto → **Plan de trabajo**.


---

## 0) Qué debo entregar (resumen)

- **Un único archivo** con nombre: `Tarea5_Unidad1_Nombre completo del alumno.formato`
- Contenido mínimo:
  1) **Pre-anteproyecto** (criterio f)  
  2) **Guion de trabajo** (criterio i)  
  3) (Opcional) Anexos: esquemas, tablas extendidas, capturas, etc.
- Presentación breve en el aula (5–7 minutos).

---

## 1) Pre-anteproyecto (criterio f)

El pre-anteproyecto define **qué vas a hacer** y **por qué**. Debe conectar con las tareas previas (sector, necesidades, oportunidades).

### 1.1 Estructura mínima recomendada

1. **Título del proyecto**  
   - Claro y específico (ej.: “Plataforma de copias de seguridad centralizada para pymes del sector vinícola”).
2. **Contexto y sector**  
   - Sector, motivación y particularidades tecnológicas (normativa, estacionalidad, conectividad, ciber-riesgos).
3. **Necesidad detectada**  
   - Problema/“pain point” priorizado en Tarea 3 (encaje con el cliente/usuario).
4. **Propuesta/idea de solución**  
   - Propósito, **alcance** (qué incluye / qué no incluye), público objetivo, beneficios.
5. **Requisitos del proyecto**  
   - **Funcionales** (mín. 5): lo que el sistema **hace**.  
   - **No funcionales**: rendimiento, seguridad, disponibilidad, usabilidad, trazabilidad, cumplimiento, etc.
6. **Recursos necesarios (estimación inicial)**  
   - **Técnicos**: HW, SW, licencias, nube, herramientas.  
   - **Humanos**: roles/perfiles (admin de sistemas, dev, QA, PM), aunque seas tú en todos.
7. **Restricciones y supuestos**  
   - Presupuesto, plazos, dependencias, normativa, límites del entorno educativo.
8. **Beneficios esperados y criterios de éxito**  
   - Indicadores medibles (ej.: RTO/RPO, % disponibilidad, reducción de incidencias).

### 1.2 Ejemplo orientativo (mini)

- **Título:** “Despliegue de VPN site-to-site y acceso remoto seguro para microempresas”  
- **Necesidad:** Teletrabajo y acceso seguro a recursos internos sin exponer servicios.  
- **Alcance:** Incluye diseño, PoC con 2 sedes y 3 usuarios remotos, política básica de acceso. No incluye SIEM ni hardening completo.  
- **Requisitos funcionales (ej.):**
  - RF1: Autenticación de usuarios remotos con MFA.  
  - RF2: Interconexión de dos sedes mediante túnel cifrado.  
  - RF3: Acceso segmentado a recursos (VLAN o ACLs).  
  - RF4: Registro básico de accesos.  
  - RF5: Manual de uso para empleados.
- **Requisitos no funcionales (ej.):**
  - RNF1: Disponibilidad ≥ 99 %.  
  - RNF2: Cifrado ≥ AES-256.  
  - RNF3: Acceso remoto operativo en ≤ 2 clics tras MFA.  
  - RNF4: RTO ≤ 2 h; RPO ≤ 24 h.
- **Recursos:** 2 routers compatibles/IPsec o WireGuard, servidor AAA, DNS, documentación.  
- **Restricciones:** Sin IP fija en sedes; presupuesto educativo; tiempo 6 semanas.  
- **Criterios de éxito:** 100 % de tests de conectividad y MFA superados; guía aprobada.

---

## 2) Guion de trabajo (criterio i)

El guion de trabajo es la **hoja de ruta**: qué pasos seguirás, en qué orden, con qué recursos y en qué tiempos.

### 2.1 Objetivos del proyecto

Formula objetivos **SMART** (específicos, medibles, alcanzables, relevantes, temporales).

> **Plantilla SMART**  
> - Objetivo O1: “Implementar un túnel site-to-site operativo con cifrado ≥ AES-256 entre Sede A y Sede B en la **Semana 3**, validado con tres pruebas documentadas (ping, recursos compartidos, throughput).”

### 2.2 Entregables y criterios de aceptación

Define qué “productos” intermedios generarás y cómo validarás que están bien.

> **Tabla de Entregables**
>
> | Entregable | Descripción | Criterios de aceptación | Fecha objetivo |
> |---|---|---|---|
> | E1 – Documento de Análisis | Contexto, requisitos (f/nf) | Revisión docente sin cambios críticos | S2 |
> | E2 – Diseño de Red | Diagrama lógico/físico, direccionado | Prueba de coherencia, sin conflictos | S3 |
> | E3 – PoC VPN | Túnel operativo entre sedes | 3/3 pruebas superadas y log evidencias | S4 |
> | E4 – Acceso Remoto | MFA activo para 3 usuarios | Conexión estable y auditada | S5 |
> | E5 – Documentación | Manual técnico y de usuario | Checklist de calidad completo | S6 |

### 2.3 Estructura de trabajo (WBS)

Desglosa **fases → tareas → subtareas** (numeración 1, 1.1, 1.1.1…).

> **WBS (ejemplo)**
>
> ```
> 1. Análisis
>   1.1 Revisión de requisitos
>   1.2 Estudio de viabilidad y supuestos
> 2. Diseño
>   2.1 Diseño lógico y direccionamiento
>   2.2 Diseño físico (equipos, topología)
> 3. Implementación
>   3.1 Configuración site-to-site
>   3.2 Configuración acceso remoto (MFA)
> 4. Pruebas y validación
>   4.1 Plan y casos de prueba
>   4.2 Ejecución y evidencias
> 5. Documentación y cierre
>   5.1 Manual técnico / usuario
>   5.2 Revisión final y checklist
> ```

### 2.4 Cronograma inicial (tipo Gantt simplificado)

Planifica semanas, dependencias e hitos.

> **Cronograma (ejemplo)**
>
> | Fase | S1 | S2 | S3 | S4 | S5 | S6 |
> |---|:--:|:--:|:--:|:--:|:--:|:--:|
> | 1. Análisis | █ | █ |  |  |  |  |
> | 2. Diseño |  | █ | █ |  |  |  |
> | 3. Implementación |  |  | █ | █ |  |  |
> | 4. Pruebas/Validación |  |  |  | █ | █ |  |
> | 5. Documentación/Cierre |  |  |  |  | █ | █ |
>
> **Hitos:** H1 (fin análisis S2), H2 (diseño validado S3), H3 (PoC operativa S4), H4 (presentación S6).

### 2.5 Roles y recursos por tarea

Aunque sea un proyecto individual, **explicita el rol** que asumes en cada tarea y los recursos que usarás.

> **Asignación (ejemplo)**
>
> | Tarea | Rol | Recursos |
> |---|---|---|
> | 2.1 Diseño lógico | Admin de sistemas | Draw.io, RFC/IP plan |
> | 3.2 Acceso remoto | Admin de sistemas / Seguridad | WireGuard/OpenVPN, IdP/MFA |

### 2.6 Flujo de trabajo y métodos

Estándares que usarás para **orden** y **calidad**:
- **Control de versiones:** Git, ramas `main`/`dev`, mensajes tipo Conventional Commits.  
- **Seguimiento:** tablero Kanban (ToDo/Doing/Done), revisiones semanales.  
- **Documentación:** Markdown + capturas, nombres `YYYY-MM-DD_*`, índice y glosario.  
- **Normativa/estándares:** buenas prácticas de seguridad (mínimas), naming, backups de evidencias.

### 2.7 Gestión de riesgos

Identifica **mínimo 5** riesgos con su probabilidad/impacto, prevención y contingencia.

> **Riesgos (plantilla)**
>
> | Riesgo | Prob./Impacto | Prevención | Contingencia |
> |---|---|---|---|
> | Sin IP fija | Media/Media | DynDNS, puertos controlados | Alternar a túnel saliente |
> | Fallo HW | Baja/Alta | Equipo backup/VM | Migración a VM en Proxmox |
> | Tiempo insuficiente | Media/Media | Timeboxing semanal | Reducir alcance (MoSCoW) |
> | MFA incompatible | Baja/Media | Prueba piloto | Método alternativo temporal |
> | Logs insuficientes | Media/Media | Config inicial logging | Aumentar verbosidad y retención |

### 2.8 Plan de comunicación y control

- **Qué**: estado de tareas, bloqueos, evidencias, próximos pasos.  
- **Quién**: alumno → profesor/tutor.  
- **Cuándo**: checkpoint semanal (fecha fija).  
- **Cómo**: acta breve (1 página) + tablero actualizado.

> **Acta (mini-plantilla)**
>
> - Semana: S3 (fecha)  
> - Avances: …  
> - Bloqueos: …  
> - Decisiones: …  
> - Próximos pasos (S4): …

---

## 3) Checklist de calidad antes de entregar

- [ ] Título, sector, necesidad y **alcance** están claros.  
- [ ] Requisitos **funcionales (≥5)** y **no funcionales** definidos.  
- [ ] Recursos, restricciones y criterios de éxito especificados.  
- [ ] **Objetivos SMART** redactados.  
- [ ] **WBS** con fases/tareas coherentes.  
- [ ] **Cronograma** con semanas e hitos.  
- [ ] **Entregables** con criterios de aceptación.  
- [ ] **Riesgos (≥5)** con prevención/contingencia.  
- [ ] **Plan de comunicación** (ritmo y formato).  
- [ ] Documento en **PDF** con nombre correcto y numeración de páginas.

---

## 4) Errores frecuentes (y cómo evitarlos)

- **Alcance difuso:** define explícitamente **qué no incluye** el proyecto.  
- **Requisitos genéricos o vacíos:** escribe requisitos **verificables**.  
- **Cronogramas irreales:** sé prudente; usa timeboxing.  
- **Sin criterios de aceptación:** añade “cómo sabré que está bien”.  
- **Riesgos decorativos:** piensa en **lo que de verdad te puede frenar**.  
- **Sin evidencias:** planifica capturas/logs/poC para demostrar avances.

---

## 5) Plantillas listas para copiar

### 5.1 Requisitos (tabla)
| ID | Tipo | Descripción | Criterio de verificación |
|---|---|---|---|
| RF1 | Funcional | … | Caso de prueba #… |
| RNF1 | No funcional | … | Métrica ≥ … |

### 5.2 Entregables
| Entregable | Descripción | Criterios de aceptación | Fecha |
|---|---|---|---|
| E1 | … | … | … |

### 5.3 WBS (esqueleto)
  Análisis
  1.1 …
  
  Diseño
  2.1 …
  
  Implementación
  3.1 …
  
  Pruebas/Validación
  4.1 …
  
  Documentación/Cierre
  5.1 …

### 5.4 Cronograma
| Fase | S1 | S2 | S3 | S4 | S5 | S6 |
|---|:--:|:--:|:--:|:--:|:--:|:--:|
| 1. Análisis |  |  |  |  |  |  |
| 2. Diseño |  |  |  |  |  |  |
| 3. Implementación |  |  |  |  |  |  |
| 4. Pruebas |  |  |  |  |  |  |
| 5. Documentación |  |  |  |  |  |  |

### 5.5 Riesgos
| Riesgo | Prob./Impacto | Prevención | Contingencia |
|---|---|---|---|
| … | … | … | … |

### 5.6 Acta semanal
- Semana: … (fecha)  
- Avances: …  
- Bloqueos: …  
- Decisiones: …  
- Próximos pasos: …

---

## 6) Entrega

- **Formato:** PDF  
- **Nombre de archivo:** `Tarea5_Unidad1_Nombre completo del alumno.pdf`  
- **Entrega:** Moodle

> Consejo final: escribe primero un **borrador breve** (1–2 páginas) para validar enfoque y alcance. Después amplía con requisitos, WBS y cronograma.

---

# RESUMEN RÁPIDO – Tarea 5: Pre-anteproyecto y guión de trabajo

> **Objetivo general:**  
> Definir tu idea de proyecto (**pre-anteproyecto**) y planificar **cómo vas a desarrollarla** (**guion de trabajo**).  
> Es el paso previo al anteproyecto final del trimestre.

---

##  Parte 1 – Pre-anteproyecto (criterio f)

Define **qué vas a hacer** y **por qué**.  
Conecta con las tareas anteriores (sector, empresa, necesidad detectada).

**Contenido mínimo:**
1. **Título del proyecto**  
2. **Sector y contexto** (motivación y características tecnológicas)  
3. **Necesidad o problema detectado**  
4. **Propuesta o idea de solución**  
   - Propósito y alcance  
   - Público objetivo y beneficios  
5. **Requisitos del proyecto**  
   - Funcionales (qué hace el sistema)  
   - No funcionales (rendimiento, seguridad, disponibilidad, etc.)  
6. **Recursos necesarios** (técnicos y humanos)  
7. **Restricciones o límites**  
8. **Beneficios esperados y criterios de éxito**

---

##  Parte 2 – Guion de trabajo (criterio i)

Planifica **cómo** vas a realizar el proyecto: fases, tiempos, tareas, riesgos y control.

**Debe incluir:**
1. **Objetivos SMART** (claros, medibles y alcanzables)  
2. **Entregables** con criterios de aceptación  
3. **Estructura de trabajo (WBS)** – fases y tareas numeradas  
4. **Cronograma o Gantt simple** – semanas, hitos y dependencias  
5. **Roles y recursos por tarea**  
6. **Método de trabajo** – Git, documentación, tableros, revisiones  
7. **Gestión de riesgos** – mínimo 5 con prevención y contingencia  
8. **Plan de comunicación y control** – informes o actas semanales  

---

##  Checklist antes de entregar

✅ Requisitos funcionales y no funcionales definidos  
✅ Objetivos SMART redactados  
✅ Fases y tareas bien estructuradas (WBS)  
✅ Cronograma realista con hitos  
✅ Riesgos y medidas preventivas incluidos  
✅ Documento claro, numerado y completo  
✅ Nombre correcto del archivo:  
`Tarea5_Unidad1_Nombre completo del alumno.pdf`

---

##  Formato y entrega

- **Formato:** presentación  
- **Nombre del archivo:** `Tarea5_Unidad1_Nombre completo del alumno.pdf`  
- **Entrega:** Moodle  
- **Presentación:** breve exposición (5–7 min) con los aspectos clave del proyecto.

> 💡 **Consejo:**  
> Resume en una diapositiva los apartados clave (título, necesidad, solución, fases e hitos).  
> Esto te servirá como guion para la presentación oral.

