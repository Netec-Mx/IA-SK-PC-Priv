<a href="https://netec.com">
  <img src="https://static.wixstatic.com/media/96edd2_934dddb3230b4b16b1d1c56c51143738~mv2.png" alt="Logo de Netec" width="300"/>
</a>

# Diseño y desarrollo de Agent Skills con ChatGPT, Codex y Amazon Bedrock

## Plataforma de laboratorios

Este curso desarrolla competencias para diseñar, construir, integrar, probar y mantener Agent Skills reutilizables que permitan estandarizar procedimientos y extender las capacidades de asistentes y agentes de inteligencia artificial.

Los participantes aprenderán los fundamentos y arquitectura de Agent Skills y aplicarán estos principios principalmente mediante ChatGPT y Codex, incorporando instrucciones especializadas, referencias, scripts y herramientas.

Considerando que el cliente trabaja con agentes desarrollados en Amazon Bedrock y utiliza Amazon API Gateway para la gestión y publicación de sus APIs, el curso también aborda la integración de Agent Skills con capacidades externas disponibles en AWS. Se utilizarán Amazon API Gateway y Amazon Bedrock Agents como componentes de referencia para construir workflows que combinen Skills, APIs y agentes, sin asumir el uso de Agent Skills directamente dentro de AWS.



## Lista de laboratorios

Cada uno de estos laboratorios está diseñado para ofrecerte una experiencia práctica. Haz clic en los enlaces para comenzar.

### Capítulo 1

#### [Práctica 1. Construir una Skill para generar documentación técnica](Capitulo01/README.md#construir-una-skill-para-generar-documentación-técnica)

- Descripción: Crear desde cero una Agent Skill que transforme información técnica de un componente o servicio en documentación estandarizada para el equipo. Definir su propósito, criterios de activación, estructura de SKILL.md, secuencia de trabajo y formato esperado del documento. Ejecutarla con diferentes entradas para comprobar que mantiene una estructura y criterios consistentes.
- ⏱️ Duración estimada: 60 min.

#### [Práctica 2. Crear una Skill apoyada en estándares y documentación de referencia](Capitulo01/README.md#crear-una-skill-apoyada-en-estándares-y-documentación-de-referencia)

- Descripción: Construir una Skill para responder consultas sobre estándares técnicos de un proyecto utilizando archivos de referencia proporcionados durante la práctica. Organizar las fuentes para evitar incluir todo el contenido dentro de SKILL.md y comprobar que la Skill localiza y utiliza únicamente la información relevante para cada solicitud.
- ⏱️ Duración estimada: 30 min.

### Capítulo 2

#### [Práctica 3. Crear una Skill para clasificar y gestionar incidencias técnicas](Capitulo02/README.md#crear-una-skill-para-clasificar-y-gestionar-incidencias-técnicas)

- Descripción: Construir una Skill que analice la descripción de una incidencia y determine su categoría, prioridad y siguiente acción utilizando criterios definidos. Incorporar rutas diferentes según el tipo y severidad del problema, solicitar información adicional cuando el contexto sea insuficiente y producir una salida estructurada para facilitar su seguimiento.
- ⏱️ Duración estimada: 50 min.

#### [Práctica 4. Crear una Skill con validación automatizada mediante un script](Capitulo02/README.md#crear-una-skill-con-validación-automatizada-mediante-un-script)

- Descripción: Construir una Skill que reciba un archivo de configuración, utilice un script para comprobar automáticamente requisitos técnicos definidos y posteriormente interprete los resultados para generar un reporte de cumplimiento. Comparar qué validaciones conviene ejecutar mediante código y cuáles requieren análisis del modelo.
- ⏱️ Duración estimada: 40 min.

### Capítulo 3

#### [Práctica 5. Automatizar una revisión de código con Codex](Capitulo03/README.md#automatizar-una-revisión-de-código-con-codex)

- Descripción: Crear una Skill que permita a Codex revisar cambios de código de acuerdo con estándares definidos por el equipo. Analizar modificaciones, detectar posibles problemas, clasificar los hallazgos por severidad y producir recomendaciones estructuradas que faciliten la revisión humana.
- ⏱️ Duración estimada: 45 min.

#### [Práctica 6. Generar pruebas para una modificación de código](Capitulo03/README.md#generar-pruebas-para-una-modificación-de-código)

- Descripción: Construir una Skill que analice un cambio realizado en una funcionalidad, identifique escenarios que requieren pruebas y genere los casos correspondientes. Ejecutar las pruebas disponibles, interpretar los resultados y señalar los escenarios que necesitan validación adicional.
- ⏱️ Duración estimada: 45 min.

#### [Práctica 7. Investigar la causa de un fallo mediante Codex](Capitulo03/README.md#investigar-la-causa-de-un-fallo-mediante-codex)

- Descripción: Utilizar una Skill de troubleshooting ante un escenario donde una aplicación presenta un comportamiento inesperado. Analizar código, mensajes de error y contexto disponible; formular hipótesis; buscar evidencia que permita descartarlas o confirmarlas y generar una conclusión diferenciando síntomas, causa probable y acciones correctivas.
- ⏱️ Duración estimada: 45 min.

### Capítulo 4

#### [Práctica 8. Integrar una Skill con una API publicada mediante Amazon API Gateway](Capitulo04/README.md#integrar-una-skill-con-una-api-publicada-mediante-amazon-api-gateway)

- Descripción: Utilizar una Agent Skill para resolver una tarea que requiera información o una operación proporcionada por una API previamente publicada mediante Amazon API Gateway. Definir cuándo debe utilizarse la capacidad externa, enviar los parámetros requeridos, procesar la respuesta e incorporarla al workflow de la Skill, contemplando errores y respuestas incompletas.
- ⏱️ Duración estimada: 37 min.

#### [Práctica 9. Construir un workflow que combine una Skill con capacidades de AWS](Capitulo04/README.md#construir-un-workflow-que-combine-una-skill-con-capacidades-de-aws)

- Descripción: Construir un workflow en el que una Agent Skill coordine una tarea técnica utilizando una API administrada mediante Amazon API Gateway y una capacidad proporcionada por un agente de Amazon Bedrock. Definir qué responsabilidad corresponde a cada componente, intercambiar el contexto requerido y consolidar los resultados, incorporando manejo de errores y controles para evitar ejecuciones incorrectas.
- ⏱️ Duración estimada: 60 min.

### Capítulo 5

#### [Práctica 10. Diseñar y ejecutar una batería de pruebas para una Skill integrada](Capitulo05/README.md#diseñar-y-ejecutar-una-batería-de-pruebas-para-una-skill-integrada)

- Descripción: Seleccionar una Skill que dependa de capacidades externas y construir pruebas que contemplen solicitudes válidas, solicitudes fuera de alcance, información incompleta, respuestas inesperadas de una API y fallos de una dependencia externa. Evaluar su comportamiento, identificar errores y ajustar la Skill con base en los resultados obtenidos.
- ⏱️ Duración estimada: 40 min.

#### [Práctica 11. Evolucionar una Skill sin introducir regresiones](Capitulo05/README.md#evolucionar-una-skill-sin-introducir-regresiones)

- Descripción: Incorporar un nuevo requerimiento a una Skill previamente probada, identificar los componentes que deben modificarse y generar una nueva versión. Ejecutar nuevamente los casos de prueba, comparar los resultados y documentar los cambios antes de dejar disponible la nueva versión.
- ⏱️ Duración estimada: 30 min.

Duración total de los laboratorios: 482 minutos (8 horas y 2 minutos).

---

## 📬 Contacto y más información

Si tienes alguna pregunta o necesitas más detalles, no dudes en [contactarnos](mailto:soporte@netec.com). También puedes encontrar más recursos en nuestra [página](https://netec.com).

---

¡Gracias por visitar nuestra plataforma! No olvides revisar todos los laboratorios y comenzar tu viaje de aprendizaje hoy mismo.
