# Guion del video: Sistemas expertos

**Integrante(s):** [Nombre completo]
**Matrícula:** [Matrícula]
**Duración estimada:** 9 a 10 minutos

**Liga del video (YouTube):** [pegar aquí la liga cuando lo subas]

---

## Antes de grabar

- Pregunta al profesor sobre la vestimenta adecuada y si el video debe ser público o no listado.
- Al inicio y al final del video debes verte **de cuerpo entero**. En la parte intermedia puedes mostrar solo las diapositivas.
- Lee el guion en voz alta dos o tres veces antes de grabar. Evita las muletillas ("este...", "o sea", "eeeh"): haz una pausa corta en lugar de rellenar el silencio.
- Habla despacio. El texto está escrito para decirse, no para leerse palabra por palabra.
- Sube el video a YouTube y comprueba que se abre sin iniciar sesión.

---

## Inicio (cuerpo entero) · 0:00 a 0:30

*[Estás de pie, de cuerpo entero, mirando a la cámara.]*

Buenos días. Mi nombre es [nombre], de la Facultad de Ciencias de la Información de la UNACAR. En este video voy a explicar qué es un sistema experto. Veremos qué es el conocimiento, cómo se guarda en una base de conocimiento, cómo razona un motor de inferencia, la historia de estos sistemas y sus tipos.

## Diapositiva 2: punto de partida · 0:30 a 1:15

Para empezar, ubiquemos los sistemas expertos dentro de la inteligencia artificial. John McCarthy la definió como la ciencia y la ingeniería de hacer máquinas inteligentes, especialmente programas de cómputo inteligentes. En el curso trabajamos con una definición más sencilla: la inteligencia artificial es la habilidad de un individuo para resolver problemas de su entorno. Los sistemas expertos son una rama de la IA que resuelve problemas usando el conocimiento de un especialista.

## Diapositiva 3: qué es un sistema experto · 1:15 a 2:00

Un sistema experto es un sistema informático que simula el aprendizaje, el razonamiento y la acción de un experto humano en una rama de la ciencia. Según Wikipedia, emula la toma de decisiones de un experto, razonando sobre conocimiento representado sobre todo con reglas del tipo si-entonces. En pocas palabras, es un programa que guarda el conocimiento de un especialista, lo aplica para resolver problemas de un área y puede explicar cómo llegó a su conclusión.

## Diapositiva 4: conocimiento · 2:00 a 2:50

Todo parte del conocimiento. No es lo mismo un dato, una información y un conocimiento. Un dato es un valor sin contexto, por ejemplo 38,5. La información le da significado: el paciente tiene 38,5 grados de temperatura. El conocimiento nos dice qué hacer con esa información: si hay fiebre y tos, hay que buscar una infección. El reto está en la ingeniería del conocimiento: extraer lo que sabe el experto y llevarlo a una forma que la computadora pueda usar. Es difícil, porque los expertos son escasos y parte de lo que saben es intuitivo.

## Diapositiva 5: base de conocimiento · 2:50 a 3:50

La base de conocimiento guarda los hechos y las reglas del dominio. Aquí vemos un ejemplo en Prolog, el lenguaje que usamos en el curso. Los hechos dicen que el paciente uno tiene fiebre y tos. La regla dice que un paciente tiene infección si tiene fiebre y tiene tos. Es la parte del sistema que cambia de un problema a otro, y se mejora agregándole más conocimiento. Los primeros sistemas, como MYCIN, usaban afirmaciones planas. Los sistemas posteriores organizan el conocimiento en clases y objetos.

## Diapositiva 6: motor de inferencia · 3:50 a 4:50

El motor de inferencia aplica las reglas a los hechos conocidos para obtener conclusiones nuevas. Además, puede explicar la cadena de reglas que utilizó. Existen dos formas principales de razonar. El encadenamiento hacia adelante parte de los datos: cuando los datos cumplen una regla, el sistema la dispara y agrega la conclusión. Por ejemplo, de "Sócrates es hombre" concluye "Sócrates es mortal". El encadenamiento hacia atrás parte de una posible conclusión y comprueba si se cumplen sus condiciones; si falta un dato, se lo pregunta al usuario. Este es el que usa Prolog por defecto.

## Diapositiva 7: arquitectura · 4:50 a 5:30

Así se ve la arquitectura completa. El usuario habla con una interfaz, la interfaz con el motor de inferencia y el motor consulta la base de conocimiento. Además hay un módulo de explicación, que muestra cómo se llegó a la conclusión, y un módulo de adquisición de conocimiento, con el que el experto agrega y corrige reglas. El motor y la interfaz se pueden reutilizar; lo que cambia con cada problema es la base de conocimiento.

## Diapositiva 8: línea de tiempo · 5:30 a 6:50

Veamos su historia. En 1956, en el taller de Dartmouth, nace el campo de la inteligencia artificial. Hacia 1965, Edward Feigenbaum y su equipo en Stanford presentan los primeros sistemas expertos, con DENDRAL, que identificaba moléculas orgánicas. En los años setenta aparece MYCIN, que diagnosticaba infecciones. En 1980 el sistema XCON, de la empresa DEC, empieza a configurar computadoras y llega a ahorrar unos 25 millones de dólares al año. En 1981, Japón lanza su proyecto de Quinta Generación, que impulsa el interés mundial. En 1987 se hunde el mercado de las máquinas LISP, y en los años noventa el término "sistema experto" casi desaparece. A partir del año 2000, sus ideas siguen en los motores de reglas de negocio y conviven con el aprendizaje automático.

## Diapositiva 9: tipos · 6:50 a 7:50

Hay varias formas de clasificarlos. Por la técnica de razonamiento, tenemos los basados en reglas, que usan si-entonces; los basados en casos, que comparan con problemas ya resueltos; los basados en redes bayesianas, que manejan probabilidades; los difusos, que usan lógica difusa para datos imprecisos; y los híbridos con redes neuronales, que combinan reglas y aprendizaje. Por la tarea que resuelven, hay sistemas de interpretación, como PROSPECTOR; de diagnóstico, como MYCIN; de diseño, como DENDRAL y R1; de monitoreo, como REACTOR, para reactores nucleares; y de control de procesos en tiempo real.

## Diapositiva 10: ventajas y limitaciones · 7:50 a 8:30

Entre sus ventajas, están siempre disponibles, responden rápido, explican sus soluciones y cuestan menos por usuario que un experto humano. Entre sus limitaciones, es difícil obtener el conocimiento del experto, el conocimiento es superficial y de dominio cerrado, con muchas reglas es difícil verificar que no se contradigan, y es complicado integrarlos con sistemas ya existentes.

## Diapositiva 11: conclusiones · 8:30 a 9:00

*[Puedes mostrar la diapositiva o pasar a cámara completa.]*

Para cerrar: un sistema experto es una base de conocimiento más un motor de inferencia para resolver problemas de un dominio. Tuvieron su auge en los años ochenta, pero sus ideas siguen vivas en los motores de reglas de las empresas. Sus límites llevaron a combinarlos con el aprendizaje automático.

## Cierre (cuerpo entero) · 9:00 a 9:40

*[Vuelves a cuadro, de pie y de cuerpo entero.]*

Como conclusión personal: [escribe aquí en una o dos frases qué aprendiste, por ejemplo qué te pareció más interesante de cómo razona un sistema experto, o para qué problema de tu entorno lo usarías]. Gracias por su atención.

---

## Fuentes (mostrar la diapositiva 12 unos segundos)

- J. McCarthy, *What is Artificial Intelligence?* (2007)
- Wikipedia: "Expert system" y "Xcon"
- zsjunai.github.io/history-of-ai: "Expert systems era"
- UNIR: ¿Qué es un sistema experto?
- TechTarget: "Expert system"
- Britannica: "Edward Albert Feigenbaum"
- IBM: historia de la inteligencia artificial
- Material del curso: actividades-ia
