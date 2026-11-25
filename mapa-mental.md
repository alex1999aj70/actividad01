# Mapa mental: Inteligencia, IA y sistemas expertos

Este código sirve para generar la base del mapa mental en Excalidraw:

1. Abre https://excalidraw.com/
2. Menú de herramientas: **Más herramientas → Mermaid a Excalidraw** (también **Insertar → Mermaid**, según la versión).
3. Pega el código de abajo, inserta y acomoda los elementos.
4. Exporta el resultado como imagen o guarda el archivo `.excalidraw`, y súbelo al repositorio.

```mermaid
flowchart LR
  IA((Inteligencia Artificial))

  IA --> INT[Inteligencia]
  INT --> I1[RAE: entender y resolver problemas]
  INT --> I2[Psicologia: adaptarse y aprender de la experiencia]
  INT --> I3[Autores: Spearman, Cattell, Gardner, Sternberg]
  INT --> I4[McCarthy: parte computacional de lograr metas]

  IA --> DEF[Definiciones de IA]
  DEF --> D1[McCarthy: ciencia e ingenieria de maquinas inteligentes]
  DEF --> D2[Cuatro enfoques: pensar y actuar, como humanos y racionalmente]
  DEF --> D3[Definicion de trabajo: habilidad para resolver problemas del entorno]

  IA --> HIS[Historia]
  HIS --> H1[1950 Test de Turing]
  HIS --> H2[1956 Dartmouth]
  HIS --> H3[1965 DENDRAL]
  HIS --> H4[1980 XCON]
  HIS --> H5[1987 caida de maquinas LISP]

  IA --> SE[Sistemas expertos]
  SE --> S1[Base de conocimiento: hechos y reglas]
  SE --> S2[Motor de inferencia: adelante y atras]
  SE --> S3[Interfaz y modulo de explicacion]
  SE --> S4[Tipos: reglas, casos, bayesianos, difusos, hibridos]

  IA --> RAM[Otras ramas]
  RAM --> R1[Redes neuronales]
  RAM --> R2[Algoritmos geneticos]
  RAM --> R3[Aprendizaje automatico]
```

## Mismo contenido en forma de lista

- **Inteligencia artificial**
  - **Inteligencia**: RAE (entender y resolver problemas) · Psicología (adaptarse, aprender de la experiencia) · Autores (Spearman, Cattell, Gardner, Sternberg) · McCarthy (parte computacional de lograr metas).
  - **Definiciones de IA**: McCarthy · Cuatro enfoques de Russell y Norvig · Definición de trabajo del curso.
  - **Historia**: 1950 test de Turing · 1956 Dartmouth · 1965 DENDRAL · 1980 XCON · 1987 caída de las máquinas LISP.
  - **Sistemas expertos**: base de conocimiento · motor de inferencia · interfaz y explicación · tipos.
  - **Otras ramas**: redes neuronales · algoritmos genéticos · aprendizaje automático.
