# Resúmenes de PDFs — Sistemas Expertos
**Fernando Alfaro Montalvo | Matrícula 221204**

---

## 1. Resumen: Ingeniería de Conocimiento (Capítulo 2)
**Archivo:** `0-Ingenieria-del-conocimiento(complementaria).pdf`

### Conceptos fundamentales

**Conocimiento**
Desde el punto de vista de la IA, el conocimiento es la combinación de esquemas o estructuras de datos y procedimientos que confieren comportamiento inteligente. Está formado por hechos, conceptos, procedimientos, ideas, abstracciones, reglas y asociaciones usadas para modelar el mundo real. Existen tres tipos:

- **Conocimiento declarativo:** expresión de hechos o atributos poseídos por un objeto, persona o concepto.
- **Conocimiento procedural:** conjunto de reglas basadas en conocimiento que los expertos usan para resolver problemas.
- **Metaconocimiento:** conocimiento sobre el propio conocimiento y la experiencia; forma parte del Motor de Inferencia.

**Ingeniero del Conocimiento (ICO)**
Especialista informático con conocimientos profundos sobre el desarrollo de sistemas basados en conocimiento (Sistemas Expertos). Sus funciones son: extraer el conocimiento del experto humano y plasmarlo en una Base de Conocimiento, e implementar correctamente ese conocimiento.

**Ingeniería del Conocimiento (IC)**
Disciplina asociada a la IA que se ocupa de la adquisición, representación, validación, inferenciación, explicación y mantenimiento del conocimiento. Su objetivo es construir sistemas expertos mediante tres procesos fundamentales:

1. **Adquisición del Conocimiento:** extracción del conocimiento de las fuentes (estáticas: libros, artículos; dinámicas: el experto humano).
2. **Representación del Conocimiento (KR):** proceso de llevar el conocimiento extraído a una forma inteligible para el sistema. Los principales esquemas son: reglas de lógica simbólica, redes semánticas, gráficos conceptuales, árboles de decisión, frames/slots y diagramas lógicos.
3. **Base de Conocimiento:** almacén donde entra la información tal como llega; puede representarse mediante reglas de producción (si → entonces).

### Etapas de la Adquisición del Conocimiento
El proceso tiene 5 etapas:
1. **Identificación:** reconocimiento del problema y sus características.
2. **Entendimiento:** determinación de conceptos y relaciones relevantes.
3. **Formalización:** representación del conocimiento en la Base de Conocimiento.
4. **Implementación:** programación del conocimiento en la computadora; se desarrolla un prototipo.
5. **Pruebas:** validación del sistema mediante ejemplos reales evaluados con el experto humano.

### Representación del Conocimiento — Lógica
La lógica proposicional evalúa proposiciones como verdaderas (V) o falsas (F) usando operadores lógicos (∧, ∨, ¬, →, ≡). Los mecanismos de inferencia básicos son:
- **Modus Ponendo Ponens:** si P→Q y P, entonces Q.
- **Modus Tollendo Tollens:** si P→Q y ¬Q, entonces ¬P.

La lógica de predicados amplía la proposicional incluyendo predicados, variables, funciones y cuantificadores, permitiendo enunciados más expresivos.

---

## 2. Resumen: Sistemas Expertos Basados en Reglas
**Archivo:** `1-sistemasExpertosBasadosEnReglas(referencia).pdf`
**Autor:** Luis Valencia Cabrera — Universidad de Sevilla

### Introducción
Los sistemas basados en reglas son una herramienta eficiente para tratar situaciones complejas que se rigen por reglas deterministas (control de tráfico, seguridad, transacciones bancarias, etc.). Son la metodología más sencilla de los sistemas expertos y sirvieron como base para desarrollos más complejos.

### Componentes principales

**Base de Conocimiento**
Contiene dos elementos:
- **Hechos:** son dinámicos, conocidos en una situación particular y se almacenan en la *memoria de trabajo*. Pueden cambiar de una aplicación a otra.
- **Reglas:** son estáticas, no cambian entre aplicaciones (a menos que haya aprendizaje) y se almacenan en la *base de conocimiento*.

**Motor de Inferencia**
Aplica la lógica clásica a las reglas de la base de conocimiento para sacar conclusiones automáticamente.

### Estructura de una regla
Una regla es una afirmación lógica con dos partes:
- **Premisa (antecedente):** expresión lógica entre las palabras clave *Si* y *entonces*. Puede combinar afirmaciones con operadores `y`, `o`, `no`.
- **Conclusión (consecuente):** expresión lógica tras la palabra clave *entonces*.

Ejemplo:
```
Regla 1: Si nota > 9, entonces calificación = sobresaliente.
Regla 2: Si puesto < 20 o nota > 7, entonces Admitir = sí y Notificar = sí.
```

### Tipos de reglas
- **Regla simple:** contiene solo expresiones lógicas simples (una afirmación objeto-valor).
- **Regla compuesta:** contiene expresiones lógicas compuestas (múltiples afirmaciones conectadas).

### Ejemplo — Cajero Automático
Problema determinista modelado con reglas: un cliente solo recibe dinero si la tarjeta es verificada, la fecha no ha expirado, el NIP es correcto, no se excedió el número de intentos, y la cantidad solicitada no supera el saldo disponible ni el límite diario. Cada condición se codifica como una regla.

### Sustitución de reglas
Las reglas con el operador `o` en la premisa pueden dividirse en reglas simples equivalentes sin perder generalidad, facilitando la implementación en código:
```
Regla: Si A o B, entonces C
→ Regla 1a: Si A, entonces C
→ Regla 1b: Si B, entonces C
```

### Sistemas probabilísticos
Los sistemas basados en reglas deterministas son un caso particular de los sistemas probabilísticos. Cuando la certeza de las reglas no es absoluta, se extienden hacia modelos probabilísticos (redes bayesianas, etc.), que son una generalización de los sistemas basados en reglas.

### Limitaciones
- Solo funcionan bien en dominios bien definidos y con reglas claras.
- No manejan bien la incertidumbre sin extensiones probabilísticas.
- La base de conocimiento puede volverse difícil de mantener a gran escala.
- Dependen de la calidad del conocimiento extraído del experto humano.
