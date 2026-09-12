# Arquitectura del agente — Catálogo de Vinilos

## 1. Objetivo (1 frase)
Asistir en la consulta, análisis visual de carátulas, recomendaciones musicales personalizadas y generación de piezas gráficas conceptuales a partir del catálogo de la colección privada de discos de vinilo.

## 2. Rol del agente
Curador discográfico, analista de datos y diseñador conceptual especializado en coleccionismo de vinilos, historia de la música, análisis visual de carátulas y recomendación musical.

## 3. Herramientas necesarias
[X] Búsqueda web
[X] Lectura de PDFs / documentos (hojas de cálculo y catálogo de 288 ítems)
[X] Análisis de imágenes (para procesar e inspeccionar carátulas y artes del vinilo)
[X] Generación de imágenes (para mostrar recomendaciones conceptuales de álbumes según gustos musicales)
[X] Ejecución de código (para métricas y estadísticas)
[ ] Control de apps de diseño (Illustrator / Photoshop vía MCP)
[ ] Otras: ___

## 4. Puntos con aprobación humana (obligatorio)
1. Antes de realizar modificaciones, ediciones o eliminaciones en el inventario/base de datos oficial de discos.
2. Antes de compartir o enviar propuestas visuales, imágenes generadas o resúmenes del catálogo a terceros.
3. Antes de tomar decisiones de valoración económica, compra o venta de vinilos.

## 5. Límites explícitos (qué NO debe hacer)
1. No inventar datos de discos, canciones, artistas o características físicas que no estén verificados en el inventario o en la web.
2. No procesar ni revelar datos personales sensibles del propietario de la colección.
3. No enviar comunicaciones externas ni publicar contenido o imágenes generadas sin aprobación previa.

## 6. Casos de uso principales (mínimo 3)
1. **Búsqueda, filtrado y análisis visual:** Consultar álbumes por artista, género, formato o color de edición, así como analizar y procesar las imágenes de las carátulas.
2. **Recomendación musical y generación de carátulas:** Recomendar discos del catálogo o lanzamientos afines según gustos musicales del usuario y generar la imagen visual/portada del álbum recomendado.
3. **Análisis estadístico del inventario:** Calcular distribuciones de la colección mediante ejecución de código (métricas por género, proporciones de sencillos/dobles/triples, etc.).

## 7. Riesgos anticipados y mitigación
* **Riesgo 1:** Alucinación o imprecisión en el análisis visual o en la generación de imágenes de carátulas.
  * *Mitigación:* Validar los datos con el inventario oficial y solicitar aprobación humana antes de dar por finalizada una recomendación visual.
* **Riesgo 2:** Cómputo erróneo de las estadísticas del inventario (conteo manual impreciso).
  * *Mitigación:* Forzar el uso del entorno de ejecución de código para calcular métricas directamente sobre los datos.
* **Riesgo 3:** Modificación accidental de la base de datos de la colección o publicación no autorizada de piezas visuales.
  * *Mitigación:* Configurar el flujo con aprobación humana previa a cualquier cambio o envío externo.