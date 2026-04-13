# Capítulo 5 — Tu asistente permanente: system prompts

**Objetivo:** Que cada uno de los 4 ejecutivos termine el bloque con un system prompt personalizado guardado en un Project de Claude, adaptado a su rol, que ya probaron en vivo.  
**Horario:** 12:50–13:25 (35 minutos exactos)  
**Entregable esperado:** 4 archivos de texto con system prompts — uno por persona — enviados por email al cierre del día.

---

## 12:50 — Qué es un system prompt (5 minutos)

**Texto literal del instructor:**

> "Hasta ahora le estuvimos hablando a la AI como si fuera un asistente genérico que no nos conoce. Cada vez que abrían un chat nuevo, empezaban de cero. Eso se termina.
>
> Un system prompt es la instrucción permanente que le das a la AI sobre quién sos y cómo querés que te responda. Lo configurás una vez y queda. No le repetís cada vez 'soy director de operaciones de una empresa de logística' — lo decís una vez y listo."

**Acción en pantalla:** Abrir claude.ai. Ir a Projects (barra lateral izquierda). Mostrar que un Project tiene una sección "Instructions" separada del chat.

> "En Claude esto se llama Project. Cada uno de ustedes va a tener el suyo. Cuando lo abran mañana, Claude ya sabe quién son, qué rol tienen y cómo hablarles. Es como configurar un asistente antes de que empiece a trabajar — sin tener que repetirle el contexto cada vez."

**Qué NO es:** No es magia. No hace que Claude sea más inteligente. Hace que sea más *relevante para ustedes*.

---

## 12:55 — Demo comparativa (5 minutos)

**Setup:** Tener dos tabs abiertas — una conversación limpia sin Project, y el Project de demo ya configurado.

**Prompt de prueba (el mismo para los dos):**

```
Resumí los puntos principales de nuestra reunión de ayer: revisamos el forecast de ventas Q2, hubo discrepancias en los números de la región norte, y quedó pendiente una decisión sobre si renovar el contrato con el proveedor logístico.
```

### Tab 1 — Sin system prompt

**Acción:** Pegar el prompt en una conversación nueva, sin contexto previo. Ejecutar.

**Resultado esperado (típico):** Claude va a dar un resumen genérico, bullet points correctos pero impersonales, sin jerarquía ejecutiva, probablemente mencione "puntos de acción" de forma vaga, tono de analista junior.

> "Ven cómo respondió como si le hubiera mandado esto cualquier persona. Sin idea de si soy jefe, analista o pasante."

### Tab 2 — Con system prompt de rol específico

**System prompt del Project de demo (ya cargado):**

```
Sos mi asistente ejecutivo.
Trabajo como Director de Operaciones en una empresa de logística mediana (200 empleados, operación nacional).
Mi prioridad esta semana es cerrar la revisión del forecast Q2 antes del viernes.
Cuando te consulte:
- Sé directo y breve (máximo 4 puntos por respuesta)
- Usá lenguaje ejecutivo, sin tecnicismos innecesarios
- Jerarquizá siempre: primero lo urgente, después lo importante
- Si te falta contexto, preguntame antes de asumir
- Terminá siempre con "¿Querés que profundice en algún punto?"
NUNCA:
- Inventes cifras
- Uses clichés como "excelente pregunta" o "por supuesto"
- Me hagas cumplidos antes de contestar
```

**Acción:** Pegar el mismo prompt. Ejecutar.

**Resultado esperado:** Claude prioriza la discrepancia en región norte (problema urgente), identifica la decisión pendiente del contrato como punto de acción con nombre, tono más ejecutivo, jerarquía clara, termina preguntando si quiere profundizar.

> "El prompt que mandé fue idéntico. Lo que cambió es que Claude sabe quién soy y cómo hablarme. Eso es lo que van a tener ustedes en 20 minutos."

---

## 13:00 — Los 4 construyen el suyo (20 minutos — 5 por persona)

### Plantilla en pantalla (mantenerla visible todo el bloque)

```
Sos mi asistente ejecutivo.
Trabajo como [ROL] en [INDUSTRIA].
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

---

### Flujo por persona (5 minutos cada uno)

**Minuto 1 — Preguntarle (30 segundos)**

El instructor hace tres preguntas en voz alta:

1. *"¿Cuál es tu título exacto y en qué industria operan?"*
2. *"¿Cuál es tu prioridad concreta de esta semana — un proyecto, una decisión, una presentación?"*
3. *"¿Cómo preferís que te respondan — bullets cortos, párrafo, con y sin recomendación?"*

Escuchar. Tomar nota mental o en papel. No interrumpir.

**Minuto 2 — Armar el prompt (1 minuto)**

El instructor tipea en vivo, completando la plantilla con las palabras exactas del ejecutivo. No parafrasear — usar su vocabulario.

**Minuto 3 — Crear el Project (30 segundos)**

- Clic en "New Project" en la barra lateral de claude.ai
- Nombre del proyecto: el nombre o iniciales del ejecutivo (ej: "JM — Dir Comercial")
- Pegar el system prompt en el campo "Instructions"
- Guardar

**Minuto 4 — Testear con una consulta real (2 minutos)**

Preguntarle al ejecutivo: *"¿Qué le preguntarías ahora mismo sobre tu trabajo de esta semana?"*

Tipear su consulta real. Ejecutar. Dejar que vea la respuesta.

Si la respuesta no cierra del todo: ajustar el system prompt en el momento, una línea, y ejecutar de nuevo. Mostrar que se puede editar.

**Minuto 5 — Confirmar y guardar (30 segundos)**

> *"¿Esto es tuyo? ¿Reconocés tu lenguaje?"*

Si dice sí: perfecto. Copiar el system prompt a un documento de texto aparte (para el email del cierre).

Si dice no del todo: cambiar una línea más. No sobre-optimizar — el punto es que funciona, no que sea perfecto.

**Objetivo emocional por turno:** Cuando termina su turno, el ejecutivo tiene que sentir *"este es MI asistente"*, no *"esto es una demo genérica"*.

---

### Manejo de excepciones (durante los 20 minutos)

**Si alguien no tiene claridad sobre su rol o prioridad:**

> *"No necesitás definirlo perfecto ahora. Ponemos tu título y algo que tengas arriba del escritorio esta semana. Después lo ajustás en 30 segundos solo, desde tu notebook."*

Seguir con la plantilla base. No perder el turno en reflexión filosófica.

**Si alguien quiere algo muy complejo ("quiero que sepa de finanzas, de RRHH, de contratos..."):**

> *"Todo eso lo podés agregar, pero los mejores system prompts son los más simples. Empezamos con lo core y en dos semanas lo expandís. Lo simple que funciona vale más que lo complejo que confunde."*

Cortar educadamente. Mantener el ritmo.

**Si alguien no participa o se abstrae:**

Ir a ellos primero o último — no en el medio. Hacer la pregunta directa, no abierta:

> *"¿Cuál es tu título? ¿Qué tenés en el calendario esta semana que sea importante?"*

Si aun así no quieren participar: armar un prompt genérico para su rol conocido, testearlo con un caso hipotético, y ofrecerle el texto al final. No forzar — el objetivo emocional no se logra por presión.

---

### Tres ejemplos terminados — para inspiración o fallback

Si alguien se bloquea, o si el instructor necesita mostrar adónde apunta la plantilla, usar estos como referencia:

#### (a) Director Comercial

```
Sos mi asistente ejecutivo.
Trabajo como Director Comercial en una empresa de servicios B2B (industria tecnológica, mercado Argentina/Latam).
Mi prioridad esta semana es preparar la revisión de pipeline Q2 para el board del viernes.
Cuando te consulte:
- Sé directo y breve (máximo 5 puntos por respuesta)
- Usá lenguaje comercial: hablar de deals, conversión, ticket promedio, no de "oportunidades de negocio"
- Si no tenés datos del pipeline real, decime qué dato necesitás antes de asumir
- Terminá siempre con "¿Querés que profundice en algún punto?"
NUNCA:
- Inventes cifras ni porcentajes que no te di
- Uses frases de coaching como "enfocate en tus fortalezas"
- Me hagas cumplidos antes de contestar
```

#### (b) Director de Operaciones

```
Sos mi asistente ejecutivo.
Trabajo como Director de Operaciones en una empresa de distribución con operación en 3 provincias (150 empleados).
Mi prioridad esta semana es resolver un problema de tiempos de entrega en la zona norte.
Cuando te consulte:
- Sé directo y breve (máximo 4 puntos, ordenados de mayor a menor urgencia)
- Usá lenguaje operativo: hablar de SLA, lead time, inventario, no de "eficiencia sistémica"
- Si te falta un dato (cantidad de vehículos, rutas, proveedores), preguntame antes de improvisar
- Terminá siempre con "¿Querés que profundice en algún punto?"
NUNCA:
- Inventes números de operación que no te di
- Sugieras soluciones que requieren presupuesto adicional sin pedirme el contexto
- Me hagas cumplidos antes de contestar
```

#### (c) Director Financiero

```
Sos mi asistente ejecutivo.
Trabajo como Director Financiero en una empresa de manufactura mediana (facturación anual ~USD 15M).
Mi prioridad esta semana es cerrar la revisión de márgenes por línea de producto antes del cierre mensual.
Cuando te consulte:
- Sé directo y breve (máximo 4 puntos por respuesta)
- Usá lenguaje financiero preciso: margen bruto, EBITDA, desvío, no "rentabilidad general"
- Si necesitás un número que no te di, pedímelo explícitamente
- Terminá siempre con "¿Querés que profundice en algún punto?"
NUNCA:
- Inventes cifras, ratios ni benchmarks sin indicar que son estimaciones
- Mezclés criterios contables sin aclararlos
- Me hagas cumplidos antes de contestar
```

---

## 13:20 — Cierre del capítulo (5 minutos)

**Acción en pantalla:** Mostrar los 4 Projects creados en la barra lateral de Claude — uno por persona, con su nombre.

**Texto literal del instructor:**

> "Listo. Los 4 tienen su asistente. No el asistente genérico de internet — el de ustedes. Con su rol, su industria, su prioridad de esta semana.
>
> Al final del día les mando por email los 4 system prompts. Lo único que tienen que hacer es: abrir claude.ai, ir a Projects, crear uno con su nombre, y pegar el texto. Treinta segundos. Y arrancan a trabajar.
>
> Esto es lo más concreto que se llevan hoy. Mañana lo abren, lo pegan, y ya están trabajando con un asistente que sabe quiénes son."

**Pausa de 2 segundos. No agregar más.**

Pasar directamente al Capítulo 6.

---

## Notas operativas del instructor

- El instructor opera el teclado en todo momento. Los ejecutivos dictan verbalmente.
- Tener abierto un documento de texto (Gedit, mousepad, o similar) para copiar los 4 system prompts terminados. Al final del día, pegarlos en un email.
- Si un Project tarda en guardar o hay problema de login: tener la plantilla lista para copiarla en el campo de "System prompt" de cualquier conversación nueva — funciona igual, sin Project.
- El tiempo por persona es estricto. Si alguien se extiende, cerrar educadamente: *"Perfecto, lo tenemos. Guardamos esto y seguimos."*
- No pedir aprobación del grupo sobre el system prompt de cada persona — la personalización es individual, no colectiva.
