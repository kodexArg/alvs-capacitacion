# Capítulo 2 — Qué es realmente (y qué no) una AI

| | |
|---|---|
| **Objetivo** | Instalar el modelo mental mínimo viable + panorama de herramientas sin perder profundidad |
| **Horario** | 10:20–11:00 (40 minutos exactos) |
| **Materiales** | Este guion + tabla de herramientas impresa o en segundo monitor |
| **Tabs/apps a tener abiertos ANTES de empezar** | Claude Desktop · chatgpt.com · gemini.google.com · chat.mistral.ai · chat.deepseek.com · eurotrip2026.kodexarg.com |
| **Herramienta primaria** | Claude Desktop (Windows/Mac) |

---

## 10:20 — Modelo mental (10')

### Qué decir

*"Antes de ver las herramientas, necesito que todos tengamos la misma imagen en la cabeza. Una sola metáfora, tres ideas. Nada más."*

Pausa. Mirar al grupo.

*"Imaginen un becario brillante. Leyó todo internet — libros, artículos, foros, manuales técnicos, miles de millones de páginas. Tiene una memoria fotográfica para patrones. Pero tiene un problema grave: cuando no sabe algo, en vez de decir 'no sé', inventa — y lo hace con total confianza, sin titubear. Eso es una AI generativa hoy."*

Pausa. Dejar que eso aterrice.

*"Con eso en mente, tres ideas que les pido que recuerden al salir de acá:"*

**Idea 1 — No razona, predice:**

*"Esto no piensa. No razona como un abogado o un contador. Predice cuál es la próxima palabra más probable, dado todo lo que vio. A veces esa predicción es brillante. A veces es completamente inventada. El problema es que el mecanismo es el mismo en ambos casos — no hay señal de advertencia."*

**Idea 2 — Tiene fecha de corte:**

*"El conocimiento se congeló en algún momento del año pasado. No sabe qué pasó la semana pasada. No sabe si la empresa que mencionaron firmó una adquisición ayer. Si le preguntan por algo reciente, va a responder igual de seguro — con información desactualizada o inventada."*

**Idea 3 — Alucina con confianza:**

*"Esto es lo más peligroso para nosotros como usuarios. La AI no dice 'esto no lo sé'. Dice algo que suena correcto, bien redactado, con estructura, con datos específicos — y esos datos pueden ser completamente falsos. Ya lo vieron antes con el comunicado de prensa. Eso no fue un error del sistema. Eso es el funcionamiento normal."*

> **Nota instructor:** Ahora preguntas socráticas. No avances hasta tener respuestas reales del grupo. Esto ancla los conceptos mejor que cualquier slide.

### Preguntas al grupo (elegir 2, no las 4)

- *"¿En qué área de su trabajo sería más peligroso que una AI alucine un dato? ¿Compras? ¿Legal? ¿Comunicación?"*
- *"Si un becario real les entregara algo con este nivel de confianza pero potencialmente inventado, ¿qué proceso tendrían para verificarlo?"*
- *"¿Alguien usa ya alguna de estas herramientas? ¿Qué notaron?"*
- *"¿Cuál de las tres ideas les preocupa más en relación a su área?"*

Escuchar. No corregir. Anotar lo que digan — aparecen de nuevo en el Capítulo 6.

*"Bien. Con ese modelo mental claro, ahora les muestro qué herramientas existen hoy."*

---

## 10:30 — Tour de herramientas (15')

### Qué decir (intro)

*"Hay seis herramientas que tienen que conocer por nombre. Pero hoy dos de ellas son las protagonistas — las otras cuatro las menciono para que sepan que existen. Las dos protagonistas las van a usar ustedes a partir de mañana: **Claude Desktop** para análisis profundo, y **Copilot** — el de Microsoft — para lo que ya hacen todos los días adentro de Excel y Word."*

### Tabla comparativa (mostrar en pantalla o imprimir)

| Herramienta | Rol hoy | Mensaje de 30 segundos | Qué mostrar en vivo | Privacidad por default |
|---|---|---|---|---|
| **Claude Desktop** ⭐ | **Protagonista** | El más serio para análisis profundo y privacidad. **No entrena con sus datos por default.** Es el que usamos la mayor parte del día. | App abierta, file upload, ícono de Projects | ❌ NO entrena |
| **Copilot M365** ⭐ | **Protagonista** | Ya vive adentro de Word, Excel y Outlook. Con licencia corporativa los datos **nunca salen del tenant de la empresa**. Si Claude es el analista externo, Copilot es el compañero de escritorio. | **Demo en vivo**: abrir un Excel, panel lateral, un prompt ejecutivo | ❌ NO entrena con datos del tenant |
| **ChatGPT** | Contexto | El más conocido y versátil. Genera imágenes, navega la web. Pero por default sí usa tus datos para entrenamiento. | Mostrar Settings → Data Controls → el opt-out | ✅ SÍ entrena por default |
| **Gemini** | Contexto | El de Google. Vive integrado con Gmail, Drive, Docs. Natural si todo su trabajo está en Google Workspace. | Vista rápida del UI | ✅ SÍ entrena por default |
| **Le Chat** (Mistral) | Contexto | Europeo, privacidad primero. Alternativa válida si Claude no funciona. | Vista rápida del UI | ❌ NO entrena por default |
| **DeepSeek** | Contexto | Chino, razonamiento barato. Lo mencionamos para que sepan que existe. No lo usamos. | Solo nombrarlo | Ambiguo |

> **Nota instructor:** 15 minutos de tour = **3' Claude + 3' Copilot (demo en vivo) + 1' cada una de las otras 4 (4' total) + 5' de márgen para preguntas o transición**. Las dos protagonistas son donde te detenés; las otras son vuelo de reconocimiento. Si alguien pregunta mucho sobre una herramienta de contexto, decí *"buena pregunta, anotalo para el Q&A del final"* y seguís.

### Guion por herramienta

**Claude** (3 min — la más importante):

Abrir claude.ai.

*"Esta es la que usamos hoy. Interfaz limpia. Acá arriba pueden subir archivos — Excel, PDF, imágenes. Y acá a la izquierda ven Projects: una forma de guardar instrucciones permanentes para que Claude recuerde quién sos cada vez que lo abrís."*

*"Lo más importante de Claude para ustedes: por default, no usa sus conversaciones para entrenar el modelo. Lo que pegan acá, queda acá. Eso es lo único que les pido que recuerden del tour completo."*

---

**ChatGPT** (2 min):

Abrir chatgpt.com.

*"El más conocido. Cuatro años siendo el referente. Tiene cosas que Claude no tiene: genera imágenes, navega la web en tiempo real."*

*"El tema de privacidad: por default, sí usa tus datos. Hay un opt-out, pero tenés que ir a Settings → Data Controls y desactivarlo. Si van a usar ChatGPT con archivos de la empresa, lo primero es hacer eso."*

Mostrar el camino hasta Data Controls. No explicar en detalle.

---

**Gemini** (2 min):

Abrir gemini.google.com.

*"El de Google. Si el trabajo de ustedes vive en Gmail, Drive y Docs, este tiene una ventaja natural: puede leer sus archivos directamente, sin que tengan que subirlos."*

*"Misma advertencia que ChatGPT: entrena con tus datos por default."*

Mostrar integración con Drive si está disponible. Sino, solo el UI.

---

**Le Chat** (1 min):

Abrir chat.mistral.ai.

*"Europeo. La regulación europea de privacidad los obliga a tener estándares más altos. No entrena con tus datos. Si algún día Claude no funciona por alguna razón, este es el plan B."*

Vista rápida del UI. Nada más.

---

**DeepSeek** (30 segundos):

Abrir o mencionar.

*"Chino. Razonamiento matemático y técnico muy bueno, precio muy bajo. Lo mencionamos para que sepan que existe. No lo usamos hoy por los temas de privacidad — no tienen declaración clara sobre qué hacen con los datos."*

---

**Copilot** (30 segundos, sin abrir):

*"Copilot de Microsoft. Hasta el 15 de abril — la semana pasada — era la opción integrada gratis con Word, Excel y PowerPoint. Microsoft lo limitó drásticamente. Hoy es solo un chat web. No es candidato serio por ahora."*

---

### Cierre del tour

*"Resumen de una frase: todas hablan, todas entienden, difieren en para qué sirve mejor cada una. Y si mañana van a subir un archivo de la empresa sin leer 40 páginas de términos, la opción más segura por default es Claude. Eso es lo que usamos hoy."*

---

## 10:45 — Wow 1: eurotrip2026 (10')

> **Nota instructor:** Abrir la tab de eurotrip2026.kodexarg.com que ya tenés preparada. Si la red es lenta, abrir antes del capítulo.

### Qué decir

Abrir https://eurotrip2026.kodexarg.com en pantalla completa.

*"Cambio de tema. Les muestro algo personal."*

Dejar que vean el sitio. Desplazar lentamente.

*"Este sitio lo hice yo. Un fin de semana. Solo. Sin agencia, sin diseñador, sin equipo técnico. Con AI como copiloto."*

Pausa.

*"Pero lo importante no es el sitio. Lo importante es lo que cambió para poder hacerlo. Yo no escribí el código. Yo no diseñé los layouts. Yo dirigí. Le dije a la AI qué quería, revisé lo que generó, le dije qué cambiar, iteré. Como dirigen ustedes a un equipo — pero con alguien que tipea veinte veces más rápido que cualquier persona y no se cansa."*

Pausa.

*"El cambio que les propongo es este: ustedes, que dirigen equipos, ahora pueden dirigir también al software. No necesitan saber programar. Necesitan saber qué quieren y cómo pedirlo. Eso lo practican toda la vida — es lo que hacen en cada reunión."*

*"¿Alguien tiene algún caso en su área donde quisieran poder hacer algo así? Un informe que hoy depende de que un analista tenga tiempo, o una presentación que demora tres días porque tienen que coordinar con diseño."*

Escuchar 1–2 respuestas. No profundizar — hay un Q&A al final.

*"Bien. Antes del descanso, quiero que me digan qué quieren ver."*

---

## 10:55 — Wow 2: demos en vivo dictadas por ellos (5')

> **Nota instructor:** Esta sección no tiene guion fijo. Son ellos los que mandan. Tu trabajo es ejecutar limpio y rápido. Tener claude.ai abierto y listo.

### Qué decir

*"Dos minutos para cada uno. Me dicen qué quieren ver — lo hago en vivo, sin preparación. ¿Qué les sería útil ver hoy?"*

Esperar. Si el grupo no propone nada en 5 segundos, ofrecer semillas:

**Semillas (leer una por una, parar cuando alguien levante la mano):**

- *"¿Quieren ver cómo transforma un email largo en tres bullets?"*
- *"¿Una fórmula de Excel explicada en palabras?"*
- *"¿Un borrador de respuesta a un mensaje difícil?"*
- *"¿Un resumen de un documento que tengan en el celular?"*
- *"¿Cómo planificar la agenda de una reunión de directorio con temas que me dicten?"*

Tomar la primera sugerencia. Ejecutar. Mostrar el resultado. No editar — mostrar lo que sale.

Tomar la segunda sugerencia. Ejecutar. Si hay tiempo, tercera.

> **Nota instructor:** Si la respuesta no es buena, no la ocultes. Decí: *"Fíjense — no es perfecto. Ahora le damos más contexto y lo iteramos."* Esa iteración en vivo enseña más que un resultado perfecto.

*"Eso es lo que vamos a hacer durante las próximas tres horas. Pero primero, diez minutos de descanso."*

---

## Resumen de tiempos

| Subsección | Inicio | Fin | Duración |
|---|---|---|---|
| Modelo mental | 10:20 | 10:30 | 10' |
| Tour de herramientas | 10:30 | 10:45 | 15' |
| Wow 1 — eurotrip2026 | 10:45 | 10:55 | 10' |
| Wow 2 — demos libres | 10:55 | 11:00 | 5' |
| **Total** | | | **40'** |

---

## Checklist pre-capítulo

- [ ] Tabs abiertos: claude.ai, chatgpt.com, gemini.google.com, chat.mistral.ai, chat.deepseek.com, eurotrip2026.kodexarg.com
- [ ] claude.ai: sesión iniciada, lista para usar
- [ ] eurotrip2026.kodexarg.com: cargado y funciona
- [ ] Tabla de herramientas visible (pantalla o impresa)
- [ ] Semillas de Wow 2 a la vista (post-it o segundo monitor)
