# ETQ Reliance Automation Engineering

> Ingeniería aplicada para convertir automatizaciones ETQ Reliance en soluciones seguras, explicables y mantenibles.
>
> Applied engineering for turning ETQ Reliance automations into safe, explainable, and maintainable solutions.

[Español](#español) · [English](#english) · [Solicitar acceso](#solicitar-acceso--request-access)

---

## Español

### Acerca del proyecto

ETQ Reliance Automation Engineering es una iniciativa independiente para organizar, analizar y mejorar soluciones construidas alrededor de ETQ Reliance. Su propósito es transformar scripts aislados y conocimiento operativo disperso en una biblioteca de ingeniería estructurada, bilingüe y preparada para procesos regulados.

El proyecto no se limita a almacenar código. Cada solución documenta qué problema resuelve, cómo funciona, qué información consulta o modifica, cuáles son sus riesgos, cómo debe validarse y qué controles necesita antes de utilizarse en producción.

### Qué problemas busca resolver

- Scripts sin contexto, responsables o criterios claros de aceptación.
- Automatizaciones legacy difíciles de mantener o comparar.
- Consultas repetidas, procesamiento innecesario y uso ineficiente de recursos.
- Logs excesivos que ocultan los eventos realmente importantes.
- Duplicados causados por procesos que no son idempotentes.
- Diferencias de configuración entre DEV, VAL y PROD.
- Falta de evidencia para validar, recuperar o investigar una ejecución.

### Alcance técnico

| Área | Contenido de la biblioteca privada |
| --- | --- |
| **ETQScript Formulas** | Cálculos, validaciones, acciones, subformularios y lógica de workflow. |
| **Form Settings** | Fórmulas para eventos como On Open, On Refresh y On Save. |
| **EtQScript Profiles** | Utilidades reutilizables que pueden ser invocadas por múltiples formularios y Tasks. |
| **Task Profiles** | Automatizaciones programadas, procesamiento masivo, sincronización y mantenimiento controlado. |
| **SQL Server** | Consultas administrativas, diagnóstico, configuración, seguridad y soporte documental. |
| **Ingeniería operativa** | Observabilidad, métricas, manejo de errores, validación y recuperación. |

### Módulos documentados

- **Training Management:** creación y mantenimiento de Training Assignments, Course Profiles, grupos y reglas de aplicabilidad.
- **Document Control:** distribución, archivo, migración, actualización y control del ciclo documental.
- **Administration Center:** usuarios, grupos, perfiles, sesiones y tareas administrativas.
- **Compliance Obligations:** integraciones y automatizaciones relacionadas con obligaciones regulatorias.
- **Shared Workflow:** acciones, rutas y utilidades reutilizables entre módulos.

### Método de ingeniería

Cada componente sigue un ciclo verificable:

```text
Fuente recibida
      ↓
Clasificación por módulo y riesgo
      ↓
Preservación de la versión legacy
      ↓
Análisis de reglas, consultas y efectos
      ↓
Diseño de la versión optimized
      ↓
Pruebas y comparación en DEV
      ↓
Validación controlada en VAL
      ↓
Promoción aprobada a PROD
```

Los criterios principales incluyen:

- documentación separada en español e inglés;
- distinción explícita entre `legacy` y `optimized`;
- preservación de reglas de negocio observables;
- idempotencia y prevención de duplicados;
- límites de volumen y consultas acotadas;
- cierre seguro de documentos y recursos;
- métricas agregadas y logs accionables;
- manejo de errores sin ocultar fallos;
- estrategia de validación y recuperación.

### Trabajo original

La arquitectura documental, la clasificación por módulos, las explicaciones funcionales, los análisis de riesgo, las comparaciones, los planes de prueba y las propuestas de optimización son trabajo técnico y editorial propio del proyecto.

Los nombres de productos, módulos, clases y métodos se utilizan únicamente para identificar dependencias técnicas. Los manuales del proveedor no se publican ni se presentan como contenido propio. El código histórico de terceros se identifica como `legacy` y conserva su atribución correspondiente.

---

## English

### About the project

ETQ Reliance Automation Engineering is an independent initiative for organizing, analyzing, and improving solutions built around ETQ Reliance. Its purpose is to transform isolated scripts and scattered operational knowledge into a structured, bilingual engineering library suitable for regulated workflows.

The project does more than store source code. Every solution explains the problem it addresses, how it operates, what information it reads or changes, its risks, the validation it requires, and the controls needed before production use.

### Problems addressed

- Scripts with no operational context, ownership, or acceptance criteria.
- Legacy automations that are difficult to maintain or compare.
- Repeated queries, unnecessary processing, and inefficient resource use.
- Excessive logging that hides meaningful events.
- Duplicate records caused by non-idempotent processing.
- Configuration differences across DEV, VAL, and PROD.
- Missing evidence for validation, recovery, and execution analysis.

### Technical scope

| Area | Content in the private library |
| --- | --- |
| **ETQScript Formulas** | Calculations, validations, actions, subforms, and workflow logic. |
| **Form Settings** | Formulas for events such as On Open, On Refresh, and On Save. |
| **EtQScript Profiles** | Reusable utilities shared by multiple forms and Tasks. |
| **Task Profiles** | Scheduled automation, bulk processing, synchronization, and controlled maintenance. |
| **SQL Server** | Administration, diagnostics, configuration, security, and document-support queries. |
| **Operational engineering** | Observability, metrics, error handling, validation, and recovery. |

### Documented modules

- **Training Management:** creation and maintenance of Training Assignments, Course Profiles, groups, and applicability rules.
- **Document Control:** distribution, archiving, migration, updates, and document-lifecycle control.
- **Administration Center:** users, groups, profiles, sessions, and administrative Tasks.
- **Compliance Obligations:** integrations and automation related to regulatory obligations.
- **Shared Workflow:** actions, routing, and reusable cross-module utilities.

### Engineering method

Each component follows a traceable lifecycle:

```text
Received source
      ↓
Module and risk classification
      ↓
Legacy version preservation
      ↓
Business-rule, query, and effect analysis
      ↓
Optimized candidate design
      ↓
Testing and comparison in DEV
      ↓
Controlled validation in VAL
      ↓
Approved promotion to PROD
```

Core criteria include:

- separate Spanish and English documentation;
- an explicit distinction between `legacy` and `optimized`;
- preservation of observable business rules;
- idempotency and duplicate prevention;
- bounded volume and query execution;
- reliable document and resource cleanup;
- aggregated metrics and actionable logs;
- error handling that does not hide failures;
- validation and recovery strategies.

### Original work

The documentation architecture, module classification, functional explanations, risk analyses, comparisons, test plans, and optimization proposals are original engineering and editorial work produced for this project.

Product, module, class, and method names are used only to identify technical dependencies. Vendor manuals are neither published nor presented as original project content. Historical third-party code is identified as `legacy` and retains the appropriate attribution.

---

## Solicitar acceso / Request access

La documentación completa y el código se mantienen en un repositorio privado. El acceso se concede individualmente después de revisar el propósito y el alcance solicitado.

The complete documentation and source code are maintained in a private repository. Access is granted individually after reviewing the requested purpose and scope.

[Abrir una solicitud de acceso / Open an access request](https://github.com/yorzethmc/etq-reliance-automation-overview/issues/new)

Incluya únicamente / Include only:

1. Usuario de GitHub / GitHub username.
2. Propósito de la solicitud / Purpose of the request.
3. Módulo o tema requerido / Required module or topic.
4. Uso previsto de la información / Intended use of the information.

No publique información confidencial, datos personales, configuraciones internas ni detalles de producción dentro del issue.

Do not include confidential information, personal data, internal configuration, or production details in the issue.

## Límites del proyecto / Project boundaries

- No contiene documentación oficial del proveedor.
- No distribuye manuales de ETQ u Octave.
- No publica datos, configuraciones ni código de ambientes productivos.
- Ningún ejemplo debe considerarse listo para PROD sin validación independiente.

- It does not contain official vendor documentation.
- It does not distribute ETQ or Octave manuals.
- It does not publish production data, configuration, or source code.
- No example should be considered production-ready without independent validation.

## Independence notice

ETQ, ETQ Reliance, and Octave Reliance are names and trademarks of their respective owners. This independent project is not affiliated with, endorsed by, or a replacement for the vendor's official documentation, training, licensing, or support.
