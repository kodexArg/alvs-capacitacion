# Plan Maestro v2 — Workshop AI para Alta Dirección

**Fecha:** 2026-04-14 · **Horario:** 10:00–14:00 · **Audiencia:** 4 ejecutivos sin base previa en AI  
**Formato:** Presencial. Demo única desde notebook del instructor en monitor.  
**Herramienta primaria:** **Claude Desktop** (los usuarios están en Windows/Mac). Tour comparativo: ChatGPT, Gemini, Le Chat, DeepSeek.  
**Objetivo estrella:** Que salgan sabiendo interrogar un Excel propio con Claude y generar un dashboard en vivo con Artifacts.

---

## Principio rector (ajuste v2)

> **No es un curso — es un diálogo dirigido por ejecutivos.**
>
> No hay práctica individual. El formato es **socrático de alto calibre**: el instructor opera el teclado, **ellos dirigen** qué preguntar. Esto los pone en rol de decisores (lenguaje natural de un jefe) y evita la trampa del "sentate y mirá" que mata el engagement en adultos senior.
>
> La credibilidad del instructor se construye **admitiendo el rol**: *"No soy capacitador, soy su jefe de sistemas. Vamos a resolver esto juntos."* Esta honestidad vale más que cualquier MBA de formación.

---

## Grilla horaria definitiva

| # | Hora | Capítulo | Dur | Modo |
|---|------|----------|-----|------|
| 1 | 10:00–10:20 | **El hook: la AI falla en vivo** | 20' | Demo provocadora + diálogo |
| 2 | 10:20–11:00 | **Qué es realmente (y qué no) una AI** | 40' | Modelo mental + tour de herramientas |
| ☕ | 11:00–11:10 | Descanso activo | 10' | — |
| 3 | 11:10–11:50 | **Cómo se le habla: framework CQR** | 40' | Comparativa + ejercicio socrático |
| 4 | 11:50–12:40 | **La estrella: sus datos en Claude** (Excel + Artifact) | 50' | Demo con datos reales |
| ☕ | 12:40–12:50 | Descanso | 10' | — |
| 5 | 12:50–13:25 | **Tu asistente permanente: system prompts** | 35' | Construcción guiada por rol |
| 6 | 13:25–14:00 | **Gobernanza, objeciones y próximos 90 días** | 35' | Ética + Q&A + cierre estratégico |

---

## Capítulo 1 — El hook (10:00–10:20)

**Objetivo:** Romper el hielo con un momento de tensión real. Que en los primeros 3 minutos uno de ellos piense *"esto es más serio de lo que creía"*.

**Apertura literal (minuto 0–3):**
> *"Buenos días. No soy capacitador, soy su jefe de sistemas. Vamos a pasar 4 horas viendo cómo se usa esta tecnología — y sobre todo cuándo NO usarla. No vamos a seguir un guión. Ustedes van a dirigir los ejemplos. Yo manejo el teclado."*

**Demo de apertura (minuto 3–8): la AI falla**
- Pedir a ChatGPT un comunicado de prensa sobre la empresa real con datos específicos.
- Dejar que **alucine** una cifra, un partner, una fecha.
- Preguntar al grupo: *"¿Quién acá detectaría eso antes de que llegue al directorio?"*
- Pausar. Dejar el silencio incómodo.
- *"Ese es el trabajo de ahora. Esto no reemplaza el juicio de ustedes — lo amplifica. Si ustedes no revisan, nadie revisa."*

**Diálogo socrático (minuto 8–18):**
> *"Antes de seguir: ¿qué es lo primero que les viene a la cabeza cuando piensan en AI? ¿Miedo, curiosidad, hype, útil, amenaza? Una palabra cada uno."*

Anotar las 4 palabras en pizarra o doc abierto. Usarlas como referencia durante todo el workshop.

**Cierre del capítulo (minuto 18–20):**
> *"Hoy, al final, cada uno debería poder: (1) decir una forma en que esto cambia su área, (2) hacer una pregunta que van a llevar al directorio, (3) tener claro qué NO poner en un chatbot público. Si logramos esas tres cosas, el día valió la pena."*

---

## Capítulo 2 — Qué es realmente la AI (10:20–11:00)

**Objetivo:** Instalar el modelo mental mínimo viable + mostrar el panorama de herramientas sin perder profundidad.

### 2a — Modelo mental (10')

**La metáfora rectora:**
> *"Pensen en un becario brillante, que leyó todo internet, pero que a veces inventa cosas con total confianza. Eso es una AI generativa hoy. No 'piensa' — predice. No 'sabe' — reconoce patrones. Y a veces alucina."*

**3 ideas a instalar, nada más:**
1. **Es predicción de texto entrenada con billones de documentos.** No razonamiento.
2. **Tiene fecha de corte**: no sabe qué pasó esta semana.
3. **Alucina con confianza**: inventa cuando no sabe, sin avisar.

### 2b — Tour de herramientas (15')

Abrir cada pestaña, 2–3 minutos cada una. **Mensaje central**: todas hablan, todas entienden, difieren en *para qué sirve mejor cada una*.

**Dos protagonistas + contexto:** el tour tiene dos herramientas que sí vamos a usar mañana (Claude y Copilot) y cuatro que conviene conocer por nombre. Los ejecutivos se van con **dos atajos de adopción**, no con un catálogo.

| Herramienta | Estatus | Mensaje de 30 segundos | Qué mostrar |
|---|---|---|---|
| **Claude Desktop** ⭐ | Protagonista | "El más serio para análisis profundo y privacidad. **No entrena con tus datos por default.** Es el que vamos a usar la mayor parte del día." | App abierta, file upload, Projects |
| **Copilot M365** ⭐ | Protagonista | "Ya vive adentro de Word, Excel y Outlook. Con licencia corporativa los datos **nunca salen del tenant**. Si Claude es el analista externo, Copilot es el compañero de escritorio." | **Demo en vivo (2')**: abrir un Excel real, panel lateral de Copilot, un prompt ejecutivo |
| **ChatGPT** | Contexto | "El más conocido y versátil. Genera imágenes, navega web. **Entrena con tus datos salvo que lo desactives.**" | UI + dónde está el opt-out |
| **Gemini** | Contexto | "El de Google. Integra Gmail, Drive, Docs. Buen compañero si viven en Google Workspace." | Vista rápida |
| **Le Chat (Mistral)** | Contexto | "Europeo, privacy-first. Alternativa válida si Claude no funciona." | Vista rápida |
| **DeepSeek** | Contexto | "Chino, razonamiento barato. Se menciona para que sepan que existe." | Solo nombrarlo |

**La regla del día (el mensaje que se tienen que llevar):**
> *"Dos herramientas, dos lenguajes. **Claude** para análisis profundo, dashboards y cuando necesiten sacar los datos a trabajar. **Copilot** para el Excel, Word y Outlook de todos los días, adentro del archivo, con los datos nunca saliendo de la empresa."*

> **Nota de tiempo:** Copilot pasa de "mencionar" a "demo en vivo de 2 minutos" → el tour ahora es 2 protagonistas (3' c/u) + 4 menciones rápidas (1'–1.5' c/u). Total sigue siendo 15 minutos.

### 2c — Wow 1: eurotrip2026 (10')

Abrir https://eurotrip2026.kodexarg.com en el monitor.

**Guion:**
> *"Este sitio lo hice yo en un fin de semana, solo, sin agencia, sin diseñador. Con AI como copiloto. No es el sitio lo importante — es que pude dirigir el trabajo de alguien que tipea por mí. Ese es el cambio: ustedes, que dirigen equipos, ahora pueden dirigir también al software."*

### 2d — Wow 2: 2 demos rápidas dictadas por ellos (5')

- *"Antes del descanso, una cada uno: ¿qué quieren ver? ¿un email transformado? ¿una fórmula Excel explicada? ¿un resumen de un PDF?"*
- Tomar 2 sugerencias. Ejecutarlas en vivo. Sin guión.

---

## Capítulo 3 — Framework CQR (11:10–11:50)

**Objetivo:** Que tengan un método repetible para hablar con la AI. Que entiendan que la calidad del output = calidad del input.

### 3a — La idea central (5')

> **C**ontexto: ¿quién soy y en qué situación estoy?  
> **Q** (Consulta): ¿qué necesito exactamente?  
> **R**esultado esperado: ¿cómo quiero recibir la respuesta?

### 3b — Demo comparativa: pobre vs CQR (10')

Dos prompts al mismo problema, lado a lado:

| Prompt pobre | Prompt CQR |
|---|---|
| *"Resumí esto"* | *"Soy director de operaciones de una empresa de logística. Este es el acta de la reunión de directorio de ayer (3 páginas). Necesito un resumen ejecutivo de máximo 5 bullets, ordenados por urgencia, tono directo, sin jerga."* |

Mostrar ambos resultados en pantalla. La diferencia habla sola.

### 3c — Panorama de otros frameworks (5')

Mostrar de pasada que existen otros: **RACE** (Role/Action/Constraints/Example), **CO-STAR** (Context/Objective/Style/Tone/Audience/Response). Mensaje: *"Todos dicen lo mismo: contexto + qué + cómo. CQR es el que vamos a usar porque es más corto y en español."*

### 3d — Ejercicio socrático (20')

> *"Elijan un problema real de su trabajo actual — uno concreto, de esta semana. Vamos a construir el prompt CQR entre todos."*

Tomar uno. Reconstruirlo verbalmente:
- **C**: ¿quién sos en este caso? ¿qué sabe Claude antes de empezar?
- **Q**: ¿qué le estás pidiendo exactamente?
- **R**: ¿cómo querés la respuesta? ¿en bullets? ¿tabla? ¿párrafo?

El instructor tipea. Ejecutan. Iteran juntos si el resultado no cierra. **Repetir con otro caso si hay tiempo**.

---

## Capítulo 4 — La estrella: sus datos en Claude (11:50–12:40)

**Objetivo:** El momento de máximo impacto. Ver un Excel real convertirse en insights + dashboard interactivo en vivo.

### Setup previo (CRÍTICO — hacer 1 hora antes)

- [ ] Elegir 1 Excel real de la empresa, anonimizado
- [ ] **Simplificarlo**: eliminar macros, referencias externas, pivots. Dejar datos limpios con encabezados claros
- [ ] Guardar como .xlsx (<10MB idealmente)
- [ ] Probar subida a Claude web con la cuenta que se usará en vivo
- [ ] Ejecutar el prompt de dashboard canónico y verificar que renderiza
- [ ] Tomar screenshot del dashboard funcionando como backup
- [ ] Desactivar ad blockers del navegador

### 4a — Subir y preguntar (10')

Arrastrar el Excel al chat de Claude.
> *"Acabo de darle acceso a los datos del último año. Ahora puedo hacerle preguntas en castellano como si fuera un analista."*

**Primeras 3 preguntas (instructor las tiene listas):**
1. *"Resumime este archivo en 5 bullets: qué datos contiene, qué período cubre, 3 cosas que me llaman la atención."*
2. *"¿Cuál fue el peor mes y por qué? Usá solo los datos que viste."*
3. *"¿Hay algún dato anómalo o outlier que merezca revisión humana?"*

**Observación clave**: después de cada respuesta, recordar *"¿Cómo verificamos esto? Siempre se verifica lo crítico."*

### 4b — Ellos dirigen (15')

> *"¿Qué le preguntarían ustedes a estos datos? Pregunten fuerte — el sistema está para aguantar."*

Tomar preguntas reales. Ejecutarlas. Si alguna es muy vaga, **no escapar**: preguntar de vuelta *"¿a qué te referís con 'bien'? ¿margen, volumen, mix?"* — esa es la lección de cómo iterar con la AI.

### 4c — El dashboard en vivo (20')

**Prompt canónico:**
```
Generá un dashboard interactivo HTML con los datos del Excel que acabás de analizar. 
Incluí:
1. Tarjetas con 3 KPIs clave en la parte superior
2. Gráfico de líneas mostrando la tendencia del período
3. Gráfico de barras comparando las principales categorías
4. Un filtro desplegable para segmentar por [región/categoría/etc]
Paleta: azul y gris corporativo. Usá Recharts y Tailwind. Profesional, no de tutorial.
```

Esperar render (10–20 segundos). **Cuando aparece** → pausa dramática.

**Iteración en vivo:**
> *"¿Qué cambiarían? ¿Otro gráfico? ¿Otros colores? ¿Agregar otra métrica?"*

Aceptar una sugerencia, tipear la modificación, regenerar. **Este es el pico emocional del workshop**.

**Si falla:**
- Artifact no renderiza → *"A veces el código tiene un error silencioso. Dejame regenerar con chequeos."* → agregar "con manejo de errores" al prompt.
- Rate limit → *"Pico mundial de uso. En producción con cuenta dedicada esto no pasa."* → sacar el screenshot backup.
- Datos mal graficados → *"Mostrame primero qué datos estás usando, después graficá."*

### 4d — El cierre del capítulo (5')

> *"Esto que acabamos de hacer en 50 minutos — que hace un año era un proyecto de 3 semanas con un analista BI. Esa es la escala del cambio."*

---

## Capítulo 5 — System prompts (12:50–13:25)

**Objetivo:** Que cada uno diseñe verbalmente su "asistente permanente" adaptado a su rol.

### 5a — Qué es un system prompt (5')

> *"Es la instrucción permanente: quién sos vos, qué tono querés, qué formato, qué NUNCA hacer. Como configurar un asistente antes de que empiece a trabajar."*

### 5b — Demo comparativa (5')

Claude sin system prompt → responde genérico.  
Claude con system prompt de *"Gerente de operaciones, empresa de logística, respuestas directas en máximo 5 bullets, sin jerga, siempre pregunta si falta contexto"* → responde adaptado.

### 5c — Construyen el suyo (20')

**Plantilla guía en pantalla:**
```
Sos mi asistente ejecutivo.
Trabajo como [ROL] en [INDUSTRIA/EMPRESA].
Mi prioridad esta semana es [FOCO].
Cuando te consulte:
- Sé directo y breve (máximo [N] puntos)
- Usá lenguaje ejecutivo, sin tecnicismos innecesarios
- Si te falta contexto, preguntame antes de asumir
- Terminá siempre con "¿Querés que profundice en algún punto?"
NUNCA:
- Inventes cifras
- Uses clichés
- Me hagas cumplidos antes de contestar
```

**Recorrer los 4 participantes, uno por uno.** Cada uno dicta su versión. El instructor tipea. Guarda el system prompt en un Project de Claude a nombre de esa persona. Testean con una consulta real de ese ejecutivo. **Al terminar el bloque, los 4 tienen un "asistente" personalizado listo para usar al día siguiente**.

### 5d — Cierre (5')

> *"Este system prompt es suyo. Mañana lo abren, lo pegan en Claude, y ya están listos para trabajar. Yo se los mando por email al final del día."*

---

## Capítulo 6 — Gobernanza, objeciones y próximos 90 días (13:25–14:00)

**Objetivo:** Cierre de alto calibre. Instalar la agenda estratégica, no solo la técnica.

### 6a — Qué nunca pegar (5')

**Lista corta, una pantalla:**
- Datos de clientes con nombres reales
- Información salarial, contractual o de RRHH
- Estrategias no publicadas, M&A, pricing interno
- Contratos, documentos legales
- Código propietario crítico

**Regla simple:** *"Si no lo publicarías en LinkedIn con tu nombre, no lo pegues en un chatbot público."*

**Matiz importante:** Claude por default **no** entrena con tus datos. ChatGPT y Gemini por default **sí**. Esto cambia el cálculo de riesgo.

### 6b — Limitaciones reales (5')

1. **Alucinaciones**: inventa con confianza. Verificar lo crítico siempre.
2. **Fecha de corte**: no sabe qué pasó recientemente.
3. **No razona**: reconoce patrones. No tiene juicio humano.
4. **No reemplaza decisiones**: amplifica al decisor, no lo sustituye.

### 6c — Manual de objeciones ejecutivas (10')

Preguntar abiertamente: *"¿Qué los frena para que esto sea algo serio en su área mañana?"* Responder con las respuestas preparadas (ver `research/04-hallazgos-clave-v2.md` — sección objeciones).

Principales a tener listas:
- "Alucina" → "Por eso no es para decisiones binarias, es para drafting y detección de anomalías."
- "Mis datos son confidenciales" → "Separás datos de herramienta. O usás Claude (no entrena por default)."
- "Va a reemplazar gente" → "Automatiza tareas, no puestos. Los puestos se corren a juicio."
- "Es hype" → "Puede ser. El costo de probarlo es 4 horas. El costo de llegar tarde es problema de directorio."

### 6d — Los próximos 90 días (10')

**Propuesta concreta al grupo:**

> *"No les pido fe, les pido un piloto acotado. Cada uno elige un caso de uso chico de su área, lo prueba con Claude durante 30 días, y nos juntamos a ver qué aprendimos. Go/no-go al final."*

**Outcomes que deberían llevarse hoy:**
1. Un caso de uso concreto en mente ("en mi equipo, esto serviría para...")
2. Una pregunta de gobernanza para la próxima reunión de directorio
3. Haber visto en vivo una alucinación y una recuperación
4. Un system prompt personalizado listo para usar
5. La idea de un piloto de 90 días con criterio de decisión

### 6e — Cierre (5')

> *"La AI no va a reemplazar a los que toman decisiones. Pero los que sepan usarla van a tomar mejores decisiones, más rápido, con más información. Hoy dieron el primer paso — y lo más importante: saben cuándo NO confiar. Con eso alcanza para arrancar."*

---

## Artefactos a producir (Sonnets en paralelo)

| Archivo | Agente | Foco |
|---|---|---|
| `capitulos/01-hook.md` | Sonnet 1 | Apertura + demo de falla + diálogo inicial |
| `capitulos/02-que-es-ai.md` | Sonnet 2 | Modelo mental + tour + eurotrip |
| `capitulos/03-framework-cqr.md` | Sonnet 3 | CQR + comparativa + ejercicio socrático |
| `capitulos/04-datos-excel.md` | Sonnet 4 | Excel + dashboard + recuperación |
| `capitulos/05-system-prompts.md` | Sonnet 5 | System prompts + construcción por rol |
| `capitulos/06-gobernanza-cierre.md` | Sonnet 6 | Ética + objeciones + 90 días |
| `capitulos/00-guion-minuto-a-minuto.md` | Sonnet 7 | Cue cards del instructor |
| `capitulos/00-prompts-prearmados.md` | Sonnet 8 | Todos los prompts listos para copy-paste |

---

## Checklist pre-workshop (esta noche / mañana temprano)

- [ ] Claude Desktop instalado y con sesión iniciada
- [ ] Cuenta Claude (Pro si posible para velocidad y límites)
- [ ] Excel real de la empresa, simplificado, anonimizado, <10MB
- [ ] Testear subida + prompt de dashboard con ese Excel
- [ ] Screenshot del dashboard funcionando (backup)
- [ ] eurotrip2026.kodexarg.com abierto en tab
- [ ] ChatGPT, Gemini, Le Chat, DeepSeek abiertos en tabs
- [ ] Prompts pre-armados en un archivo de texto para copy-paste rápido
- [ ] Ad blockers desactivados
- [ ] Verificar red corporativa: acceso libre a claude.ai, chatgpt.com, gemini.google.com, chat.mistral.ai
