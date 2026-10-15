# sistema-gestion-tareas-proyectos
Sistema digital para organizar tareas, proyectos y dar seguimiento a sus avances.
Sistema de Gestión de Tareas y Proyectos

1. Descripción general:
El Sistema de Gestión de Tareas y Proyectos es una propuesta de aplicación digital para organizar proyectos, registrar tareas y consultar su estado de avance desde un solo lugar. La idea es facilitar el seguimiento del trabajo, reducir la pérdida de información y ayudar a identificar las actividades pendientes.
2. Problema que busca resolver:
Cuando las tareas se administran únicamente por mensajes, notas sueltas o conversaciones, puede ser difícil saber quién debe realizar cada actividad, cuál es su fecha límite y qué queda pendiente. El sistema propone reunir esa información en un espacio organizado y fácil de consultar.
3. Objetivo:
Diseñar una  base técnica para una aplicación que permita registrar proyectos y tareas, asignar responsables, definir prioridades y dar seguimiento al progreso.
4. Funcionalidades principales previstas:
- Registrar y consultar proyectos.
- Crear tareas asociadas a un proyecto.
- Describir cada tarea y asignar prioridad.
- Indicar el estado de una tarea: pendiente, en proceso o completada.
- Registrar responsable y fecha límite.
- Consultar el avance general del proyecto.

5. Arquitectura propuesta:
Se propone una arquitectura de tres capas:
- Presentación (frontend): interfaz con formularios, listados y vistas de seguimiento. Recoge las acciones del usuario y muestra los resultados.
- Lógica de aplicación (backend): valida los datos, aplica las reglas del sistema y procesa las solicitudes del frontend.
- Persistencia (base de datos): almacena usuarios, proyectos y tareas de forma organizada.

Organización frontend/backend:

El frontend enviaría solicitudes al backend mediante una API HTTP, preferiblemente REST, usando JSON para intercambiar datos. El backend validaría cada solicitud, aplicaría las reglas de negocio y consultaría o actualizaría la base de datos. Luego devolvería una respuesta que el frontend presentaría al usuario. La base de datos no debería ser accedida directamente desde el navegador.
6. Herramientas previstas:
- Git para registrar cambios y recuperar versiones.
- GitHub para alojar el repositorio y colaborar.
- GitHub Issues para documentar incidencias y tareas pendientes.
- GitHub Projects para visualizar el estado del trabajo.
- Markdown para documentar el proyecto.
- UML para representar los requisitos y el diseño antes de implementar.
7. Registro de cambios y avances:
1. Se delimitó el problema que atenderá el sistema y se redactó su objetivo.
2. Se organizaron las funcionalidades principales previstas.
3. Se definió una arquitectura inicial separando presentación, lógica y persistencia.
4. Se documentó la comunicación prevista entre frontend y backend mediante una API.
5. Se estableció el uso de GitHub Issues y Projects para dar seguimiento a pendientes y riesgos.
8. Seguimiento mediante Issues:
1. [Documentación] Confirmar tecnologías del sistema
Descripción: seleccionar y justificar las tecnologías que se utilizarán en frontend, backend y base de datos.
Criterio de cierre: el README indica las tecnologías elegidas y la razón de la elección.
Etiquetas sugeridas: documentación, decisión técnica.
2. [Diseño] Completar diagramas UML
Descripción: revisar los actores, casos de uso, entidades y relaciones principales.
Criterio de cierre: los diagramas corresponden con los requisitos documentados.
Etiquetas sugeridas: UML, diseño.
3. [Riesgo] Definir validación y manejo de errores
Descripción: especificar cómo se manejarán campos vacíos, fechas inválidas, tareas inexistentes y errores de comunicación.
Criterio de cierre: se documentan reglas y respuestas esperadas.
Etiquetas sugeridas: riesgo, backend.
4. [Pendiente] Preparar pruebas funcionales
Descripción: definir pruebas para crear, consultar, actualizar y completar tareas.
Criterio de cierre: cada función prevista cuenta con pasos de prueba y resultado esperado.
Etiquetas sugeridas: pruebas, pendiente.

9. Organización del tablero de GitHub Projects:
Usar columnas que representen el estado real de cada actividad:
- Pendiente: aún no iniciada.
- En progreso: trabajo iniciado y no terminado.
- En revisión: requiere validación.
- Completada: finalizada y revisada.
10. Nota técnica de versión:

Esta versión reúne la descripción del problema, el objetivo, las funcionalidades previstas, la arquitectura propuesta y una estrategia básica para controlar cambios y tareas. También establece cuatro asuntos que requieren seguimiento mediante Issues.

Los cambios controlados en esta etapa corresponden a la organización y documentación del alcance técnico. No se afirma que exista una aplicación funcional si todavía no se ha implementado ni probado. Quedan pendientes la confirmación de las tecnologías, la finalización de los diagramas UML, la definición detallada de validaciones y la preparación de pruebas funcionales.

Próximo paso técnico: confirmar el stack tecnológico, crear la estructura inicial del repositorio y desarrollar una primera función pequeña que permita registrar y consultar una tarea. Después se deberán ejecutar pruebas y documentar los resultados.

11. Datos que deben completarse antes de entregar:

- Enlace real del repositorio: [https://github.com/Franciscoguz05/sistema-gestion-tareas-proyectos].
- Nombre y fecha de la versión publicada, si se crea una etiqueta o reléase.
- Captura del README.md dentro de GitHub.
- Captura de los cuatro Issues creados en el repositorio.
- Captura del tablero de GitHub Projects con estados actualizados.
- Ajustar el registro de cambios y los estados para que coincidan con lo que realmente se hizo.

12. Control de versions:
Se recomienda guardar el documento y el README con Git, usar mensajes de confirmación claros y crear una etiqueta de versión cuando la documentación haya sido revisada. Ejemplo de mensaje de commit: docs: documentar cierre técnico inicial.
