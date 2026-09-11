# **Clase 22 — ¿Qué es un modelo de IA? · Primer contacto con Colab**

**Diplomado IA Aplicada al Diseño · UDD · 2026** Profesor: Darío Osorio Fecha: Jueves 13 de agosto de 2026 · 18:30–21:00 hrs Modalidad: **online sincrónico** Unidad 3 · Sesión 1 de 10 · **Propuesta D**

## **Apertura**

Es la primera clase de la Unidad 3 y la primera de todo el arco técnico del diplomado. La pregunta que abre el semestre es simple: **¿qué es exactamente un modelo de IA?** No la respuesta de laboratorio, la respuesta útil para diseñar con estas herramientas sin volverse ni evangelista ni escéptico.

En paralelo, damos el primer contacto con **Google Colab** — la plataforma donde vamos a ejecutar código las próximas tres clases. Después dejamos Colab y pasamos a herramientas SaaS. Pero antes, conviene ver una vez cómo se ve por dentro el motor de todo esto.

## **Resultado de aprendizaje de la sesión**

Al finalizar la clase el estudiante podrá:

1. **Explicar** con palabras propias qué es un modelo de IA y por qué “predice” es más preciso que “entiende”.

2. **Distinguir** modelos generativos (crean) de modelos analíticos (clasifican).

3. **Abrir un notebook en Google Colab** y ejecutar sus celdas.

4. **Identificar** qué familia de modelo va a usar en su proyecto de posta.

## **Glosario clave (5 términos)**

| Término | Definición operativa |
| :---- | :---- |
| **Modelo de IA** | Función matemática con muchísimos parámetros que aprendió a relacionar entradas con salidas mirando millones de ejemplos. |
| **Parámetro** | Número interno del modelo. GPT-4 tiene \~1.8 billones. |
| **Inferencia** | Cuando el modelo ya entrenado responde a un input nuevo. Cada vez que escribes un prompt, eso es inferencia. |
| **Modelo generativo** | Produce contenido nuevo: texto, imagen, audio, video. Ej: ChatGPT, DALL·E. |
| **Modelo analítico** | Clasifica o predice sobre lo existente. Ej: sistemas de recomendación, detección de spam. |

## **Parte 1 — Materia**&nbsp;

### **Bloque 1¿Qué es “modelo” en IA?**

Un modelo de IA es una función matemática muy compleja. Punto. Lo que la hace especial no es la fórmula (que existe hace décadas) sino dos cosas:

1. Tiene **millones o miles de millones de parámetros internos** que se ajustan automáticamente.

2. Esos parámetros se ajustaron mirando una **cantidad descomunal de ejemplos** durante el entrenamiento.

**Analogía honesta**: imagina que quieres enseñarle a alguien a reconocer si un tipo de letra es serif o sans-serif. No le explicas reglas tipográficas — le muestras miles de imágenes etiquetadas. Después de mucho mirar, esa persona desarrolla intuición. Eso, hecho con números a escala industrial, es un modelo.

**Punto crítico**: los modelos **predicen**, no entienden. Un LLM predice “¿cuál es el token más probable que siga?”. Un modelo de imagen predice “¿qué patrón de píxeles es coherente con este texto?”. No hay comprensión en el sentido humano — hay estimación estadística de altísima calidad. Esta distinción no es filosófica, es operativa: cambia cómo confías en el output.

### **Bloque 2 : Generativos vs. analíticos — la decisión de diseño**

Toda la IA que vas a usar en el curso cae en una de estas dos familias:

| Generativos | Analíticos |
| :---- | :---- |
| Producen contenido nuevo | Clasifican, predicen, extraen |
| Texto, imagen, audio, video | Etiquetas, probabilidades, categorías |
| GPT, Claude, DALL·E, Suno | BERT, YOLO, sistemas de recomendación |
| Costo alto por uso | Costo bajo por uso |
| Difícil de evaluar | Métricas claras (accuracy) |
| Uso en diseño: coideación, bocetos | Uso en diseño: análisis de feedback |

**Guía rápida**: ¿necesitas producir algo? → generativo. ¿Necesitas entender o categorizar? → analítico. ¿Ambas cosas? → pipeline con las dos.

### **Bloque 3 : Panorama del ecosistema (versión mínima)**

Los modelos que vamos a usar durante el módulo 3:

* **Cerrados (dependes de la empresa)**: GPT (OpenAI), Claude (Anthropic), Gemini (Google), Midjourney.

* **Abiertos (puedes descargarlos)**: Llama (Meta), Mistral, Stable Diffusion, DeepSeek, Hermes.

* **Multimodales** (procesan texto \+ imagen \+ audio \+ video): GPT-4o, Claude Opus 4, Gemini 2.5, Veo (Flow).

Los cerrados son más pulidos y fáciles. Los abiertos te dan control, privacidad y menor costo a escala. En el semestre vamos a tocar los dos mundos.

## **Parte 2 — Ejercicios prácticos**&nbsp;

**Herramienta principal**: [Google Colab](https://colab.research.google.com) · **Notebook**: Clase\_22\_notebook.ipynb

### **Ejercicio 1 — Abrir Colab por primera vez**&nbsp;

1. Ir a [colab.research.google.com](https://colab.research.google.com) e iniciar sesión con tu cuenta Google.

2. Descargar el notebook Clase\_22\_notebook.ipynb desde el repositorio del diplomado (link en el chat).

3. Subir el notebook a Colab: Archivo → Subir cuaderno.

4. **Recorrido guiado por la interfaz**: celdas de código, celdas de texto, cómo se ejecutan, botón de “Play”.

5. Ejecutar la primera celda (\!pip install ...). No importa que digas “no entiendo el código” — importa que funcione.

### **Ejercicio 2 — Ver embeddings en acción**&nbsp;

El notebook incluye un ejercicio pre-armado donde vas a:

1. Cargar un modelo pequeño de “embeddings” (que convierte palabras en coordenadas matemáticas).

2. Modificar UNA lista de palabras con términos relevantes a tu proyecto de diseño.

3. Ejecutar y **ver visualmente** cómo el modelo agrupa conceptos parecidos.

No hay que escribir código. Sólo hay que cambiar la lista de palabras y presionar Play. El objetivo es que **veas por ti mismo** que la IA representa el significado como geometría.

### **Ejercicio 3 — Comparar generativo vs. analítico en vivo**&nbsp;

En el mismo notebook:

1. Ejecutar la celda de **clasificación de sentimiento** (analítico). Meter 3 frases de tu proyecto y ver la respuesta.

2. Ejecutar la celda de **generación de texto** (generativo). Ver cómo responde a un prompt inicial.

3. Anotar las diferencias en tu bitácora: velocidad, tipo de respuesta, reproducibilidad.

### **Ejercicio 4 — Primer borrador de la ficha de tu proyecto**&nbsp;

En un documento nuevo ([Google Docs](https://docs.google.com) recomendado), completar:

* Nombre interno del proyecto.

* Problema heredado de la Unidad 2 (2-3 frases).

* Qué tipo de modelo crees que vas a necesitar (generativo / analítico / ambos).

* 2-3 modelos candidatos concretos (de los mencionados en la materia o los que descubriste en Colab).

**¿Y si no tienes problema heredado de la Unidad 2?** Inventa algo simple pero que aguante las 10 clases — necesita dar pie a un dataset (Clase 23), texto/LLM (Clase 25), imagen (Clase 27), video (Clase 29\) y un flujo agéntico (Clase 28-31). Opciones rápidas:

* **Un emprendimiento real cercano** (el café de la esquina, la marca de un amigo, un taller de cerámica) que necesita identidad visual \+ contenido para redes. Es la más fácil: da reseñas de clientes para el dataset, copy para redes, imágenes de producto, video promocional.

* **Un proyecto cultural o patrimonial local** — difundir un museo regional, un festival, un oficio artesanal en riesgo. Encaja con el marco crítico del curso (sesgos, representación, soberanía de datos).

* **Una causa o servicio social** — una app o campaña para adultos mayores, accesibilidad, o una ONG que conozcan. Bueno si quieren que el agente final (Clase 30-31) resuelva algo con peso real.

* **Algo autobiográfico** — su propio portafolio o práctica creativa como “cliente”. Menos ambicioso, pero más fácil de sostener motivacionalmente 10 clases.

No hace falta que sea el proyecto definitivo — con nombre, problema en 2-3 frases y un modelo candidato alcanza para hoy. Se puede ajustar o cambiar de tema hasta la Clase 25 sin gran costo.

Este documento va a crecer clase a clase. Es tu **model card** en versión de borrador.

## **Parte 3 — Revisiones en salas**&nbsp;

**Formato**: salas breakout de 3-4 estudiantes en Zoom/Teams.

### **Consigna para las salas**

Cada grupo:

1. Mostrar su lista de palabras del ejercicio de embeddings y contar qué le llamó la atención.

2. Compartir la ficha borrador de su proyecto.

3. Recibir del grupo **una pregunta y una sugerencia** — sin evaluar, sin corregir. Solo aportar mirada externa.

### **Cierre en plenario**&nbsp;

El grupo completo vuelve a la sala principal. El profesor pregunta:

* ¿Qué les sorprendió más de lo que vieron hoy?

* ¿Alguien encontró algo raro en los embeddings de su proyecto?

* ¿Qué duda quedó dando vueltas para llevarse a casa?

## **Trabajo autónomo (entre clase 22 y 23, \~2 horas)**

1. **Consolidar la ficha del proyecto** con lo discutido en la sala breakout (30 min).

2. **Ver el video de 3Blue1Brown** [*But what is a neural network?*](https://www.youtube.com/watch?v=aircAruvnKk) (YouTube, 20 min). No hace falta entender la matemática — sí construir intuición visual.

3. **Explorar el catálogo de modelos** en [huggingface.co/models](https://huggingface.co/models) sin instalar nada. Filtrar por tarea (text-generation, text-classification, image-generation) y anotar 3 que te llamen la atención (30 min).

4. **Crear tu cuenta en GitHub** si aún no la tienes ([github.com/signup](https://github.com/signup)). Guía completa en Clase\_22\_guia\_estudiante.md sección “GitHub para el diplomado” (30 min).

## **Conexión con el entregable**&nbsp;

## **Esta clase abre el borrador inicial del prototipo:**

* Ficha del proyecto con problema, familia de modelo y candidatos.

* Cuenta de GitHub activa (indispensable para todas las clases siguientes).

## **Recursos útiles**

**Videos accesibles (no obligatorios pero muy recomendados)**:

* 3Blue1Brown — [*But what is a neural network?*](https://www.youtube.com/watch?v=aircAruvnKk) (YouTube, \~20 min). El clásico para intuición visual.

* Andrej Karpathy — [*Intro to Large Language Models*](https://www.youtube.com/watch?v=zjkBMFhNj_g) (YouTube, \~1 hora). Denso pero maravilloso.

* [Two Minute Papers](https://www.youtube.com/@TwoMinutePapers) — canal completo. Ideal para mantenerse al día.

**Lecturas cortas complementarias**:

* Bommasani et al. (2021) [*On the Opportunities and Risks of Foundation Models*](https://arxiv.org/abs/2108.07258) — leer sólo secciones 1 y 2 (una tarde, sin apuro).

## **Referencias culturales y casos LATAM**

* [**CENIA Chile**](https://www.cenia.cl) — Centro Nacional de Inteligencia Artificial. Interesante conocer el ecosistema local.

* [**Latinx in AI**](https://www.latinxinai.org) — comunidad de investigadoras e investigadores latinoamericanos.

* **Karen Hao** — periodista, autora de [*Empire of AI*](https://www.penguinrandomhouse.com/books/743569/empire-of-ai-by-karen-hao/) (2025). Su trabajo cubre la dimensión laboral y geopolítica del sector.

## **Pregunta abierta de cierre**

Si un modelo “no entiende” en el sentido humano pero produce respuestas que son útiles, hermosas o certeras — ¿qué diferencia hay entre ese output y el trabajo de una persona? ¿Y qué te dice esa diferencia sobre el rol del diseñador en 2026?
