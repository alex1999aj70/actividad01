# Resumen: Inteligencia Artificial y Sistemas Expertos

**Documento resumido:** presentación "Sistemas Expertos, Unidad de Competencia I: Inteligencia Artificial y Sistemas Expertos", de M. en C. Edith Cristina Herrera Luna (UAEM, Ingeniería en Computación, mayo de 2015). 34 diapositivas.
**Resumen elaborado por:** Alejandro del Jesus Diaz Lopez (matrícula 191087).

## Idea central

La unidad presenta los conceptos básicos de la inteligencia artificial (IA) y de los sistemas expertos (SE). Su punto de partida es que un problema de IA se resuelve mejor al **restringir su dominio**: no existen soluciones generales para problemas como traducir lenguaje natural o entender la voz y la visión por completo, pero si se limita el área del problema se obtiene una solución útil. La unidad se organiza en tres bloques: IA, sistemas expertos, y lenguajes y herramientas.

## 1. Inteligencia Artificial

- **Inteligencia:** conjunto de propiedades de la mente (planear, resolver problemas, razonar). Es la habilidad de tomar decisiones correctas dado un conjunto de entradas y una variedad de acciones posibles.
- **IA:** desarrollar máquinas que se comporten como si fueran inteligentes; estudiar cómo hacer que las computadoras hagan las cosas en las que, por ahora, las personas son mejores.

**Antecedentes que menciona:**

| Año | Hecho |
| --- | ----- |
| 1955 | Simon, Newell y Shaw desarrollan IPL-11, el primer lenguaje orientado a resolver problemas. Un año después crean el Logic Theorist, que demostraba teoremas matemáticos. |
| 1956 | McCarthy, Minsky y Shannon acuñan el término "inteligencia artificial" en la Conferencia de Dartmouth. Las previsiones triunfalistas a diez años no se cumplieron y las investigaciones se abandonaron casi por completo durante quince años. |
| 1973 | Colmerauer y su equipo (Universidad de Aix-Marseille) crean PROLOG. |
| 1974 | Shortliffe presenta su tesis con MYCIN, que asistía a médicos en el diagnóstico de infecciones de la sangre. |
| 1970-1980 | Crece el uso de sistemas expertos (R1/XCON, PUFF, CASNET, INTERNIST/CADUCEUS). Algunos *shells* siguen vigentes: EMYCIN, EXPERT, OPS5. |

### Reconocimiento de patrones

Disciplina científica que comenzó formalmente a finales de los años cincuenta. Resuelve problemas de identificación, pronóstico y clasificación de objetos, con base en la idea de que los objetos semejantes pertenecen a una misma clase y los diferentes a clases distintas. Distingue tres tipos de clasificación:

- **Supervisada:** hay objetos de todas las clases y se aprende de ellos.
- **No supervisada:** no se conocen las clases ni cómo se agrupan los objetos.
- **Parcialmente supervisada:** hay objetos en algunas clases y al menos una clase no tiene objetos.

También menciona la **selección de variables**, que reduce los términos con los que se describe un objeto y permite saber qué rasgos discriminan más.

### Paradigmas de programación para IA

Un paradigma es un enfoque o filosofía para diseñar soluciones. Los problemas de IA se trabajan sobre todo con paradigmas **no procedurales**.

- **Procedurales:** implementan un algoritmo, y el programador especifica con exactitud cómo debe resolverse el problema, instrucción por instrucción. No son del tipo de IA. Incluyen la programación imperativa (C, FORTRAN, Pascal, COBOL, BASIC; no es eficiente para SE) y la funcional (basada en funciones matemáticas; ejemplo: LISP).
- **No procedurales:** el programador especifica **qué** se debe lograr, no los detalles de la solución, y separan la meta de los métodos usados. Incluyen la programación declarativa (orientada a objetos, lógica y basada en reglas) y la no declarativa (basada en inducción y redes neuronales, que se entrenan).

## 2. Sistemas expertos

**Definición:** un programa de cómputo inteligente que usa conocimiento y procedimientos de inferencia para resolver problemas lo bastante difíciles como para requerir experiencia humana significativa. Usa conocimiento especializado como lo haría un especialista humano.

**Conceptos clave:**

| Concepto | Significado |
| -------- | ----------- |
| Dominio del problema | El área |
| Dominio del conocimiento | El conocimiento del especialista |
| Mecanismo de inferencia | La conclusión, el razonamiento y la respuesta |
| Ingeniero del conocimiento | Quien construye el SE |
| Ingeniería del conocimiento | El proceso de construir un SE |

**Ventajas:** mayor disponibilidad, costo reducido, peligro reducido, permanencia, experiencia múltiple, mayor confiabilidad, explicación, respuesta rápida, respuestas sólidas y sin emociones, tutoría inteligente y base de datos inteligente.

**Características:** alto desempeño, tiempo de respuesta adecuado, confiabilidad, ser comprensible y flexible. Algunos además dan un pronóstico, enumeran razones a favor y en contra, y enumeran hipótesis y las explican.

### ¿Cómo trabajar con reglas?

La ciencia cognitiva modela cómo procesamos la información. Con el Solucionador General de Problemas (GPS) de Newell y Simon surgen las **reglas de producción** del tipo SI ... ENTONCES .... Una regla es un pequeño fragmento de conocimiento, y los fragmentos se organizan con otros relacionados.

| En la mente | En un sistema de reglas |
| ----------- | ----------------------- |
| Memoria a largo plazo | Reglas almacenadas |
| Memoria a corto plazo | Conocimiento temporal o memoria activa |
| Procesador cognitivo | Reglas activadas y mecanismo de inferencia |

La **granularidad** es la cantidad de conocimiento que contienen las reglas.

### Estructura de un sistema experto

Según el diagrama de la diapositiva 25, un SE se compone de:

- **Base de conocimiento:** guarda las reglas.
- **Memoria de trabajo:** guarda los hechos.
- **Motor de inferencia:** conectado a las dos anteriores, con una **agenda** interna.
- **Módulo de explicación** y **módulo de adquisición de conocimiento:** ambos conectados al motor de inferencia.
- **Interfaz de usuario:** conectada a los dos módulos anteriores.

## 3. Lenguajes y herramientas

- **Lenguaje para SE:** ofrece formas robustas y flexibles de representar el conocimiento. Es un traductor de comandos con una sintaxis específica que incluye un mecanismo de inferencia que ejecuta las instrucciones.
- **Herramienta:** un lenguaje asociado con programas de utilería que facilitan el desarrollo, la depuración y el uso de las aplicaciones.
- **Shell:** una herramienta de propósito especial en la que el usuario solo proporciona la base de conocimiento.

### Métodos generales de inferencia

- **Encadenamiento hacia adelante:** va de los hechos a la conclusión.
- **Encadenamiento hacia atrás:** va de una hipótesis a los hechos, para probar una conclusión. Una hipótesis es un hecho cuya veracidad está en duda y necesita establecerse.

**Ejemplo (cruzar una calle):** la regla `Luz_roja` dice SI la luz es roja ENTONCES alto, y la regla `Luz_verde` dice SI la luz es verde ENTONCES siga. La parte condicional (lado izquierdo) es el **antecedente** y la acción (lado derecho) es la **consecuencia**.

## Recomendaciones del documento

Para ampliar el tema, el documento sugiere investigar el motor de inferencia de un SE existente, buscar una herramienta o lenguaje para representar un SE, estudiar el shell **JESS** (Java Expert System Shell) y usar el programa **Weka** como primera vista a una herramienta de aprendizaje.

## Referencias principales del documento

- Giarratano, J. C. y Riley, G. *Expert Systems: Principles and Programming* (4.ª ed., 2004).
- Lucas, P. y van der Gaag, L. *Principles of Expert Systems* (1991).
- Russell, S. y Norvig, P. *Artificial Intelligence: A Modern Approach* (2.ª ed., 2002).
