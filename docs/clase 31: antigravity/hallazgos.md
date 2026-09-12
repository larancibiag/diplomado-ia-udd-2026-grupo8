# Principales Hallazgos de Diseño: Proyecto Spinstack
**Dossier Humano–IA · Customer Experience y AI Experience Design**  
*Universidad del Desarrollo · Facultad de Diseño · Educación Continua*  
**Autor:** Luis Ángel Arancibia Galleguillos  
**Sistema:** Spinstack (Asistente inteligente para colección, recomendación y analítica de vinilos)

---

## 1. Tensión Central: Optimización Algorítmica vs. Ritual Análogo
- **La trampa del streaming:** Los modelos genéricos de IA tienden a tratar la música como una plataforma de streaming tradicional (ej. Spotify), priorizando la retención y la alta rotación.
- **El bucle de popularidad (*Popularity Bias*):** El algoritmo sobrepondera los discos más escuchados recientemente, generando una cámara de eco que contradice el deseo primordial del coleccionista: rescatar la diversidad de su estantería física y desempolvar álbumes olvidados.
- **El valor del ritual:** En la escucha en vinilo, la fricción y el acto físico (seleccionar la edición, poner el disco en el tocadiscos, leer la portada) forman parte intrínseca del disfrute. Automatizar excesivamente esta experiencia degrada su valor afectivo.

---

## 2. Auditoría de Sesgos y Decisiones Críticas
El análisis de las 3 decisiones algorítmicas clave identificó sesgos cruzados entre el sistema y el usuario:

| Decisión Crítica | Sesgo Cognitivo (Usuario) | Sesgo Algorítmico (Sistema) | Riesgo Identificado | Solución de Diseño (Fricción Constructiva) |
| :--- | :--- | :--- | :--- | :--- |
| **1. Sugerencia de vinilo en el feed** | *Automation Bias / Anchoring*: Asume que la tarjeta destacada es la opción "óptima". | *Sesgo de optimización*: Recomienda títulos seguros de alta rotación previa. | Cámara de eco y subutilización de la colección física. | **Pausa explicativa** del criterio ("Sugerido por tarde lluviosa") + opción activa de **agitar para descubrir un disco olvidado**. |
| **2. Generación de recomendaciones y reportes** | *Automation Bias*: Acepta que las métricas reflejan la totalidad de sus hábitos. | *Bucle de retroalimentación*: Analiza solo reproducciones registradas recientemente. | Estancamiento en la diversidad del consumo y olvido de discos de baja rotación. | Módulo de verificación de hábitos + control explícito **"Romper el bucle"**. |
| **3. Asignación de perfil de coleccionista** | *Confirmation Bias / Overconfidence*: Valida la etiqueta como un juicio absoluto sobre su legitimidad. | *Proxy Bias*: Usa el valor comercial o volumen de la colección como proxy de calidad. | Daño de estatus, estigmatización y compras forzadas para "subir de nivel". | **Desglose transparente** de cálculo + opción de **personalizar rasgos o desactivar la etiqueta pública**. |

---

## 3. Estrategia UX: Fricción Constructiva vs. "Invisibilidad"
- **El mito de la invisibilidad:** Diseñar una IA completamente invisible no genera mayor fluidez, sino desconfianza y opacidad ("caja negra") cuando una recomendación no hace sentido.
- **Fricción constructiva:** Introducir pausas intencionales, explicaciones contextuales y controles manuales que devuelven la soberanía y la agencia al usuario:
  - **Pausas explicativas:** Mostrar siempre la razón contextual de una sugerencia.
  - **Gestos análogos:** Traducir controles digitales a gestos táctiles (ej. agitar el teléfono para explorar "The B-Side" o vinilos olvidados).
  - **Coproducción narrativa (*AI Liner Notes*):** La IA redacta borradores historiográficos, pero el usuario siempre puede editarlos y contrastarlos con metadatos oficiales de Discogs antes de guardarlos.

---

## 4. Brecha de Señales (*Signal Map*)
Existe un desfase crítico entre lo observable por la pantalla y la realidad del usuario:
- **Disco inactivo por 6+ meses:** El sistema tiende a inferir desinterés y ocultar el álbum; sin embargo, el usuario suele escucharlo físicamente sin registrar la sesión en la app.
- **Rechazos rápidos (swipes sucesivos):** No representan un fallo general del algoritmo, sino una búsqueda puntual de energía o *mood*. Se resuelve con selectores manuales rápidos en lugar de sobreajustes agresivos del perfil.
- **Escucha concentrada en un horario:** El sistema no debe encasillar al usuario en un único género para esa franja horaria.

---

## 5. Matriz Humano–IA y Soberanía del Usuario
La relación con la tecnología se define bajo un modelo de copiloto analítico:

- **Lo que hace la IA:**
  - Estructura metadatos complejos (integración Discogs).
  - Sugiere vinilos para evitar la parálisis de decisión.
  - Genera borradores narrativos y resúmenes cualitativos.
  - Ofrece rutas divergentes fuera de la rutina.
- **Lo que NUNCA hace la IA:**
  - Nunca reproduce música de forma automática ni reemplaza el acto físico.
  - Nunca publica ni comparte datos sin aprobación explícita.
  - Nunca asume emociones sin permitir validación rápida.
  - Nunca envía datos a la nube: **procesamiento 100% On-Device**.

---

## 6. Supuestos del Proyecto Revisados y Cuestionados
1. **"A mayor automatización, mejor experiencia de usuario":**  
   *Revisión:* En experiencias analógicas y afectivas, la automatización total destruye el ritual. La fricción constructiva restituye la agencia humana.
2. **"La IA debe ser invisible para sentirse fluida":**  
   *Revisión:* La invisibilidad produce desconfianza. La verdadera fluidez se logra con explicabilidad y transparencia.
3. **"El usuario siempre sabe lo que quiere o acepta ciegamente la IA":**  
   *Revisión:* El usuario oscila entre la parálisis de decisión y el sesgo de automatización. El sistema debe ofrecer un descubrimiento guiado y reconfigurable.
