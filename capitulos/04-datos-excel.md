# Capítulo 4 — La estrella: sus datos en Claude

> **OBJETIVO CRÍTICO**: Este es el capítulo que justifica el día entero. En los próximos 50 minutos van a ver un archivo real de la empresa convertirse en insights accionables y un dashboard interactivo. Tienen que salir de acá queriendo abrirlo mañana a primera hora.

**Horario:** 11:50–12:40  
**Duración:** 50 minutos exactos  
**Requisitos previos:** Haber completado el Capítulo 3 (framework CQR). Todos en la sala entienden que la calidad del output depende de la calidad del input.

---

## Checklist de setup — HACER 60 MINUTOS ANTES

Este capítulo no puede improvisar. Hacer todo esto antes de que lleguen.

- [ ] **El Excel**: elegir 1 archivo real de la empresa, anonimizado. Nombres de clientes → "Cliente A/B/C". Montos reales OK si no son sensibles, o escalar por un factor fijo.
- [ ] **Limpiarlo**: eliminar macros, referencias a otras hojas externas, tablas dinámicas complejas. Dejar una sola hoja con datos planos, encabezados en fila 1, sin filas vacías intermedias.
- [ ] **Formato**: guardar como `.xlsx`. Peso objetivo: < 10 MB. Si pesa más, recortar columnas o filas innecesarias.
- [ ] **Testearlo en Claude**: subir el archivo con la misma cuenta que se usará en vivo. No asumir que funciona — verificarlo.
- [ ] **Ejecutar el prompt de dashboard** (ver sección 12:15): confirmar que el artifact renderiza sin errores.
- [ ] **Tomar screenshot** del dashboard funcionando. Guardarlo accesible (escritorio o tab abierta). Es el backup de emergencia.
- [ ] **Desactivar ad blockers** del navegador — algunos bloquean el render de artifacts.
- [ ] **Abrir nueva conversación limpia** (o el Project de la empresa) lista para la demo.

> **Nota crítica sobre fórmulas:** Claude ve los *valores calculados* de las celdas, no las fórmulas de Excel. Si alguien en la sala pregunta "¿puede explicar cómo se calcula el margen?", Claude no puede extraer `=B2/A2` del archivo. Para eso hay que copiar la fórmula como texto en el chat. Anticiparlo antes de que pase.

---

## 11:50 — Subir y preguntas básicas (10')

### Qué hacer en pantalla

Abrir claude.ai (la pestaña ya debería estar lista). Arrastrar el archivo `.xlsx` al chat — dejarlo caer encima del campo de texto. Esperar el tick de confirmación verde.

### Qué decir al grupo

> *"Acabo de darle acceso a los datos del último año. A partir de ahora puedo hacerle preguntas en castellano como si le estuviera preguntando a un analista. Sin fórmulas, sin filtros, sin tablas dinámicas. Solo preguntas."*

Hacer una pausa. Dejar que eso aterrice.

### Prompt 1 — Orientación inicial

Copiar y pegar textual:

```
Acabo de subir un archivo Excel con datos de la empresa.
Resumime en exactamente 5 bullets:
1. Qué datos contiene este archivo (columnas, período, estructura)
2. Qué métricas o indicadores principales aparecen
3. Tres cosas que te llaman la atención a primera vista
Sé concreto. No repitas lo que está en los encabezados — interpretalo.
```

Mientras Claude genera: *"Fíjense que no usé ninguna fórmula. No escribí un macro. Solo le pregunté como le preguntaría a un persona."*

**Después de la respuesta — pregunta de validación al grupo:**
> *"¿Coincide con lo que ustedes saben del archivo? ¿Hay algo raro, algo que se inventó, algo que falta? Esa es la primera verificación. Siempre."*

### Prompt 2 — El peor momento

```
¿Cuál fue el peor mes en términos de performance? Justificá con los datos que viste.
Si hay más de una métrica relevante, elegí la más significativa y explicá por qué la elegiste.
```

**Después de la respuesta:**
> *"¿Eso lo sabían? ¿Les cambiaría algo saberlo más rápido?"*

### Prompt 3 — Anomalías

```
¿Hay algún dato anómalo, outlier o inconsistencia en este archivo que merezca revisión humana?
Listalo con la fila o período aproximado y por qué te llama la atención.
Si no encontrás nada, decime que no encontraste nada — no inventes.
```

**Punto pedagógico clave** — decirlo en voz alta:
> *"Le pedí explícitamente que diga si no encontró nada. Eso es importante: si no lo especificamos, la AI a veces inventa un outlier para darte una respuesta útil. El prompt bien construido le cierra esa puerta."*

---

## 12:00 — Ellos dirigen (15')

### Apertura del bloque

> *"Hasta ahora les mostré mis preguntas. A partir de acá, el teclado lo sigo manejando yo, pero las preguntas las ponen ustedes. ¿Qué le preguntarían a estos datos si fueran el responsable de tomar decisiones?"*

Esperar. Si hay silencio: mirar a alguien específico, nombrarlo. *"Vos, desde tu área, ¿qué te interesa ver?"*

### Cómo manejar los tres tipos de pregunta que van a aparecer

**Tipo 1 — Pregunta muy vaga**

Ejemplo: *"¿Cómo venimos?"*

No esquivarla. Usarla como momento pedagógico:

> *"'Cómo venimos' es perfecta para un humano que tiene contexto compartido. Para Claude necesito ser un poco más específico — ¿venimos en qué? ¿volumen, margen, mix de producto, comparado con cuándo?"*

Reformular en vivo con el que hizo la pregunta. Tipear la versión mejorada. Mostrar la diferencia en el output.

**Tipo 2 — Pregunta muy específica sin los datos**

Ejemplo: *"¿Cuánto representa el cliente X en el margen neto después de descuentos?"*

> *"Buena pregunta. Pero si ese dato no está en el archivo, Claude no lo tiene. ¿Lo tenemos acá? Si no está, podemos estimarlo con lo que hay o te armo la estructura para cuando tengas ese dato."*

No es una falla — es una lección sobre los límites de la herramienta.

**Tipo 3 — Pregunta perfecta**

Ejemplo: *"¿Hay estacionalidad en las ventas? ¿Algún patrón que se repite?"*

Ejecutarla sin modificar. Dejar que Claude brille. Después:

> *"Esa pregunta está perfectamente formulada. ¿Ven por qué? Tiene contexto implícito, pide un análisis específico y no asume que el resultado va a ser de un tipo particular. Eso es CQR aplicado sin pensar en CQR."*

### Si se quedan callados — preguntas semilla para ofrecer

Si después de 20 segundos no hay voluntarios, ofrecer tres opciones y dejar que elijan:

> *"Tengo tres sugerencias. ¿Cuál les interesa más explorar?"*
>
> A) *¿Cuál es la tendencia de los últimos 3 meses comparada con el mismo período del año anterior?*
>
> B) *¿Qué categoría o segmento tiene el peor ratio de rendimiento vs. esfuerzo?*
>
> C) *Si tuviera que hacer un forecast del próximo trimestre con estos datos, ¿qué me diría?*

Que elijan. Que sientan que están dirigiendo el análisis.

---

## 12:15 — El dashboard en vivo (20')

### La pausa de anticipación

Antes de escribir el prompt, decir esto en voz alta:

> *"Lo que viene es el momento más visual del día. Voy a pedirle que genere un dashboard interactivo — gráficos, filtros, KPIs. En 15 o 20 segundos van a ver algo que en otro contexto hubiera tardado días en producción. Mirá la pantalla."*

### El prompt canónico — copiar textual

```
Con los datos del Excel que analizaste, generá un dashboard HTML interactivo.

Estructura exacta:
1. Fila superior: 3 tarjetas KPI con las métricas más importantes que encontraste (valor numérico grande, etiqueta abajo, variación respecto al período anterior si está disponible)
2. Gráfico de líneas: tendencia de la métrica principal a lo largo del tiempo (eje X = períodos, eje Y = valor)
3. Gráfico de barras: comparación entre las principales categorías o segmentos
4. Filtro desplegable en la parte superior derecha para segmentar por la dimensión más relevante de los datos

Diseño: paleta azul y gris corporativo. Sin colores saturados. Fuente limpia, sin ornamentos. Que se vea como una herramienta, no como una presentación.
Tecnología: Recharts para los gráficos, Tailwind CSS para el layout. Sin dependencias externas más allá de esas.
Requisito clave: el filtro debe funcionar — al seleccionar una opción, los gráficos deben actualizarse.
```

### La pausa dramática — instrucción para el instructor

Después de enviar el prompt: **no hablar durante el render**. Dejar el silencio. 10, 15, 20 segundos de spinner. Cuando el artifact empieza a aparecer línea por línea, decir en voz baja:

> *"Ahí va..."*

Cuando renderiza completo: silencio dos segundos más. Dejar que lo vean. Después:

> *"Eso. Un dashboard de ejecutivos. En 20 segundos. Con sus datos."*

### La iteración en vivo — este es el pico emocional

Mirar al grupo:

> *"¿Qué cambiarían? Una cosa. Lo que sea — otro tipo de gráfico, otros colores, agregar una métrica, sacar algo que no les sirve."*

Aceptar la primera sugerencia que llegue. Tipear la modificación en el chat, en lenguaje natural. Ejemplo:

```
Cambiá el gráfico de barras por un gráfico de área apilada.
Agregá una línea de promedio horizontal en el gráfico de líneas.
```

Enviar. Esperar el render. Cuando aparece:

> *"Eso es lo que cambia. No hay que volver a programar nada, no hay que llamar a IT, no hay que esperar al viernes. Le decís qué querés y lo regenera."*

**Este es el momento que tienen que recordar mañana.** No apurarlo. Dejar que lo absorban.

---

## 12:35 — Cierre del capítulo (5')

### Recapitulación final

Antes de cerrar, hacer esta pregunta al grupo:

> *"¿Qué acaba de pasar acá?"*

Escuchar. No interrumpir. Dejar que lo digan con sus palabras. Eso fija el aprendizaje mejor que cualquier resumen del instructor.

Después, la frase de cierre:

> *"Esto que acabamos de hacer en 50 minutos — hace un año era un proyecto de 3 semanas con un analista BI, reuniones de relevamiento, iteraciones de diseño, aprobaciones de IT. Eso no desapareció. Pero ahora tienen una forma de llegar al 80% de esa respuesta en el tiempo que tardó Claude en renderizar. Esa es la escala del cambio."*

Pause.

> *"En 10 minutos de descanso, si alguien quiere probar con su propio archivo, lo hacemos."*

---

## Recovery playbook — Fallas en vivo y cómo manejarlas

| Falla | Síntoma | Qué decir | Acción técnica |
|---|---|---|---|
| **Artifact en blanco** | El panel derecho aparece pero está vacío, sin error visible | *"El componente tiene un error silencioso. Claude a veces genera código con un bug menor. Dejame pedirle que lo corrija."* | Escribir en el chat: `"El artifact quedó en blanco. Revisá el código, identificá el error y regeneralo con manejo de errores explícito."` Si vuelve a fallar, pedir el código como texto y abrir en tab nueva con `data:text/html,...` |
| **Claude inventa un número** | Cita una cifra que no estaba en el archivo | *"Fíjense lo que acaba de pasar. Ese número no estaba en los datos. Claude lo estimó — o lo inventó. Regla de oro: si no lo pueden rastrear a una celda del Excel, no es confiable. Por eso siempre verificamos."* | Pedirle al grupo que señale la celda de origen. Si no existe, documentarlo como ejemplo de alucinación en contexto seguro |
| **Rate limit** | Claude muestra mensaje de límite de uso | *"Claude está pidiendo un respiro — pico de tráfico. Pasa en free tier. En producción, con una cuenta dedicada de empresa, esto no existe."* | Sacar el screenshot del dashboard pre-generado. Mostrar la imagen mientras pasa el límite (suele ser 30–60 segundos). Si hay segunda cuenta disponible, cambiar |
| **Archivo muy grande o parse lento** | Spinner durante más de 30 segundos al subir el archivo, o Claude dice que no puede acceder al contenido | *"El archivo es más pesado de lo ideal para esta demo. Tenemos un plan B."* | Subir la versión CSV del mismo archivo (exportar desde Excel como CSV antes del workshop). El CSV parsea siempre. Tenerlo listo en el escritorio |
| **WiFi lento o caído** | El chat no envía, o la respuesta nunca llega | *"La red corporativa a veces filtra o ralentiza estas plataformas. En el mundo real esto corre desde la laptop de cada uno con su propia conexión, no depende del WiFi de la sala."* | Mostrar el screenshot del dashboard. Si hay datos móviles disponibles, conectar el notebook por hotspot. Continuar la narrativa con el backup visual |
| **Claude pide explicar una fórmula del archivo** | Alguien pregunta "¿puede explicar cómo calcula el margen?" y Claude dice que no tiene acceso a las fórmulas | *"Momento importante: Claude ve los valores calculados, no las fórmulas de Excel. Es como si le mostráramos la planilla impresa — ve los números, no cómo se calcularon. Para explicar una fórmula, la pegamos como texto."* | Ir al Excel, copiar la fórmula de la celda (ej: `=B2/(A2+C2)*100`), pegarla en el chat y pedir la explicación |
| **El grupo no hace preguntas** | Silencio en el bloque "ellos dirigen" | *"Está bien. Les doy tres puntas — eligen la que más les interesa."* | Ofrecer las preguntas semilla del bloque 12:00. Nombrar a alguien específico y preguntarle sobre su área |
| **Respuesta demasiado larga o técnica** | Claude da una pared de texto o explicaciones estadísticas complejas | *"Le faltó instrucción de formato. Así se arregla."* | Escribir: `"Esa respuesta es correcta pero demasiado larga. Resumila en 3 bullets, lenguaje ejecutivo, sin tecnicismos."` Mostrar la diferencia |

---

> **Nota para el instructor:** Si llegás al momento del dashboard y todo sale bien — no apures el cierre. Los 5 minutos finales son los más valiosos del día. Deja que el silencio trabaje. El impacto se fija en el silencio, no en más información.
