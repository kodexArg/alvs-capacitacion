# Capítulo 3 — Cómo se le habla: framework CQR

| | |
|---|---|
| **Objetivo** | Que cada participante tenga un método repetible para hablar con la AI. Que quede claro que la calidad del output depende directamente de la calidad del input. |
| **Duración** | 40 minutos exactos (11:10–11:50) |
| **Modo** | Comparativa en pantalla + ejercicio socrático con problemas reales del grupo |

---

## 11:10 — La idea CQR (5 minutos)

**Arrancar directo, sin introducción larga.**

> *"Ya vieron qué es esto, ya vieron cómo falla. Ahora viene la parte práctica: cómo se le habla para que funcione. Hay un método. Se llama CQR. Son tres letras, tres preguntas, y las tres son de sentido común."*

Escribir en pantalla — en el chat de Claude, o en un doc abierto — las tres líneas:

```
C — Contexto: ¿quién soy y en qué situación estoy?
Q — Consulta: ¿qué necesito exactamente?
R — Resultado: ¿cómo quiero recibir la respuesta?
```

**Explicar la analogía del empleado nuevo:**

> *"Imaginen que acaban de contratar un empleado nuevo, muy capaz, pero que no sabe nada de la empresa todavía. Si lo mandan a buscar 'información sobre el proveedor', vuelve con cualquier cosa. Pero si le dicen: 'Soy el gerente de compras, tenemos una reunión mañana con Proveedor X, necesito los puntos clave de las últimas tres negociaciones, en tres bullets, tono directo' — ahí sí saben qué van a recibir. Claude es exactamente ese empleado. Brillante, pero literalmente no sabe nada de ustedes a menos que se lo digan."*

**Las tres preguntas, una por una:**

- **C — Contexto**: ¿Quién sos vos en esta situación? ¿Qué rol, qué empresa, qué momento? Claude no sabe que son ejecutivos, no sabe qué industria, no sabe si el documento es confidencial o público. Tienen que decírselo.

- **Q — Consulta**: ¿Qué le están pidiendo exactamente? No "resumí esto" — "resumí los tres riesgos principales del proyecto". Cuanto más preciso, mejor el resultado.

- **R — Resultado esperado**: ¿Cómo querés la respuesta? ¿Cinco bullets? ¿Un párrafo? ¿Tono formal? ¿Para mandar directo o para editar? Esto lo define el output casi tanto como la consulta.

> *"Tres preguntas. Las mismas que le harían a cualquier persona antes de delegarles una tarea."*

---

## 11:15 — Demo comparativa: prompt pobre vs. prompt CQR (10 minutos)

**Presentar el escenario:**

> *"Vamos a usar el mismo problema con dos prompts distintos. El primero como lo escribe la mayoría la primera vez. El segundo con CQR. Miren la diferencia."*

**Ejemplo A — Resumen de acta de directorio**

Prompt pobre (pegar en Claude, ejecutar, mostrar resultado):
```
Resumí este texto.
[pegar acta de directorio de 3 páginas]
```

Prompt CQR (pegar en Claude, ejecutar, mostrar resultado):
```
Soy el director general de una empresa de consumo masivo en Argentina. 
Acabo de recibir el acta de la reunión de directorio del jueves pasado 
(3 páginas). Necesito un resumen ejecutivo de máximo 5 bullets, 
ordenados por urgencia para mi agenda de la semana. 
Tono directo, sin jerga corporativa, sin introducción.
[pegar acta]
```

**Reacción esperada del grupo**: El primer resultado es genérico, enumerativo, sin criterio de prioridad. El segundo recorta, prioriza, usa el lenguaje de quien pregunta. La diferencia debería ser obvia sin explicar nada.

> *"¿Ven la diferencia? No cambió el documento. No cambió Claude. Cambió cómo se lo pedimos."*

**Si quieren ver un segundo ejemplo, usar este:**

Prompt pobre:
```
Analizá esto.
[pegar tabla de variación de ingresos por mes]
```

Prompt CQR:
```
Soy el CFO de una empresa de servicios. Adjunto una tabla con ingresos 
mensuales del último año. Necesito identificar los 2 meses con mayor 
desvío negativo respecto al promedio y una hipótesis de causa para 
cada uno, basada solo en los datos que ves. Respuesta en tabla de 
dos columnas: Mes / Hipótesis. Sin conclusiones generales.
[pegar tabla]
```

> *"Con el segundo prompt, Claude ya sabe que son datos de ingresos, que soy CFO, que me interesa el desvío, y que no quiero texto de relleno. Le di el contexto de un jefe a un analista."*

---

## 11:20 — Panorama de otros frameworks (5 minutos)

> *"Una aclaración para cuando lean sobre esto en otro lado, porque hay otros nombres para lo mismo."*

Escribir en pantalla:

```
RACE  → Role / Action / Constraints / Example
CO-STAR → Context / Objective / Style / Tone / Audience / Response
CQR   → Contexto / (Q)onsulta / Resultado
```

> *"RACE tiene cuatro partes, CO-STAR tiene seis. Todos dicen lo mismo: contale quién sos, qué necesitás, y cómo lo querés. CQR es el que vamos a usar hoy porque es más corto, está en español, y tiene las tres preguntas que importan. Si en algún momento leen 'RACE' o 'CO-STAR', no hay conflicto — son compatibles. Son distintos nombres para el mismo criterio."*

**Mensaje a reforzar una sola vez:**

> *"El framework no es la magia. La magia es que ahora tienen tres preguntas que hacerse antes de tipear. Eso solo ya mejora el 80% de los prompts."*

No profundizar más. Cinco minutos para este bloque, seguir.

---

## 11:25 — Ejercicio socrático en grupo (20 minutos)

**Este es el núcleo del capítulo. No hay demo preparada — el material lo aportan ellos.**

### Apertura

> *"Ahora viene la parte que importa. Necesito que alguien me traiga un problema real de su semana. Algo que tengan sobre el escritorio ahora mismo, que les esté consumiendo tiempo, que tengan que resolver. No tiene que ser importante — puede ser chico. Yo tipeo, nosotros construimos el prompt entre todos, y lo corremos."*

Esperar. Dar 10–15 segundos de silencio antes de ayudar.

**Recuperación 1 — Si nadie ofrece un problema:**

> *"Les doy un ejemplo de arranque: ¿alguno tiene que preparar un briefing para una reunión esta semana? ¿Un correo difícil de redactar? ¿Un informe que está pendiente? Cualquier cosa que en condiciones normales les llevaría media hora."*

Si siguen sin aportar:

> *"Perfecto, entonces yo propongo uno genérico y después lo ajustamos a algo de ustedes. Imaginen que tienen una reunión mañana con un proveedor clave que está pidiendo un aumento de precio del 18%. Necesitan preparar los argumentos para la negociación. ¿Cómo armaríamos el CQR?"*

### Construcción del prompt — Guion socrático

Una vez que hay un problema sobre la mesa, construir verbalmente con estas preguntas, en este orden:

**Paso C:**
> *"¿Quién sos vos en este caso? No tu nombre — tu rol, tu contexto en esta situación. ¿Qué debería saber Claude antes de empezar?"*

Esperar respuesta. Reformular en voz alta: *"Entonces el contexto es: [repetir lo que dijeron]."*

**Paso Q:**
> *"¿Qué le estás pidiendo exactamente? No en general — lo más concreto posible. ¿Qué querés que Claude haga con eso?"*

Esperar. Si es vago:
> *"¿Querés que redacte algo, que analice algo, que te dé opciones, que te haga un resumen? Cuanto más preciso, mejor."*

**Paso R:**
> *"¿Cómo querés recibir la respuesta? ¿Bullets, tabla, párrafo? ¿Largo o corto? ¿Para compartir o solo para vos?"*

### Tipear, ejecutar, mostrar

Armar el prompt en voz alta mientras se tipea, para que todos lo vean construirse. Ejecutar. Leer el resultado en pantalla junto con el grupo.

**Si el resultado cierra:**

> *"¿Esto les sería útil tal cual? ¿Lo usarían mañana?"*

Dejar que respondan. No apurarse.

**Si el resultado no cierra — Recuperación 2:**

> *"El primer intento no siempre es el definitivo. Eso no es un problema — es parte del método. Vamos a iterar."*

Preguntar al grupo qué faltó. Agregar o ajustar el prompt. Ejecutar de nuevo. Mostrar que la segunda versión es mejor.

> *"Esto se llama iterar. No es que fallamos — es que afinamos. Es lo que hace cualquier analista cuando le hacen una devolución."*

### Si hay tiempo — Segunda ronda

> *"¿Alguien más tiene un caso? Ahora que vieron cómo funciona, el segundo es más rápido."*

Repetir el proceso. El segundo ejercicio suele fluir mejor porque el grupo ya tiene el modelo en la cabeza.

### Meta emocional del ejercicio

El objetivo no es demostrar que Claude funciona. El objetivo es que cada persona vea **su propio problema** resolverse con un método que ellos construyeron. Ese es el click. No apurarse, no llenar el silencio, dejar que el resultado respire.

---

## Cierre del capítulo (al llegar a 11:50)

> *"CQR no es magia — es disciplina. Las mismas tres preguntas que le harían a un analista antes de delegarle algo. La diferencia es que esto responde en 10 segundos. Guárdense las tres preguntas. Contexto, Consulta, Resultado. Cada vez que tipeen algo en Claude, chequeen si pusieron las tres."*

---

## Prompts exactos — Copy-paste ready

### Demo A: Acta de directorio

**Prompt pobre:**
```
Resumí este texto.
```

**Prompt CQR:**
```
Soy el director general de una empresa de consumo masivo en Argentina. 
Acabo de recibir el acta de la reunión de directorio del jueves pasado 
(3 páginas). Necesito un resumen ejecutivo de máximo 5 bullets, 
ordenados por urgencia para mi agenda de la semana. 
Tono directo, sin jerga corporativa, sin introducción.
```

---

### Demo B: Variación de ingresos

**Prompt pobre:**
```
Analizá esto.
```

**Prompt CQR:**
```
Soy el CFO de una empresa de servicios. Adjunto una tabla con ingresos 
mensuales del último año. Necesito identificar los 2 meses con mayor 
desvío negativo respecto al promedio y una hipótesis de causa para 
cada uno, basada solo en los datos que ves. 
Respuesta en tabla de dos columnas: Mes / Hipótesis. Sin conclusiones generales.
```

---

### Demo C: Briefing para reunión con proveedor (backup si nadie aporta caso)

**Prompt CQR:**
```
Soy gerente de compras de una empresa manufacturera. Tengo una reunión 
mañana con un proveedor clave que está pidiendo un aumento de precios 
del 18% por inflación de insumos. Necesito los 4 argumentos más sólidos 
para resistir o reducir ese aumento, con datos de contexto que pueda 
usar en la negociación. Formato: bullets numerados. Tono: directo, 
sin diplomacia innecesaria.
```

---

## Tabla de recuperaciones

| Situación | Qué hacer |
|---|---|
| Nadie aporta un problema | Ofrecer los ejemplos B o C de este doc. Después preguntar de vuelta si alguno quiere adaptar el ejemplo a su caso real. |
| El problema aportado es muy vago | Preguntar: *"¿Qué vas a hacer con esa respuesta? ¿Quién la va a leer?"* Eso suele clarificar. |
| El problema es muy específico y necesita datos que no están | Decir: *"Claude solo trabaja con lo que le damos. ¿Tenés el dato, o queremos que trabaje con supuestos?"* |
| El resultado sale mal o es genérico | Iterar en vivo. Mostrar que refinar el prompt es parte del proceso, no un error. |
| Se va el tiempo antes del segundo caso | *"Quedamos en deuda con el segundo ejemplo. Al final de la tarde lo hacemos si hay tiempo."* |

