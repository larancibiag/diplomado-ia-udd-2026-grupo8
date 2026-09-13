# Diplomado IA UDD 2026

Diplomado de Inteligencia Artificial Aplicada al Diseño

Unidad 3: IA Afectiva, neurocognitiva y psicosocial de la tecnología aplicada al diseño de experiencia

Integrantes: GRUPO 8: Luis ARANCIBIA · Bianca GONZÁLEZ · Fanny HOFFENBERG

&nbsp;

---
## **1\. Proyecto**

X

&nbsp;

---
## **2\. Entregables**

#### CLASE 22: Google Colab

¿Qué hicimos?
En Google Colab calculamos la matriz de similitud entre diferentes conceptos mediante embeddings para medir qué tan relacionados están semánticamente.
  
Conclusión
Interesante conocer como las inteligencias artificiales entienden el lenguaje agrupando conceptos por cercanía de significado y no solo por coincidencia de palabras.

&nbsp;

---

#### CLASE 23: Data Sheet

¿Qué hicimos?

Ejercicio 1:
Cargamos un conjunto de datos de reseñas en Google Colab para analizar su estructura y contar cuántas filas existen por cada categoría.

Conclusión: Este análisis exploratorio inicial permite entender la distribución y el volumen de los datos antes de aplicar modelos de inteligencia artificial.

Ejercicio 2:
Analizamos los gráficos de distribución y longitud de textos para detectar anomalías y desvíos en el dataset de reseñas.
- Patrón raro: Las calificaciones extremas (1 y 5 estrellas) concentran la gran mayoría de los datos (más de 300 reseñas cada una), mientras que el punto medio (3 estrellas) presenta una caída muy marcada (solo 91 reseñas).
- Sesgo: Sesgo de polarización. Los usuarios rara vez se toman el tiempo de escribir una reseña cuando un producto simplemente cumple de manera estándar o mediocre; solo se motivan a dejar un registro cuando su experiencia es maravillosa o terriblemente decepcionante.

Conclusión: 
Identificar estos patrones de sesgo permite evitar que el modelo aprenda atajos erróneos, como usar la longitud del texto en lugar del contenido real para predecir las calificaciones.

Clase más representada: La de 5 estrellas, con más de 300 reviews en total.
Clase menos representada: La de 3 estrellas, con apenas unas 90 reviews.
Sí, las reseñas de 1 estrella son mucho más largas que el resto, lo que representa un sesgo en el que un modelo predictivo podría usar la longitud del texto como pista falsa en lugar de evaluar el contenido real.

Ejercicio 3 y 4:
Creamos el archivo datashhet con datos reales del proyecto. Archivo: datasheet\_v1.md
Subimos el notebook trabajado a notebooks/Clase\_23.ipynb. Actualizar README.

&nbsp;

---

#### CLASE 24: Notebook LM

¿Qué hicimos?

Hicimos preguntas útiles, preguntas específicas y otras genéricas
— Elaborar un resumen de la colección
- ¿Qué artistas tienen la mayor cantidad de álbumes en esta lista?
- ¿Qué álbumes tengo de rock argentino?
- ¿Qué álbumes tengo de la década de los 90?
- ¿Cuáles son mis vinilos dobles?

Conclusiones

La experiencia con NotebookLM permitió comprobar que su principal aporte no está solamente en generar resúmenes, sino en transformar una fuente de información en una base de conocimiento que puede ser consultada y analizada mediante preguntas. A partir de una misma colección fue posible obtener información sobre artistas, formatos, décadas, géneros y características específicas, demostrando su capacidad para organizar grandes volúmenes de información y facilitar la detección de patrones.
Uno de los principales aprendizajes fue comprender que la calidad y utilidad de los resultados dependen en gran medida de la capacidad del usuario para formular buenas preguntas. Por lo tanto, el uso de IA requiere desarrollar nuevas habilidades de análisis y de interacción con la herramienta, más que simplemente aprender a utilizar una nueva aplicación.

También fue importante comprobar que NotebookLM tiene límites: cuando la información no estaba contenida en las fuentes originales, la herramienta fue capaz de identificar esa carencia y proponer complementar la investigación. Esto demuestra que la IA no reemplaza la investigación ni el criterio humano, sino que puede integrarse como una herramienta de apoyo que amplía nuestras capacidades.

Desde la perspectiva del diseño, considero que NotebookLM puede ser especialmente útil en etapas de investigación, análisis y organización de información. Puede permitir que el diseñador dedique menos tiempo a tareas mecánicas de búsqueda y clasificación y más tiempo a interpretar la información, generar conceptos y tomar decisiones estratégicas.

En definitiva, la experiencia demuestra que el verdadero valor de la IA no está necesariamente en que haga el trabajo por nosotros, sino en que puede ayudarnos a trabajar de una manera diferente: más rápida, informada y estratégica, manteniendo al diseñador como responsable del criterio, la interpretación y la decisión final.


&nbsp;

---

#### CLASE 25: GPT, Claude & DeepSeek

¿Qué hicimos?
Comparativa de mopdelos:  Claude, Chat GPT y DeepSeek para analizar la performance de cada uno de estas herramientas de inteligencia artificial y como abordan un mismo problema de diseño de maneras muy diferentes. 
  
Conclusiones 
La comparación entre Claude, ChatGPT y DeepSeek permitió comprobar que las herramientas de inteligencia artificial pueden abordar un mismo problema de diseño de maneras muy diferentes. Más que identificar cuál aplicación es “mejor”, la experiencia permitió reconocer que cada modelo tiene fortalezas, limitaciones y formas particulares de interpretar un mismo brief.

Uno de los principales aprendizajes fue comprobar que la calidad del resultado depende en gran medida de la información entregada, de las restricciones establecidas y, especialmente, de la capacidad de formular correctamente las instrucciones. Un buen prompt permite orientar a la IA hacia resultados más pertinentes y cercanos a las necesidades reales del proyecto.

En el desarrollo del estante, por ejemplo, DeepSeek fue capaz de analizar la cantidad de vinilos, realizar estimaciones dimensionales y proponer una distribución por géneros, además de incorporar criterios de accesibilidad y crecimiento futuro. Esto demuestra el potencial de estas herramientas para apoyar no solo la generación de ideas, sino también etapas de análisis y planificación.

Sin embargo, la experiencia también permitió comprobar que una respuesta extensa y aparentemente técnica no necesariamente constituye una solución de diseño correcta. Algunas propuestas deben ser revisadas, ajustadas y evaluadas desde criterios que la IA no necesariamente puede comprender completamente, como la experiencia del usuario, la proporción, la estética, la funcionalidad, la factibilidad constructiva o la coherencia con el contexto.

En el caso del sticker ocurre algo similar: la IA puede desarrollar un concepto, definir una composición, sugerir tipografías, colores e iconografía e incluso generar instrucciones para producirlo. Sin embargo, el diseñador sigue siendo necesario para evaluar si esa propuesta realmente funciona como pieza gráfica y si cumple adecuadamente con criterios de legibilidad, jerarquía, identidad y reproducción.

Por lo tanto, considero que el principal aporte de estas herramientas al diseño no es reemplazar al diseñador, sino modificar su manera de trabajar. La IA puede asumir parte del trabajo exploratorio, analítico y repetitivo, permitiendo que el profesional concentre mayor atención en la interpretación, el criterio, la conceptualización y la toma de decisiones.

La experiencia confirma que el valor del diseñador no desaparece frente a la IA; se desplaza desde la ejecución hacia la capacidad de plantear problemas, dirigir herramientas, evaluar resultados y tomar decisiones de diseño con criterio profesional.

En este sentido, aprender a trabajar con distintas herramientas de IA se convierte en una nueva competencia profesional. El diseñador que sepa utilizarlas críticamente podrá incorporarlas como una extensión de sus propias capacidades, obteniendo procesos más rápidos y exploratorios, sin perder aquello que sigue siendo esencial: el criterio humano.


&nbsp;

---

#### CLASE 26: Hugging Face

¿Qué hicimos?
Explorar hugging face para probar e integrar modelos avanzados de IA generativa de imagen y prototipado visual sin depender exclusivamente de plataformas cerradas de suscripción.

meta-llama/Llama-3.2-1B-Instruct: El estándar más moderno para prototipar respuestas rápidas y fluidas en aplicaciones móviles.
DeepESP/gpt2-spanish: Un clásico ligero, ideal para correr experimentos web ultrarrápidos sin hardware dedicado.
somosnlp/es-inclusivo-translator

  
Conclusiones

Principales ventajas identificadas:

1. Acceso a modelos de código y pesos abiertos (Open Weights): Permite utilizar y comparar modelos de última generación para generación visual y fotorrealismo (como la familia FLUX.1, Krea 2 Turbo y Z Image Turbo).

2. Prototipado rápido sin código (Hugging Face Spaces): Brinda aplicaciones web interactivas listas para usar que permiten a los creativos probar herramientas de texto a imagen, remoción de fondos, edición local e inpainting directamente en el navegador.

3. Personalización y control de estilos (LoRAs y ControlNet): Facilita el acceso a miles de adaptadores visuales creados por la comunidad para aplicar estilos gráficos específicos (editorial, 3D, branding) o guiar la generación a partir de bocetos y wireframes.

4. Independencia, privacidad y licencias claras: Proporciona mayor control sobre las imágenes generadas y la posibilidad de integrar los modelos en pipelines profesionales o plugins locales (como ComfyUI o Figma).

&nbsp;

---

#### CLASE 27: Gemini Nano Banana

¿Qué hicimos?
Experimentar con Nano Banana.
  
Conclusiones

La experiencia con Nano Banana confirma que la inteligencia artificial no sustituye a la dirección de arte, sino que amplifica su alcance. Aunque la plataforma ofrece un control de nivel estudio con ediciones localizadas, iluminación, profundidad de campo e integración de hasta más de 10 fuentes visuales, es la visión del creador la que otorga sentido a la pieza.

La precisión en el prompt, la sensibilidad estética y el criterio para curar, seleccionar y armonizar los elementos de la escena siguen siendo aportes insustituibles de la mente humana.

&nbsp;

---

#### CLASE 28: Agentes

####  ¿Qué hicimos?
 
Configuramos y desplegamos un agente conversacional en Claude Projects utilizando una arquitectura provista en el curso. Para lograrlo:

Definición del Agente: Cargamos el system prompt con las instrucciones de la arquitectura del asistente especializado en vinilos.

Contexto e Inventario: Proporcionamos conocimiento contextual subiendo la base de datos de la colección de vinilos y un dossier de soporte en IA.

Ejecución del Flujo: Validamos la capacidad del agente para procesar un escenario específico (tarde soleada de sábado/diseñadora trabajando) ejecutando un flujo multitarea que incluyó: recomendación personalizada, notas contextuales editoriales, verificación exacta de datos en inventario, generación e integración de prompts e ilustraciones visuales, sugerencias por similitud sonora y la maquetación final estructurada de una "ficha de track" en PDF.
  
####  Conclusiones

Al integrar nuestra propia base de datos cdentro de la base de conocimiento en claude, logramos que el asistente pueda consultar el inventario, verificando conteos por artista y género sin alucinar datos. Además, el agente demostró una gran versatilidad para adaptarse al contexto y tono solicitados (diseñadora, tarde soleada de sábado), conectando la recomendación musical con la redacción editorial y la generación de ideas visuales. Lo más destacado fue su capacidad para orquestar en un solo flujo la lectura de datos duros, la creación de contenido sintético y el diseño gráfico, estructurando todo de manera coherente en un entregable final listo para usar como la ficha de track en PDF.

&nbsp;

---

#### CLASE 31: ANTIGRAVITY

#### > ¿Qué hicimos?

Creamos una carpeta nueva con un archivo `hallazgos.md` 
Abrimos la carpeta en Antigravity y le pedimos un HTML simple, minimalista y responsive con esos hallazgos.

    " Necesito una página HTML simple que muestre los principales hallazgos de mi proyecto de diseño. Los datos están en `hallazgos.md`. Genera un HTML con estilo minimalista, responsive, en español."

Abrimos el HTML resultante y revisarlo. (capturas)
Pedimos un segundo cambio de estilo (colores, tipografía)(capturas)

#### Conclusiones



&nbsp;

---
## **3\. Conclusiones**

#### Conclusiones de grupo

A lo largo de esta unidad pudimos observar que la inteligencia artificial no es solamente una herramienta para generar contenido, sino una nueva capa que puede incorporarse transversalmente al proceso de diseño: desde la exploración y análisis de datos, la investigación y generación de insights, hasta la conceptualización, prototipado, evaluación y comunicación de soluciones.

Uno de los principales aprendizajes como grupo fue comprender que el valor de la IA no está únicamente en lo que puede producir, sino en cómo el diseñador es capaz de dirigirla. La calidad de los resultados depende de la información disponible, de las preguntas que formulamos, de las restricciones que definimos y de nuestra capacidad para evaluar críticamente lo que la herramienta entrega. Aprender a diseñar con IA implica también aprender a diseñar las instrucciones, los contextos y los criterios con los que interactuamos con ella.
Desde nuestra experiencia como diseñadores vinculados a un laboratorio de innovación, esto adquiere especial relevancia. En contextos donde trabajamos con problemas ambiguos, múltiples actores, información incompleta y necesidad de experimentar rápidamente, la IA puede convertirse en un acelerador de ciclos de exploración y aprendizaje. Permite analizar grandes volúmenes de información, encontrar relaciones que podrían pasar inadvertidas, generar múltiples alternativas, prototipar soluciones y testear diferentes caminos en mucho menos tiempo.

Sin embargo, también identificamos un límite importante: la velocidad de generación no equivale necesariamente a calidad de diseño. Una IA puede producir una respuesta técnicamente correcta, visualmente atractiva o muy elaborada, pero eso no garantiza que resuelva el problema correcto ni que sea pertinente para las personas, el negocio o el contexto. El diseñador sigue siendo responsable de interpretar, cuestionar, priorizar y decidir.

Estos ejercicios también nos mostraron que trabajar con IA exige entender los datos que la alimentan, reconocer sesgos y cuestionar los resultados, ya que un modelo puede amplificar patrones existentes y convertir un sesgo en una decisión aparentemente objetiva.
Además, notamos una transformación en el rol del diseñador: ya no se trata solo de ejecutar cada parte de una solución, sino de orquestar sistemas que combinan información, generación de contenido y producción. 

El diseñador pasa de ser ejecutor a director del proceso, y el criterio humano qué problema resolver, qué preguntas hacer, qué alternativas descartar cobra aún más peso.

Quizá no necesitamos ser programadores, pero sí entender lo básico sobre datos, sesgos, límites y privacidad de estas herramientas.
Esta unidad nos permitió ver a la IA no como un reemplazo del diseñador ni solo como una herramienta de productividad, sino una invitación a cambiar de mindser de como deberiamos a usar la IA de  forma crítica y estratégica para explorar y aprender y ejecutar  más rápido, sin delegar en ella nuestra vision integral y humana , el buen gusto, el criterio, la empatía y la creatividad que definen nuestro aporte como  profesionales del diseño.
