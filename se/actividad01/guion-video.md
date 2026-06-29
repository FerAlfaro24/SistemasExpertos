# Guion — Video Presentación: Sistemas Expertos
**Fernando Alfaro Montalvo | Matrícula 221204**

**Liga al video:** *(subir a YouTube y colocar la liga aquí)*

---

## Indicaciones de producción

- Apertura y cierre: cuerpo entero, vestimenta formal (camisa/polo, pantalón de vestir).
- Desarrollo: puedes centrarte en la pantalla con la presentación.
- Duración estimada: 8–12 minutos.
- Evitar muletillas: "este...", "o sea...", "eh...", "básicamente...".

---

## GUION

---

### [APERTURA — cámara de cuerpo entero]

*[De pie, viendo a cámara, formal]*

Hola, mi nombre es Fernando Alfaro Montalvo, matrícula 221204, estudiante de la materia de Programación Avanzada. En este video voy a presentar los conceptos principales de los **Sistemas Expertos**, una de las ramas más importantes de la Inteligencia Artificial.

Vamos a ver: qué es el conocimiento, qué es una base de conocimiento, cómo funciona el motor de inferencia, la línea de tiempo de los sistemas expertos y sus principales tipos.

*[Transición a pantalla con presentación]*

---

### [DIAPOSITIVA 1 — Título]

Los Sistemas Expertos son programas de computadora que simulan el razonamiento de un experto humano en un área específica. Fueron una de las primeras aplicaciones exitosas de la inteligencia artificial y siguen siendo relevantes hoy en día en áreas como medicina, finanzas, derecho y control industrial.

---

### [DIAPOSITIVA 2 — El Conocimiento]

Para entender los sistemas expertos, primero hay que entender qué es el **conocimiento**.

Desde el punto de vista de la inteligencia artificial, el conocimiento es la combinación de datos, reglas, conceptos y experiencias que permiten tomar decisiones inteligentes.

Existen tres tipos:

El **conocimiento declarativo**, que son los hechos y datos que sabemos sobre el mundo. Por ejemplo: "la fiebre es mayor a 38 grados".

El **conocimiento procedural**, que son los procedimientos o pasos que seguimos para resolver un problema. Por ejemplo: "si hay fiebre y dolor de garganta, recetar antibiótico".

Y el **metaconocimiento**, que es el conocimiento sobre el propio conocimiento; es decir, saber qué sabemos y cómo usarlo. Este tipo está relacionado con el motor de inferencia.

---

### [DIAPOSITIVA 3 — Base de Conocimiento]

La **base de conocimiento** es el componente central de un sistema experto. Es donde se almacena toda la información del dominio: los hechos y las reglas.

Los **hechos** son dinámicos: describen el estado actual de una situación. Por ejemplo, la temperatura de un paciente o el saldo de una cuenta bancaria. Estos se guardan en la *memoria de trabajo*.

Las **reglas** son estáticas: son afirmaciones de la forma *si... entonces...* que no cambian entre aplicaciones. Se almacenan en la base de conocimiento.

Un ejemplo de regla sería: *"Si la temperatura es mayor a 38 grados Y el paciente tiene dolor de cabeza, ENTONCES existe probabilidad de infección"*.

La calidad del sistema depende directamente de la calidad del conocimiento almacenado.

---

### [DIAPOSITIVA 4 — Motor de Inferencia]

El **motor de inferencia** es el "cerebro" del sistema experto. Es el componente que aplica las reglas de la base de conocimiento sobre los hechos disponibles para llegar a conclusiones.

Opera de dos formas principales:

El **encadenamiento hacia adelante** o *forward chaining*: parte de los hechos disponibles y aplica reglas para generar nuevas conclusiones. Se usa cuando queremos saber qué conclusiones podemos obtener de lo que ya sabemos.

El **encadenamiento hacia atrás** o *backward chaining*: parte de una hipótesis y trabaja hacia atrás buscando hechos que la soporten. Se usa cuando queremos verificar si una conclusión específica es válida.

Además del motor de inferencia, los sistemas expertos tienen un **subsistema de explicación** que permite al usuario entender por qué el sistema llegó a una conclusión determinada. Esto es fundamental para la confianza en el sistema.

---

### [DIAPOSITIVA 5 — Línea de Tiempo]

Los sistemas expertos tienen una historia de más de 60 años.

En **1956**, John McCarthy acuña el término "Inteligencia Artificial" en la Conferencia de Dartmouth. Ese mismo año Newell, Shaw y Simon crean el *Logic Theorist*, el primer programa de IA.

En **1965**, Edward Feigenbaum y Joshua Lederberg desarrollan **DENDRAL** en Stanford, el primer sistema experto real, capaz de identificar estructuras moleculares. Esto marcó el inicio de la era de los sistemas expertos.

En **1972**, se desarrolla **MYCIN**, un sistema experto para diagnóstico de enfermedades infecciosas. Fue un hito porque demostró que los SE podían rivalizar con médicos especialistas.

En los años **80**, los sistemas expertos alcanzaron su apogeo comercial. Empresas como Digital Equipment Corporation implementaron XCON, que ahorraba millones de dólares al año. Se habla del "invierno de la IA" como la etapa posterior, cuando las expectativas superaron las capacidades reales.

En los años **90 y 2000**, los SE se integran con bases de datos, Internet y sistemas de aprendizaje automático.

Hoy, en los **2020s**, los sistemas expertos evolucionaron hacia sistemas híbridos que combinan reglas con redes neuronales y aprendizaje profundo.

---

### [DIAPOSITIVA 6 — Tipos de Sistemas Expertos]

Existen varios tipos de sistemas expertos según su arquitectura y forma de razonamiento:

Los **sistemas basados en reglas** son los más sencillos. Usan reglas *si-entonces* para representar el conocimiento. Son deterministas y fáciles de implementar. Ejemplo: sistemas de diagnóstico médico básico.

Los **sistemas basados en casos** o *Case-Based Reasoning* (CBR): resuelven problemas nuevos buscando casos similares en una base de casos anteriores y adaptando la solución. Ejemplo: sistemas legales que buscan jurisprudencia.

Los **sistemas basados en marcos** (*frames*): organizan el conocimiento en estructuras llamadas marcos, similares a las clases en programación orientada a objetos. Son útiles para modelar jerarquías y herencia de propiedades.

Los **sistemas expertos difusos** o *fuzzy*: trabajan con lógica difusa para manejar incertidumbre. En lugar de verdadero/falso, usan valores graduales entre 0 y 1. Muy útiles en control industrial.

Los **sistemas híbridos**: combinan reglas con redes neuronales, algoritmos genéticos o aprendizaje automático. Son los más modernos y potentes.

---

### [CIERRE — cámara de cuerpo entero]

*[De pie, viendo a cámara]*

Para concluir, los Sistemas Expertos representan uno de los logros más significativos de la inteligencia artificial. Nos permiten capturar y automatizar el conocimiento de expertos humanos, hacerlo accesible a personas con menos experiencia y resolver problemas complejos de forma rápida y consistente.

Sus componentes principales —la base de conocimiento y el motor de inferencia— trabajan juntos para simular el razonamiento humano. Y aunque hoy los sistemas de aprendizaje profundo son más populares, los sistemas expertos siguen siendo fundamentales en áreas donde la transparencia y la explicabilidad son esenciales.

Gracias por su atención. Soy Fernando Alfaro Montalvo, matrícula 221204.

---

*[FIN DEL VIDEO]*
