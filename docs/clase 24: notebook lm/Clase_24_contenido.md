# Clase 24 — NotebookLM como asistente de research

**Diplomado IA Aplicada al Diseño · UDD · 2026**
Profesor: Darío Osorio
Fecha: Jueves 20 de agosto de 2026 · 18:30–21:00 hrs
Modalidad: **online sincrónico** · Unidad 3 · Sesión 3 de 10 · **Propuesta D**

---

## Apertura

Última clase con toque Colab. A partir de la próxima nos movemos 100% a herramientas SaaS. Y la primera es **NotebookLM** — la aplicación de Google que te deja "conversar" con tus propios documentos.

Para un diseñador que trabaja con research (papers, entrevistas, briefs), NotebookLM es probablemente la herramienta de IA más útil del ecosistema actual. No inventa: razona sobre lo que le das. Si sabes cargar bien tus fuentes, es como tener un asistente que se leyó todo.

## Resultado de aprendizaje de la sesión

Al finalizar la clase el estudiante podrá:

1. **Explicar** qué es RAG (Retrieval-Augmented Generation) en palabras simples.
2. **Cargar sus propias fuentes** en NotebookLM y consultarlas con preguntas útiles.
3. **Generar audios, mapas mentales y guías de estudio** a partir de sus documentos.
4. **Distinguir** cuándo NotebookLM es la herramienta adecuada y cuándo no.

## Glosario clave

| Término | Definición operativa |
|---------|----------------------|
| **NotebookLM** | App de Google donde cargas documentos y el modelo responde preguntas basándose sólo en ellos. |
| **RAG** | *Retrieval-Augmented Generation*: patrón donde el modelo recupera fragmentos de una base y responde con ellos. Reduce alucinaciones. |
| **Fuente / Source** | Documento cargado en NotebookLM (PDF, texto, YouTube, web). |
| **Cita** | Referencia numerada que NotebookLM agrega automáticamente para respaldar cada afirmación. |
| **Audio Overview** | Función que genera un "podcast" de dos voces resumiendo tus fuentes. |
| **Mind Map** | Función que genera un mapa mental visual del contenido cargado. |

---

## Parte 1 — Materia (30 min)

### Bloque 1 (10 min): El problema que resuelve RAG

Los LLMs "alucinan": cuando no saben algo, lo inventan con seguridad. Para un proyecto serio de diseño, esto es inaceptable.

**RAG** resuelve esto así: en lugar de que el modelo responda desde su memoria general, le damos los documentos relevantes en cada consulta. El modelo razona **solo sobre lo que le pasaste**. Si la respuesta no está en tus documentos, dice "no tengo esa información" (idealmente).

```
Tu pregunta
    ↓
[Sistema busca fragmentos relevantes en tus documentos]
    ↓
[LLM responde usando SOLO esos fragmentos]
    ↓
Respuesta con cita
```

NotebookLM es un RAG pulido y cerrado. Bajo el capó usa Gemini + un sistema de recuperación. Tú solo ves la interfaz de chat.

### Bloque 2 (10 min): Casos donde brilla

Para diseño, los usos más útiles son:

- **Investigación bibliográfica**: cargas 10 papers y pides síntesis comparada, contradicciones, lagunas.
- **Análisis de entrevistas**: cargas las transcripciones de la Unidad 2, pides patrones, quotes destacables, oportunidades de diseño.
- **Documentación de cliente**: subes todos los briefs, contratos y presentaciones y consultas requisitos implícitos.
- **Curación de contenido**: cargas 20 posts de blog o videos de YouTube y armas un mapa temático.

**Lo que NO hace bien**:
- Generar contenido nuevo desde cero (para eso: ChatGPT, Claude).
- Manejar imágenes con detalle fino.
- Actualizarse con información en tiempo real.

### Bloque 3 (10 min): Limitaciones y consideraciones

- **Privacidad**: tus documentos viajan a servidores de Google. Cuidado con datos confidenciales del cliente sin permiso.
- **Volumen**: NotebookLM Plus permite hasta 300 fuentes; el gratuito, 50. Suficiente para casi todo proyecto de diseño.
- **Idioma**: funciona bien en español. Mejor si las fuentes son consistentes en un solo idioma.
- **Sesgos**: los sesgos ya conocidos de Gemini se filtran en las síntesis. Verificar hallazgos importantes.

---

## Parte 2 — Ejercicios prácticos (90 min)

**Herramienta principal**: [notebooklm.google.com](https://notebooklm.google.com) (gratis, cuenta Google).

### Ejercicio 1 — Setup y primer notebook (15 min)

1. Ir a [notebooklm.google.com](https://notebooklm.google.com) e iniciar sesión.
2. Click en `+ Create new notebook`.
3. Nombrarlo con tu proyecto: `Proyecto_TuNombre_Diplomado`.
4. Recorrido por la interfaz: panel de fuentes (izquierda), chat (centro), estudio (derecha).

### Ejercicio 2 — Cargar fuentes reales del proyecto (25 min)

Cargar entre 3 y 8 fuentes de tu proyecto:

1. **Transcripciones de entrevistas de Unidad 2** (formato .txt o Google Doc).
2. **Papers relevantes** (PDF).
3. **Documentación del cliente** si aplica.
4. **Videos de YouTube** (puede indexar transcripciones automáticamente).
5. **Sitios web** relevantes (URL directa).

*Recomendación*: no cargues 50 fuentes de golpe. Empieza con 5 bien elegidas y evalúa la calidad de las respuestas.

### Ejercicio 3 — Hacer 5 preguntas útiles a tus fuentes (25 min)

Después de cargar, prueba al menos estas 5 preguntas (adaptadas a tu proyecto):

1. `Cuales son los 3 principales puntos de frustracion mencionados por los usuarios?`
2. `Que dijeron los entrevistados sobre [tema clave de tu proyecto]?`
3. `Hay diferencias entre los usuarios jovenes y mayores?`
4. `Que oportunidades de diseno emergen de este material?`
5. `Que temas aparecen en las fuentes que yo no habia considerado?`

**Anota en la bitácora**: qué respuesta te sorprendió, cuál te pareció una alucinación posible, qué cita textual vale la pena rescatar.

### Ejercicio 4 — Generar audio overview + mapa mental (15 min)

1. En el panel de "Estudio" (derecha), click en `Audio Overview → Generate`.
2. Esperar ~2 minutos. Se genera un "podcast" de dos voces que sintetiza tus fuentes.
3. Escuchá al menos 3 minutos y evaluá: ¿le pega al tono de tu proyecto? ¿faltó algo importante?
4. En el mismo panel, click en `Mind Map → Generate`.
5. Descarga el mapa mental (imagen o interactivo).

### Ejercicio 5 — Guardar evidencia y compartir (10 min)

1. Compartir el notebook con un compañero (`Share` → agregar correo).
2. Descargar el mapa mental y guardarlo en `outputs/` de tu repositorio GitHub.
3. Copiar 3 quotes destacables extraídos con NotebookLM a tu bitácora.

---

## Parte 3 — Revisiones en salas (30 min)

**Formato**: salas breakout de 3-4 estudiantes.

### Consigna

Cada estudiante (5-7 min):

1. Comparte pantalla y muestra su notebook con las fuentes cargadas.
2. Hace UNA pregunta en vivo delante del grupo. El grupo evalúa: ¿la respuesta fue útil? ¿Vio algo que el compañero no vio?
3. Muestra el mapa mental generado.

### Cierre en plenario (5 min)

- ¿Cuál fue la pregunta más productiva que alguien hizo?
- ¿Alguien detectó una alucinación clara?
- ¿En qué momento pensaste "esto ya no me lo hace un ChatGPT normal"?

---

## Trabajo autónomo (entre clase 24 y 25, ~2.5 horas)

1. **Cargar más fuentes** al notebook si sumás material nuevo (30 min).
2. **Escribir un mini-reporte** (1 página, en Google Docs) con los 5 hallazgos más fuertes que NotebookLM te ayudó a encontrar. Cada uno con su cita textual (1 h).
3. **Subir el mini-reporte** al repositorio como `docs/hallazgos_notebooklm.md` (15 min).
4. **Escuchar el Audio Overview completo** de tus fuentes (~15 min) y anotar 2 cosas que la síntesis dejó afuera (30 min).

---

## Conexión con el entregable de posta

Al cerrar tienes:
- Notebook LM con las fuentes del proyecto cargadas.
- Mini-reporte de hallazgos con citas textuales.
- Audio Overview generado (evidencia opcional pero útil).
- Mapa mental de los temas del proyecto.

---

## Recursos útiles

- [NotebookLM — Guía oficial](https://support.google.com/notebooklm).
- [Video oficial de Google: Introducing NotebookLM Audio Overviews](https://blog.google/innovation-and-ai/products/notebooklm-audio-video-sources/).
- Casos de uso reales en [notebooklm.google](https://notebooklm.google).

---

## Referencias culturales y casos LATAM

- **NotebookLM en periodismo latinoamericano**: casos de uso en investigación colaborativa en México ([Animal Político](https://www.animalpolitico.com)), Argentina ([Chequeado](https://chequeado.com)) y Chile ([Ciper](https://www.ciperchile.cl)).
- **Consideración ética**: recordar que las fuentes viajan a Google. Para trabajos con datos sensibles del cliente, verificar términos y consentimiento.

---

## Pregunta abierta de cierre

> NotebookLM te devuelve síntesis con citas confiables — pero decide qué es "importante" por tú. ¿Qué cambia en tu proceso de investigación cuando alguien más (o algo) hace la primera curaduría? ¿En qué momento vale la pena leer todo por tú mismo aunque tengas la herramienta?
