<p align="center">
  <img src="https://raw.githubusercontent.com/Netec-Mx/261026-IA-SK-PC-Priv/main/assets/LogoNetec.png" alt="NETEC" width="180" />
</p>

# Diseño y desarrollo de Agent Skills con ChatGPT, Codex y Amazon Bedrock

Este curso desarrolla competencias para diseñar, construir, integrar, probar y mantener Agent Skills reutilizables que permitan estandarizar procedimientos y extender las capacidades de asistentes y agentes de inteligencia artificial.

Los participantes aprenderán los fundamentos y arquitectura de Agent Skills y aplicarán estos principios principalmente mediante ChatGPT y Codex, incorporando instrucciones especializadas, referencias, scripts y herramientas.

Considerando que el cliente trabaja con agentes desarrollados en Amazon Bedrock y utiliza Amazon API Gateway para la gestión y publicación de sus APIs, el curso también aborda la integración de Agent Skills con capacidades externas disponibles en AWS. Se utilizarán Amazon API Gateway y Amazon Bedrock Agents como componentes de referencia para construir workflows que combinen Skills, APIs y agentes, sin asumir el uso de Agent Skills directamente dentro de AWS.

## Accesos rápidos

- [**Setup Guide del curso**](https://github.com/Netec-Mx/261026-IA-SK-PC-Priv/blob/main/SETUP_GUIDE.md)
- [Laboratorios por capítulo](#lista-de-laboratorios)

## Estructura

- `SETUP_GUIDE.md`: guía de instalación y preparación del entorno.
- `CapituloXX/README.md`: guía de laboratorio por capítulo.

## Lista de laboratorios

### Capítulo 1

- [Construir una Skill para generar documentación técnica](Capitulo01/README.md#construir-una-skill-para-generar-documentación-técnica)
  - Descripción: Crear desde cero una Agent Skill que transforme información técnica de un componente o servicio en documentación estandarizada para el equipo. Definir su propósito, criterios de activación, estructura de SKILL.md, secuencia de trabajo y formato esperado del documento. Ejecutarla con diferentes entradas para comprobar que mantiene una estructura y criterios consistentes.
  - Duración estimada: 60 min
- [Crear una Skill apoyada en estándares y documentación de referencia](Capitulo01/README.md#crear-una-skill-apoyada-en-estándares-y-documentación-de-referencia)
  - Descripción: Construir una Skill para responder consultas sobre estándares técnicos de un proyecto utilizando archivos de referencia proporcionados durante la práctica. Organizar las fuentes para evitar incluir todo el contenido dentro de SKILL.md y comprobar que la Skill localiza y utiliza únicamente la información relevante para cada solicitud.
  - Duración estimada: 30 min
  - [Ver capítulo completo](Capitulo01/README.md)

### Capítulo 2

- [Crear una Skill para clasificar y gestionar incidencias técnicas](Capitulo02/README.md#crear-una-skill-para-clasificar-y-gestionar-incidencias-técnicas)
  - Descripción: Construir una Skill que analice la descripción de una incidencia y determine su categoría, prioridad y siguiente acción utilizando criterios definidos. Incorporar rutas diferentes según el tipo y severidad del problema, solicitar información adicional cuando el contexto sea insuficiente y producir una salida estructurada para facilitar su seguimiento.
  - Duración estimada: 50 min
- [Crear una Skill con validación automatizada mediante un script](Capitulo02/README.md#crear-una-skill-con-validación-automatizada-mediante-un-script)
  - Descripción: Construir una Skill que reciba un archivo de configuración, utilice un script para comprobar automáticamente requisitos técnicos definidos y posteriormente interprete los resultados para generar un reporte de cumplimiento. Comparar qué validaciones conviene ejecutar mediante código y cuáles requieren análisis del modelo.
  - Duración estimada: 40 min
  - [Ver capítulo completo](Capitulo02/README.md)

### Capítulo 3

- [Automatizar una revisión de código con Codex](Capitulo03/README.md#automatizar-una-revisión-de-código-con-codex)
  - Descripción: Crear una Skill que permita a Codex revisar cambios de código de acuerdo con estándares definidos por el equipo. Analizar modificaciones, detectar posibles problemas, clasificar los hallazgos por severidad y producir recomendaciones estructuradas que faciliten la revisión humana.
  - Duración estimada: 45 min
- [Generar pruebas para una modificación de código](Capitulo03/README.md#generar-pruebas-para-una-modificación-de-código)
  - Descripción: Construir una Skill que analice un cambio realizado en una funcionalidad, identifique escenarios que requieren pruebas y genere los casos correspondientes. Ejecutar las pruebas disponibles, interpretar los resultados y señalar los escenarios que necesitan validación adicional.
  - Duración estimada: 45 min
- [Investigar la causa de un fallo mediante Codex](Capitulo03/README.md#investigar-la-causa-de-un-fallo-mediante-codex)
  - Descripción: Utilizar una Skill de troubleshooting ante un escenario donde una aplicación presenta un comportamiento inesperado. Analizar código, mensajes de error y contexto disponible; formular hipótesis; buscar evidencia que permita descartarlas o confirmarlas y generar una conclusión diferenciando síntomas, causa probable y acciones correctivas.
  - Duración estimada: 45 min
  - [Ver capítulo completo](Capitulo03/README.md)

### Capítulo 4

- [Integrar una Skill con una API publicada mediante Amazon API Gateway](Capitulo04/README.md#integrar-una-skill-con-una-api-publicada-mediante-amazon-api-gateway)
  - Descripción: Utilizar una Agent Skill para resolver una tarea que requiera información o una operación proporcionada por una API previamente publicada mediante Amazon API Gateway. Definir cuándo debe utilizarse la capacidad externa, enviar los parámetros requeridos, procesar la respuesta e incorporarla al workflow de la Skill, contemplando errores y respuestas incompletas.
  - Duración estimada: 37 min
- [Construir un workflow que combine una Skill con capacidades de AWS](Capitulo04/README.md#construir-un-workflow-que-combine-una-skill-con-capacidades-de-aws)
  - Descripción: Construir un workflow en el que una Agent Skill coordine una tarea técnica utilizando una API administrada mediante Amazon API Gateway y una capacidad proporcionada por un agente de Amazon Bedrock. Definir qué responsabilidad corresponde a cada componente, intercambiar el contexto requerido y consolidar los resultados, incorporando manejo de errores y controles para evitar ejecuciones incorrectas.
  - Duración estimada: 60 min
  - [Ver capítulo completo](Capitulo04/README.md)

### Capítulo 5

- [Diseñar y ejecutar una batería de pruebas para una Skill integrada](Capitulo05/README.md#diseñar-y-ejecutar-una-batería-de-pruebas-para-una-skill-integrada)
  - Descripción: Seleccionar una Skill que dependa de capacidades externas y construir pruebas que contemplen solicitudes válidas, solicitudes fuera de alcance, información incompleta, respuestas inesperadas de una API y fallos de una dependencia externa. Evaluar su comportamiento, identificar errores y ajustar la Skill con base en los resultados obtenidos.
  - Duración estimada: 40 min
- [Evolucionar una Skill sin introducir regresiones](Capitulo05/README.md#evolucionar-una-skill-sin-introducir-regresiones)
  - Descripción: Incorporar un nuevo requerimiento a una Skill previamente probada, identificar los componentes que deben modificarse y generar una nueva versión. Ejecutar nuevamente los casos de prueba, comparar los resultados y documentar los cambios antes de dejar disponible la nueva versión.
  - Duración estimada: 30 min
  - [Ver capítulo completo](Capitulo05/README.md)

## Flujo de colaboración

- Trabajar en `changes_course`.
- Crear Pull Request hacia `main`.
- Merge por `Squash and merge`.

---

*Material didáctico preparado por Global K, S.A. de C.V.*
