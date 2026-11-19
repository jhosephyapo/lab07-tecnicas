# Tarea: Mi prompt avanzado 
## Tarea elegida 
Diseñar las clases de un sistema de notas

## Version 1: prompt basico 
```text 
Diseña las clases de un sistema de notas para una escuela. Debe permitir registrar estudiantes, cursos y notas. Indica qué atributos tendría cada clase y cómo se relacionan entre sí.
```
- Técnica agregada: Descomposición del problema en clases y atributos.
- Por qué: Ayuda a identificar los elementos principales del sistema sin complicar el diseño.
- Qué mejoró: La respuesta queda clara y fácil de empezar: identifica estudiantes, cursos y notas, y pide explicar sus relaciones.
## Version 2 
```text 
Diseña las clases de un sistema de notas que permita gestionar estudiantes, docentes, cursos y evaluaciones. Cada evaluación debe tener una fecha, un puntaje máximo y una nota por estudiante. Propón los atributos, métodos y relaciones necesarios, e indica cómo validar que una nota esté dentro del rango permitido.
```
- Técnica agregada: Incorporación de requisitos funcionales y validaciones.
- Por qué: Un sistema de notas debe considerar quién enseña, qué se evalúa y qué límites tienen las calificaciones.
- Qué mejoró: La respuesta guía un diseño más completo al incluir docentes, evaluaciones, métodos y validación del rango de notas.
## Version 3: prompt final 
```text 
Actúa como diseñador de software orientado a objetos. Diseña las clases de un sistema de notas para una escuela.

Descompón la solución en clases, responsabilidades, atributos, métodos, relaciones y reglas de negocio. Incluye como mínimo Estudiante, Docente, Curso, Evaluación y Nota. Asegúrate de que las notas estén dentro del rango permitido, que el estudiante esté inscrito antes de recibir una nota y que no haya notas duplicadas para la misma evaluación.

Presenta la respuesta con estas secciones: resumen, clases, relaciones y multiplicidades, validaciones y ejemplo de uso en pseudocódigo.

Incluye un ejemplo breve del formato esperado: Estudiante: atributos id y nombre; método inscribirse(curso).

Al final, revisa que estén incluidas todas las clases y reglas solicitadas, y corrige cualquier omisión.
```
- Técnica agregada: Role prompting, descomposición, prompt estructurado y few-shot.
- Por qué: Se definió el rol, se dividió la tarea, se indicó un formato y se incluyó un ejemplo.
- Qué mejoró: La instrucción quedó más concreta y orientó una respuesta ordenada y detallada.

## Tecnicas usadas en el prompt final 
| Tecnica | Parte del promt final | Para que sirve|
|------|-----------------|-------------------------|
| Role prompting  |	“Actúa como diseñador de software orientado a objetos.”|	Define el rol desde el cual se aborda el diseño. |
| Descomposición | “Descompón la solución en clases, responsabilidades, atributos, métodos, relaciones y reglas de negocio.”| Divide la tarea en componentes para cubrirla mejor.| 
| Prompt estructurado  | “Presenta la respuesta con estas secciones: resumen, clases, relaciones y multiplicidades, validaciones y ejemplo de uso en pseudocódigo.”| Organiza la respuesta y facilita su revisión.| 
| Few-shot | “Estudiante: atributos id y nombre; método inscribirse(curso).”| Muestra un ejemplo del formato y el nivel de detalle esperado.| 

## Evaluacion del resultado 
| Criterio | Aciertos (de 5) | 
|------|-----------------|
| Incluye las clases Estudiante, Docente, Curso, Evaluación y Nota. |si |
| Describe atributos y métodos para las clases. | si| 
|Explica las relaciones y multiplicidades entre las clases. | si| estructurado|
|Incluye validaciones para el rango de notas, la inscripción y las notas duplicadas.  | si|
|Presenta un ejemplo de uso en pseudocódigo.  | si| 

## Por que elegi estas tecnicas

Elegí role prompting, descomposición, prompt estructurado y few-shot porque ayudan directamente a diseñar las clases del sistema: el rol orienta la respuesta, la descomposición cubre sus componentes, la estructura ordena la explicación y el ejemplo aclara el formato esperado. No elegí técnicas como chain of thought o autocrítica porque no eran necesarias para obtener una respuesta clara y completa; las indicaciones concretas y los criterios del prompt bastaban para guiar el resultado.
