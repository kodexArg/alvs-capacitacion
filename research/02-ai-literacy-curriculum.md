# AI Literacy para oficinistas principiantes (Haiku brief)

> Currículo base para el workshop de 4h.

## 1. Conceptos core (sin jerga)

Tres ideas fundacionales:

- **LLM vs "AI"**: "Esto no es inteligencia consciente — es un motor de predicción de texto muy bueno, entrenado con miles de millones de documentos. Aprendió patrones de cómo se combinan las palabras, no a razonar."
- **Tokens como bloques de texto**: "Cada mensaje usa unidades llamadas tokens (~4 caracteres c/u). Conversaciones largas consumen más tokens; documentos muy largos pueden superar lo que el modelo puede 'leer' de una sola vez."
- **Context window / alucinaciones**: "El modelo ve una ventana limitada de la conversación — como un pizarrón con espacio finito. Y a veces inventa datos con mucha confianza cuando no sabe: rellena los huecos en lugar de admitir que no sabe."
- **Training cutoff**: "El conocimiento se congeló en una fecha. No sabe qué pasó después, y no puede verificar afirmaciones en tiempo real."

**Evitar**: "redes neuronales", "transformers", "inferencia estadística".

## 2. Modelo mental: "Autocomplete con esteroides" + "becario que leyó internet"

**Metáfora principal**: "Como el autocomplete de tu teléfono, pero entrenado con millones de libros, artículos y sitios. Predice la próxima palabra extremadamente bien, pero no *entiende* — solo sabe qué suele venir después."

**Metáfora secundaria** (para matizar): "Pensalo como un becario con formación en Harvard que recuerda detalles de casi todo, pero a veces se equivoca y suena confiado mientras miente."

**Evitar**: "es como un segundo cerebro" (implica consciencia), "piensa", "sabe" — se vuelven en contra después.

## 3. Framework de prompting: RACE (minimalista)

**RACE gana sobre CO-STAR y otros para principiantes**. CO-STAR es completo pero tiene 6 componentes (demasiada carga cognitiva). RACE tiene 4:

- **Role**: "Actuá como..."
- **Action**: "Tu tarea es..."
- **Constraints**: "Usá solo formato X. No menciones Y."
- **Example**: "Acá hay un ejemplo de buena salida..."

Funciona para el 80% de tareas de oficina. Estructura = consistencia. Un principiante que aprende RACE escribe mejores prompts en 20 segundos y ve mejora inmediata.

> Nota del diseñador: el usuario mencionó originalmente "Contexto → Consulta → Resultado". Es compatible con RACE; se puede presentar con esos nombres en español.

## 4. Enseñar system prompts concretamente

**Opción A — Claude Projects**: mejor UX para no técnicos. Instrucciones persisten entre conversaciones. Free tier disponible. Demo inmediata: "redactar un email interno" en Claude base, después lo mismo en un Project con custom instructions → diferencia dramática visible al instante.

**Opción B — ChatGPT Custom Instructions**: funciona, pero el UI está enterrado y cuesta encontrarlo.

**Gemini Gems**: pagos, descartar.

## 5. Anti-patterns a pre-avisar

- **Tratarlo como Google**: "mejores restaurantes NYC" → consejos alucinados. **Enseñar**: Google para hechos, AI para brainstorm/draft/análisis.
- **Prompts one-shot**: "hacé un presupuesto" → resultado vago. **Enseñar**: estructura RACE + iterar.
- **Confianza ciega**: copiar-pegar draft sin revisar. **Enseñar**: "AI es herramienta de borrador, no publicador".
- **Compartir secretos**: pegar nombres de clientes, salarios, códigos internos. **Enseñar**: "Nunca pegues nada que no postearías en redes".

## 6. Casos de uso wow (ROI inmediato)

1. **Redacción de emails**: "draft profesional de respuesta a este mensaje" → ahorra 10 min/email.
2. **Resúmenes de reuniones**: pegar notas → bullets + action items.
3. **Fórmulas de Excel**: "escribí una fórmula que calcule X" o "explicá qué hace esta fórmula".
4. **Document Q&A**: subir PDF y preguntar.
5. **Traducción con preservación de tono**: "reformulá esto menos formal" / "traducí al inglés manteniendo el tono".
6. **Brainstorming**: "generame 5 asuntos para este email de lanzamiento".

Cada uno entrega valor en menos de 2 minutos de uso. Elegir 3–4 para demos en vivo.

## 7. Privacidad de datos (contenido mínimo viable)

Handout de una página:

- **Nunca compartir**: nombres de clientes, datos salariales, estrategias internas, código propietario, planes no publicados, datos médicos/legales.
- **Seguro compartir**: preguntas genéricas, estructuras de muestra (sin nombres reales), información pública.
- **Test rápido**: "¿Tuitearía esto?" — si no, no lo pegues.
- **Si existe**: usar la herramienta interna de la empresa en lugar del chatbot público.

## Fuentes

- zonetechai.com/2026/04/ai-literacy-guide-2026
- datacamp.com — Why Traditional AI Training Isn't Working in 2026
- parloa.com — Prompt Engineering Frameworks
- Stanford HAI — AI chatbot privacy risks (2025)
- Nucamp — Top 10 Workplace AI Use Cases 2025
