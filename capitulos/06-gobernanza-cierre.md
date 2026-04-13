# Capítulo 6 — Gobernanza, objeciones y próximos 90 días

**Objetivo:** Cierre de alto calibre. Que salgan con claridad sobre qué no pegar, respuestas para sus equipos, y un compromiso concreto de piloto.  
**Duración:** 35 minutos exactos (13:25–14:00)  
**Modo:** Socrático + diálogo dirigido por el grupo

---

### Outcomes del workshop completo (checklist mental del instructor)

Al terminar hoy, cada uno debería poder:

1. Articular un caso de uso concreto en su área
2. Identificar una pregunta de gobernanza para el próximo directorio
3. Haber visto en vivo una alucinación y una recuperación
4. Tener un system prompt personalizado listo para usar mañana
5. Comprometerse a un piloto de 90 días con criterio de decisión

---

## 13:25 — Qué nunca pegar (5')

**Al grupo:**
> "Antes de cerrar, quiero que se lleven una regla que vale más que cualquier política de IT que yo les pueda mandar después."

Abrir una pantalla en blanco o una nota. Escribir la lista mientras se dice en voz alta:

---

### ⛔ NUNCA pegar en un chatbot público

| Categoría | Ejemplo concreto |
|---|---|
| Datos de clientes | Nombre, CUIT, contrato, historial |
| RRHH | Salarios, legajos, evaluaciones, desvinculaciones |
| Estrategia no publicada | M&A, pricing interno, pipeline comercial |
| Documentos legales | Contratos firmados, NDA, disputas |
| Código propietario crítico | Algoritmos de negocio, sistemas core |

---

**Regla mnemotécnica — decirla lento, que la escuchen:**
> "Si no lo publicarías en LinkedIn con tu nombre, no lo pegues en un chatbot público."

Pausa. Repetir si hace falta.

**Matiz importante — esto sí hay que aclararlo:**
> "Ahora bien: hay una diferencia entre herramientas que importa mucho. Claude, por configuración por default, **no entrena sus modelos con lo que vos le mandás**. Es privacy-first. ChatGPT y Gemini, en las cuentas gratuitas, **sí lo hacen por default** — tenés que ir a configuración y desactivarlo explícitamente. Esto cambia el cálculo de riesgo si tienen que elegir una herramienta rápido."

Si alguien pregunta "¿y con cuenta paga?": *"Con cuentas enterprise, todas ofrecen garantías más fuertes. Pero si el equipo está usando cuentas personales, Claude es la opción más segura sin tocar nada."*

---

## 13:30 — Limitaciones reales (5')

**Al grupo:**
> "Ya las vimos en acción durante el día, pero las repaso rápido porque necesito que las lleven escritas, no solo vividas."

Cuatro limitaciones. Sin vueltas:

**1. Alucinaciones**
Inventa con total confianza. Sin avisar. Lo vimos en el cap 1. Regla: todo lo crítico se verifica con la fuente.

**2. Fecha de corte**
No sabe qué pasó en los últimos meses. Si le preguntás por una ley nueva, una fusión reciente, un evento de esta semana — no lo sabe, o peor, inventa algo que suena plausible.

**3. No razona**
Reconoce patrones extraordinariamente bien. Pero no tiene juicio humano. No entiende el contexto político de una organización, las relaciones de poder, lo que no está escrito en ningún lado. Eso sigue siendo de ustedes.

**4. No decide**
Amplifica al decisor — no lo sustituye. La firma, la responsabilidad, el criterio: son humanos. Siempre.

> "Con eso claro, vamos a lo que sé que quieren hablar."

---

## 13:35 — Manual de objeciones (10')

**Abrir el diálogo:**
> "¿Qué los frena a que esto sea algo serio en su área mañana? No me digan lo que creen que yo quiero escuchar — díganme la objeción real que van a tener cuando lleguen a la oficina y se lo cuenten al equipo."

Esperar. Dejar el silencio. Si no sale nada en 10 segundos, mirar a uno: *"¿Vos qué objeción te imaginás?"*

Usar las respuestas como trampolín. Las cinco más comunes:

---

### "Pero alucina"

> "Sí. Alucina. No voy a decirte que no. Por eso no lo usás para decisiones donde el error no tiene vuelta atrás. Lo usás para redactar el primer borrador que alguien después revisa. Para sintetizar 40 páginas en 5 bullets que vos corroborás. Para detectar anomalías en datos que un analista después valida. Como Excel: nadie le pide al Excel que decida el presupuesto. Le pide que muestre los candidatos posibles."

---

### "Es una caja negra"

> "La transparencia es un horizonte de madurez de la tecnología, no el problema de hoy. La pregunta de hoy es: ¿cómo lo deployamos con control? Con workflows de aprobación. Con auditoría de outputs. Con firma humana antes de cualquier acción. Mismo estándar que cualquier herramienta de alto impacto que ya usan."

---

### "Mis datos son confidenciales"

> "Separás datos de herramienta. Antes de pegar algo, lo anonimizás o lo resumís: en vez de 'el cliente Empresa X tiene una deuda de $2M', ponés 'un cliente del segmento industrial tiene una deuda importante'. Para lo verdaderamente sensible, existen modelos que corren dentro de tu infraestructura, on-premise, sin salir a internet. Pero la pregunta de fondo es otra: ¿prohibimos Excel con datos de clientes, o ingenieriamos controles para usarlo bien?"

Si alguien dice "pero igual me da miedo": *"Correcto. Y ese miedo convierte en política. No en prohibición — en protocolo."*

---

### "Va a reemplazar gente"

> "McKinsey publicó en 2026 que la AI automatiza el 57% de las *tareas* de un puesto típico de oficina. No el 57% de los puestos — las tareas. Los puestos se corren de ejecución a juicio. El analista que hoy carga datos va a necesitar saber qué hacer con el output que la AI genera. Eso no es recorte — es upskilling. El riesgo real no es que la AI reemplace a tu gente. Es que tu competidor, que sí actualizó a su gente, te gane mercado."

---

### "Es hype"

> "Puede ser. Yo no sé si esto va a ser tan grande como dicen, o si hay una corrección en camino. Lo que sí sé es que los competidores no están esperando para averiguarlo. Y el costo de equivocarnos en esta dirección es 4 horas y unos dólares de API. El costo de equivocarnos en la otra dirección — de llegar tarde — es un problema de directorio, no de sistemas."

---

**Si aparece una objeción que no está en la lista:**

No improvisar filosofía. Usar esta estructura:
1. *"Esa es exactamente la pregunta que va a hacer el directorio."*
2. *"¿Cómo la contestarían ustedes?"* — devolver al grupo
3. Si nadie tiene respuesta: *"Anotala. Es una de las preguntas de gobernanza que se llevan hoy."*

Nunca mentir, nunca prometer lo que no existe.

---

## 13:45 — Los próximos 90 días (10')

**Al grupo:**
> "No les pido fe. No les pido que crean que esto va a cambiar todo. Les pido un piloto acotado."

Propuesta concreta:

> "Cada uno elige un caso de uso chico — algo de su área, de esta semana o la próxima — y lo prueba con Claude durante 30 días. No necesita ser perfecto, no necesita ser el caso de uso definitivo. Solo necesita ser algo real. Nos juntamos en mayo, vemos qué aprendimos, y tomamos una decisión: seguimos, escalamos, o descartamos. Go/no-go al final. Sin compromiso previo."

**Pausa. Mirar al grupo:**
> "¿Qué caso de uso tiene cada uno en mente?"

Recorrer los 4. Escuchar. Anotar en el doc o en la pantalla. No juzgar, no corregir — solo anotar. Si alguien no tiene nada: *"¿Qué tarea tuya es hoy repetitiva y de alto volumen?"* Eso suele alcanzar.

Ejemplos que se pueden sugerir si alguien se queda en blanco:
- Resúmenes de reuniones o actas de directorio
- Redacción de comunicaciones internas o externas
- Análisis exploratorio de reportes antes de presentarlos
- Respuestas a consultas frecuentes del equipo

**Los 5 outcomes del día — decirlos en voz alta:**

> "Para que tengan claro lo que se llevan hoy:"

1. Un caso de uso concreto en mente — lo acaban de definir
2. Una pregunta de gobernanza para el próximo directorio — la identificaron recién
3. Haber visto en vivo una alucinación y una recuperación — lo hicimos en el cap 1
4. Un system prompt personalizado listo para usar mañana — lo construimos juntos en el cap 5
5. La idea de un piloto de 90 días con criterio de decisión — lo estamos definiendo ahora

---

## 13:55 — Cierre (5')

**Frase final — sin apuro, con pausa:**

> "La AI no va a reemplazar a los que toman decisiones. Pero los que sepan usarla van a tomar mejores decisiones, más rápido, con más información. Hoy dieron el primer paso — y lo más importante: saben cuándo NO confiar. Con eso alcanza para arrancar."

Silencio de 2–3 segundos.

**Cierre logístico:**
> "Esta tarde les mando por email: los 4 system prompts que construimos hoy, los prompts que usamos en el workshop, y el link directo a Claude. Cualquier pregunta durante la semana, me escriben directamente. Gracias."

---

## Notas del instructor

**Si el tiempo se come:** El bloque de limitaciones (13:30) es el más comprimible. En 2 minutos se puede hacer un barrido rápido si ya los vieron en acción durante el día.

**Si hay objeciones extra tiempo:** Cortar con: *"Esa la anotamos para el follow-up. Si intentamos resolver todo acá, llegamos a la siguiente reunión sin piloto definido."*

**Si el grupo no quiere comprometerse con el piloto:** No empujar. Decir: *"Perfecto. Lo dejo propuesto. Cada uno decide a qué velocidad avanza. Lo que no quiero es que salgan sin saber cómo empezar — y eso ya lo tienen."* El objetivo es que no salgan con miedo, sino con opciones.

**Tono del cierre:** Cálido, no vendedor. La AI no es la respuesta a todo — es una herramienta más, que ellos ahora saben usar. Eso es suficiente para hoy.
