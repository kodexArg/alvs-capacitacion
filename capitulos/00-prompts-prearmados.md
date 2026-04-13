# Prompts prearmados — Workshop AI para Alta Dirección

> Archivo de referencia para el instructor. Mantenerlo abierto durante todo el workshop.
> Cada prompt se copia y pega tal cual. Los `[CORCHETES]` son los únicos placeholders a completar en vivo.

---

## Capítulo 1 — El hook (10:00–10:20)

---

### `cap1-falla-comunicado`

**Cuándo usarlo:** Primeros 5 minutos del día. Pegar en ChatGPT (no en Claude). Dejar que alucine. No corregir nada.

```
Necesito un comunicado de prensa para distribuir mañana.
La empresa se llama [NOMBRE REAL DE LA EMPRESA].
Incluí los siguientes datos reales:
- Crecimiento del último año: [PORCENTAJE REAL O INVENTADO]
- Nombre del CEO: [NOMBRE REAL]
- Proyecto emblemático reciente: [PROYECTO REAL]
- Fecha de fundación: [AÑO REAL]

El comunicado debe tener tono corporativo formal, 3 párrafos, y mencionar planes de expansión para el próximo trimestre.
```

**Resultado esperado:** ChatGPT inventará al menos un dato (socio inexistente, cifra falsa, fecha incorrecta). Ese momento es el gancho del día.

---

## Capítulo 2 — Qué es realmente la AI (10:20–11:00)

---

### `cap2-wow-email`

**Cuándo usarlo:** Demo rápida en sec. 2d. Pegar en Claude. Si es posible, usar un hilo real de la empresa que alguien del grupo mencione.

```
Tengo este hilo de emails de los últimos días. Convertilo en una lista de tareas pendientes ordenadas por urgencia.
Para cada tarea: quién es el responsable (si se puede inferir del hilo), la fecha límite mencionada (o "sin fecha" si no hay), y una línea con qué hay que hacer.

Hilo de emails:
[PEGAR EL HILO AQUÍ — puede ser texto copiado de Outlook o Gmail]
```

**Resultado esperado:** Lista estructurada con responsables, fechas y acciones. Contrasta dramáticamente con el caos del hilo original.

---

### `cap2-wow-formula`

**Cuándo usarlo:** Demo rápida en sec. 2d. Pegar la fórmula como texto — NO subir el archivo de Excel (Claude solo ve valores calculados, no fórmulas del archivo).

```
Explicame en castellano simple qué hace esta fórmula de Excel, como si se la explicaras a alguien que no sabe de Excel pero sí entiende de negocios:

=SI(Y(C2>0,D2/C2>0.15),SUMA(E2:E12)*0.05,"Sin bonificación")

¿Qué calcula? ¿Cuándo se activa? ¿Qué significa el resultado?
```

**Resultado esperado:** Explicación en lenguaje de negocio: "Si el mes tuvo ventas y el margen superó el 15%, se aplica un 5% de bonificación al total acumulado. Si no, no hay bonificación."

---

### `cap2-wow-resumen-pdf`

**Cuándo usarlo:** Demo rápida en sec. 2d. Subir un PDF real (informe de sector, reporte, acta). Si no hay PDF disponible, usar texto copiado.

```
Resumí este documento en exactamente 5 bullets.
Criterio de selección: solo lo que cambia una decisión de negocio esta semana.
No incluyas contexto general ni introducción — solo los hallazgos que importan.
Terminá con una línea: "Pregunta que esto genera:" y formulá la pregunta estratégica más relevante que surge del documento.
```

**Resultado esperado:** 5 bullets accionables + una pregunta estratégica que el grupo puede debatir en sala.

---

### `cap2-wow-traduccion-tono`

**Cuándo usarlo:** Demo rápida si alguien del grupo menciona comunicaciones internacionales.

```
Traducí este párrafo al inglés. Mantené el tono ejecutivo formal — que suene como si lo escribiera el VP de una empresa de Fortune 500, no como una traducción automática.
Después de la traducción, agregá una línea: "Nivel de registro: [formal/neutro/informal]" para confirmar el tono.

Párrafo a traducir:
[PEGAR PÁRRAFO EN CASTELLANO]
```

**Resultado esperado:** Traducción con tono ejecutivo nativo en inglés, notablemente mejor que Google Translate.

---

## Capítulo 3 — Framework CQR (11:10–11:50)

---

### `cap3-pobre`

**Cuándo usarlo:** Primer prompt de la comparativa. Pegar en Claude. Mostrar el resultado antes de mostrar el prompt CQR.

```
Resumí esto.
```

**Resultado esperado:** Claude va a pedir aclaraciones o dar una respuesta genérica. Ese es el punto — mostrar que sin contexto, el output no sirve.

---

### `cap3-cqr-acta`

**Cuándo usarlo:** Segundo prompt de la comparativa. Pegar en Claude inmediatamente después de `cap3-pobre`. Si hay un acta real, subirla. Si no, pegar texto de ejemplo.

```
Soy director de operaciones de una empresa de logística nacional.
Este es el acta de la reunión de directorio de ayer (pego el texto completo abajo).
Necesito un resumen ejecutivo con las siguientes características:
- Máximo 5 bullets
- Ordenados por urgencia (primero lo que tiene deadline esta semana)
- Tono directo, sin jerga de consultoría
- Si hay un punto sin responsable asignado, marcarlo con "(sin dueño)"

[PEGAR TEXTO DEL ACTA AQUÍ]
```

**Resultado esperado:** Resumen estructurado y jerarquizado que contrasta visiblemente con la respuesta de `cap3-pobre`.

---

## Capítulo 4 — Sus datos en Claude (11:50–12:40)

> Recordatorio: subir el Excel ANTES de ejecutar estos prompts. Arrastrar el .xlsx al chat y esperar confirmación verde.

---

### `cap4-resumen-excel`

**Cuándo usarlo:** Primer prompt después de subir el Excel. Da orientación al grupo sobre qué hay en el archivo.

```
Acabo de subir un archivo Excel con datos de la empresa.
Resumime en exactamente 5 bullets:
1. Qué datos contiene este archivo (columnas, período, estructura)
2. Qué métricas o indicadores principales aparecen
3. Tres cosas que te llaman la atención a primera vista
Sé concreto. No repitas lo que está en los encabezados — interpretalo.
```

**Resultado esperado:** Descripción clara del contenido + 3 observaciones preliminares que abren el diálogo con el grupo.

---

### `cap4-peor-mes`

**Cuándo usarlo:** Segundo prompt del capítulo 4. Genera debate inmediato — todos quieren saber la respuesta.

```
¿Cuál fue el peor mes del período analizado y por qué?
Usá solo los datos que acabás de ver en el archivo — no asumas nada que no esté ahí.
Si hay varias métricas posibles (ventas, margen, volumen), elegí la que consideres más representativa y explicá por qué la elegiste.
```

**Resultado esperado:** Identificación del mes más débil con justificación en datos. Si Claude elige una métrica distinta a la que el grupo esperaba, es una conversación valiosa.

---

### `cap4-outliers`

**Cuándo usarlo:** Tercer prompt del capítulo 4. El más revelador para ejecutivos — suelen aparecer cosas que nadie había visto.

```
¿Hay algún dato anómalo, outlier o inconsistencia en este archivo que merezca revisión humana?
Para cada anomalía que encuentres: describila, decime en qué fila o período aparece, y cuál sería la explicación más probable (error de carga, caso excepcional, o señal real).
No inventes anomalías si no las ves. Si todo parece consistente, decilo.
```

**Resultado esperado:** Lista de 2-5 anomalías con contexto. La instrucción "no inventes" reduce alucinaciones en este prompt específico.

---

### `cap4-dashboard-canonico`

**Cuándo usarlo:** El prompt estrella. Ejecutar después de las preguntas exploratorias. Pegar exactamente así — es el momento de mayor impacto visual del workshop.

```
Generá un dashboard interactivo HTML con los datos del Excel que acabás de analizar.
Incluí:
1. Tarjetas KPI en la parte superior con: el valor total del período, el promedio mensual, y el mejor mes
2. Gráfico de líneas mostrando la evolución completa del período
3. Gráfico de barras comparando las principales categorías o segmentos
4. Un filtro desplegable que permita ver los datos de una sola región o categoría

Especificaciones técnicas:
- Usá Recharts para los gráficos y Tailwind para los estilos
- Paleta: azul corporativo (#1e40af) y gris neutro (#6b7280), fondo blanco
- Que se vea profesional, no de tutorial — sin bordes gruesos, sin colores chillones
- Los KPI cards deben mostrar el número grande arriba y una etiqueta descriptiva abajo
- El filtro debe funcionar en tiempo real sin recargar la página
```

**Resultado esperado:** Dashboard interactivo que renderiza en 10-20 segundos en el panel de Artifacts. Filtros funcionales. Aspecto ejecutivo.

---

### `cap4-iteracion-color`

**Cuándo usarlo:** Primera iteración después de que aparece el dashboard. Preguntar al grupo qué cambiarían — si dicen "los colores", usar este prompt.

```
Cambiá la paleta de colores del dashboard:
- Color principal: verde oscuro (#166534)
- Color secundario: gris cálido (#78716c)
- Fondo de las tarjetas KPI: blanco con borde verde suave
Mantené todo lo demás igual.
```

**Resultado esperado:** Dashboard regenerado con la nueva paleta en 10-15 segundos. Demuestra que iterar es trivial.

---

### `cap4-iteracion-grafico`

**Cuándo usarlo:** Si el grupo quiere cambiar el tipo de gráfico de líneas a barras o viceversa.

```
En el dashboard que generaste: cambiá el gráfico de líneas por un gráfico de área (area chart).
El área debe ser semitransparente (opacity 0.3) con el mismo color que la línea.
Todo lo demás queda igual.
```

**Resultado esperado:** Mismo dashboard con el gráfico de líneas reemplazado por área rellena. Iteración limpia.

---

### `cap4-agregar-metrica`

**Cuándo usarlo:** Si el grupo pide agregar una métrica extra al dashboard. Adaptar `[NOMBRE DE LA MÉTRICA]` en vivo.

```
Agregá una cuarta tarjeta KPI al dashboard con [NOMBRE DE LA MÉTRICA — ej: "variación vs año anterior", "ticket promedio", "cantidad de transacciones"].
Si ese dato no está disponible directamente en los datos que analizaste, calculalo de la forma más razonable posible y aclaralo debajo de la tarjeta.
El estilo debe ser idéntico a las otras tres tarjetas.
```

**Resultado esperado:** Cuarta tarjeta KPI integrada al diseño existente, con nota si el cálculo requirió una estimación.

---

## Capítulo 5 — System prompts (12:50–13:25)

---

### `cap5-sin-prompt`

**Cuándo usarlo:** Primera parte de la demo comparativa. Pegar en una conversación nueva sin ningún Project activo.

```
Resumí los puntos principales de nuestra reunión de ayer: revisamos el forecast de ventas Q2, hubo discrepancias en los números de la región norte, y quedó pendiente una decisión sobre si renovar el contrato con el proveedor logístico.
```

**Resultado esperado:** Resumen genérico, impersonal, sin jerarquía ejecutiva. Tono de analista junior. Ese contraste es el punto.

---

### `cap5-con-prompt`

**Cuándo usarlo:** Segunda parte de la comparativa. Pegar el mismo prompt de `cap5-sin-prompt` en el Project de demo (que ya tiene el system prompt del Director de Operaciones cargado).

> El prompt a pegar es el mismo que `cap5-sin-prompt`. Lo que cambia es el contexto del Project.

**Resultado esperado:** Resumen con jerarquía ejecutiva, tono directo, sin jerga, y la pregunta final "¿Querés que profundice en algún punto?" — exactamente como configuró el system prompt.

---

### `cap5-plantilla`

**Cuándo usarlo:** Mostrar en pantalla como punto de partida para que cada ejecutivo construya el suyo. Pegar en el Project de esa persona mientras dictan en voz alta.

```
Sos mi asistente ejecutivo.
Trabajo como [ROL] en [INDUSTRIA — ej: empresa de logística, retail, manufactura].
Mi prioridad esta semana es [FOCO ACTUAL — ej: cerrar el presupuesto Q3, evaluar un proveedor nuevo].

Cuando te consulte:
- Sé directo y breve (máximo [N — ej: 4] puntos por respuesta)
- Usá lenguaje ejecutivo, sin tecnicismos innecesarios
- Jerarquizá siempre: primero lo urgente, después lo importante
- Si te falta contexto, preguntame antes de asumir
- Terminá siempre con "¿Querés que profundice en algún punto?"

NUNCA:
- Inventes cifras o datos que no te di
- Uses clichés como "excelente pregunta" o "por supuesto"
- Me hagas cumplidos antes de contestar
- Des respuestas de más de [N — ej: 6] párrafos sin que te lo pida
```

**Resultado esperado:** Plantilla visible en pantalla que cada ejecutivo personaliza dictando en voz alta.

---

## Capítulo 6 — Gobernanza y cierre (13:25–14:00)

---

### `cap6-pilot-scoping`

**Cuándo usarlo:** Si en el bloque de cierre algún ejecutivo pide ver cómo arrancar un piloto. También sirve como tarea para llevar.

```
Actuá como consultor de implementación de AI con experiencia en empresas medianas de [INDUSTRIA].
Ayudame a diseñar un piloto de 90 días para implementar AI en [CASO DE USO CONCRETO — ej: "análisis de reportes de ventas semanales", "respuesta a consultas frecuentes de clientes"].

El piloto debe incluir:
1. Alcance exacto: qué entra y qué no entra en estos 90 días
2. Criterios de go/no-go al día 30 y al día 90 (métricas concretas, no conceptos)
3. Quién necesita estar involucrado (roles, no nombres)
4. Riesgos principales y cómo mitigarlos
5. Qué necesitamos para arrancar la semana que viene

Sé específico. Evitá lenguaje de consultoría genérico.
```

**Resultado esperado:** Plan de piloto estructurado con criterios de decisión concretos. Accionable para llevar al directorio.

---

## Prompts de recuperación

> Para cuando algo falla en vivo. Copiar y pegar sin explicar demasiado — la fluidez transmite confianza.

---

### `rec-artifact-vacio`

**Cuándo usarlo:** El dashboard aparece en blanco o el panel de Artifacts no muestra nada.

```
El dashboard no se renderizó — quedó en blanco. Regeneralo con las siguientes correcciones:
1. Antes de dibujar cada gráfico, verificá que el array de datos tenga al menos un elemento
2. Agregá un mensaje de error visible si algún dato no carga ("No hay datos para mostrar")
3. Envolvé el componente principal en un try/catch que muestre el error en pantalla en lugar de silenciarlo
El diseño y los datos que usabas son correctos — solo corregí el manejo de errores.
```

**Resultado esperado:** Dashboard regenerado con manejo de errores explícito. Si el problema era un error silencioso, ahora va a aparecer visible y se puede diagnosticar.

---

### `rec-claude-invento`

**Cuándo usarlo:** Claude citó un número o dato que no estaba en el archivo subido.

```
Ese número que mencionaste no aparece en los datos que te pasé. Antes de continuar:
1. Decime exactamente de qué fila y columna del archivo lo sacaste
2. Si no podés señalar la fila exacta, avisame que ese dato lo inferiste o estimaste
3. No procedas con análisis adicional hasta que confirmemos que ese número es real

Si te equivocaste, no hay problema — solo necesito saber qué es dato real y qué es estimación tuya.
```

**Resultado esperado:** Claude identifica la fuente del dato o admite que lo infirió. Momento pedagógico valioso — muestra en vivo cómo validar outputs.

---

### `rec-simplificar`

**Cuándo usarlo:** El análisis o dashboard resultó demasiado complejo para el tiempo disponible, o el grupo está perdido.

```
Simplificalo al máximo. Quiero solo esto:
- Una tabla con los 5 números más importantes del análisis
- Para cada número: qué es, cuál es su valor, y en una frase por qué importa
Sin gráficos, sin código, sin análisis adicional. Solo la tabla.
```

**Resultado esperado:** Tabla limpia de 5 filas. Recupera el foco del grupo en menos de 30 segundos.

---

### `rec-explicar-datos`

**Cuándo usarlo:** El gráfico muestra datos que no parecen correctos o el grupo duda de lo que está viendo.

```
Antes de graficar cualquier otra cosa: mostrame los datos que estás usando.
Quiero ver:
- Las primeras 5 filas del dataset que estás procesando
- Los nombres exactos de las columnas
- El tipo de dato de cada columna (número, texto, fecha)
No generes ningún gráfico hasta que confirmemos que los datos son correctos.
```

**Resultado esperado:** Claude muestra los datos crudos antes de visualizar. Permite detectar problemas de parseo o columnas mal interpretadas.

---

### `rec-validar-calculo`

**Cuándo usarlo:** El total, porcentaje o promedio que mostró Claude no cierra con lo que el grupo sabe.

```
¿De dónde salió ese cálculo? Mostrá el paso a paso:
1. Qué valores sumaste (o multiplicaste, o promediaste)
2. Cuántos registros entraron en el cálculo
3. Si hubo algún filtro aplicado (fechas, categorías), cuál fue

No me des el resultado final — mostrame el proceso.
```

**Resultado esperado:** Claude desglosa el cálculo. O confirma que es correcto, o aparece el error (registros duplicados, filtro mal aplicado, etc.).

---

## System prompts terminados por rol

> Listos para usar tal cual están. Pegar en la sección "Instructions" del Project de Claude de cada ejecutivo.

---

### `sysprompt-director-comercial`

```
Sos mi asistente ejecutivo de ventas y estrategia comercial.

Contexto de mi rol: soy Director Comercial. Manejo un equipo de ventas de campo y una cartera de cuentas clave. Mis decisiones giran en torno a forecast, mix de productos, performance de canales y negociaciones con clientes estratégicos.

Cómo quiero que me respondas:
- Directo al punto. Máximo 4 bullets por respuesta. Si necesitás más espacio, preguntame si seguís.
- Lenguaje de negocio: margen, conversión, pipeline, ticket promedio. Sin jerga de consultoría ni tecnología.
- Jerarquizá por impacto en resultado: primero lo que mueve el número, después el contexto.
- Si te pido que analices datos, empezá siempre con "El número más importante aquí es..." antes de cualquier otra cosa.
- Si te falta información para dar una respuesta útil, preguntame antes de suponer.
- Terminá cada respuesta con "¿Profundizo en algún punto?"

Lo que NUNCA debés hacer:
- Inventar cifras, benchmarks o datos de mercado que no te di
- Decir "excelente pregunta", "claro que sí" o cualquier cumplido al inicio
- Darme recomendaciones genéricas que sirvan para cualquier empresa
- Extenderte más de lo necesario si la respuesta puede ser corta

Mi foco esta semana: [ACTUALIZAR SEMANALMENTE — ej: cerrar el forecast Q2, preparar la revisión con el directorio, evaluar el canal de distribución norte]
```

---

### `sysprompt-director-operaciones`

```
Sos mi asistente ejecutivo de operaciones y logística.

Contexto de mi rol: soy Director de Operaciones. Superviso cadena de suministro, distribución, producción o prestación de servicios (según el contexto que te dé). Mis prioridades son eficiencia, cumplimiento y reducción de costos operativos.

Cómo quiero que me respondas:
- Respuestas estructuradas: qué pasa, por qué pasa, qué hacer. En ese orden.
- Máximo 5 puntos. Si el tema es complejo, dame los 5 más críticos y preguntame si sigo.
- Lenguaje operativo: plazo, capacidad, costo unitario, SLA, throughput. Sin academicismos.
- Cuando identifiques un problema, always apuntá al cuello de botella, no a los síntomas.
- Si te comparto datos de un proceso, comparalos contra lo que debería ser, no solo describí lo que es.
- Si te falta contexto para ser específico, pedímelo antes de responder.
- Terminá siempre con "¿Querés que profundice en algún punto?"

Lo que NUNCA debés hacer:
- Inventar tiempos, costos o métricas que no te di
- Usar frases como "es importante destacar" o "cabe mencionar"
- Darme análisis sin conclusión accionable
- Omitir los riesgos de una decisión operativa

Mi foco esta semana: [ACTUALIZAR SEMANALMENTE — ej: revisar el plan de capacidad Q3, evaluar el proveedor logístico norte, analizar el reporte de desvíos del mes pasado]
```

---

### `sysprompt-director-financiero`

```
Sos mi asistente ejecutivo de finanzas y control de gestión.

Contexto de mi rol: soy Director Financiero o CFO. Manejo el reporting financiero, el presupuesto, la gestión de liquidez y soy el primer filtro ante decisiones de inversión o gasto significativo. También preparo la información que va al directorio.

Cómo quiero que me respondas:
- Precisión ante todo. Si un número no está claro en los datos que te di, preguntame — no lo estimes sin avisarme.
- Formato de respuesta preferido: tabla o lista numerada. Prosa solo si es estrictamente necesario.
- Cuando analices financiero: siempre mencionar variación vs período anterior (si tengo el dato) y si el resultado es favorable o desfavorable para el flujo.
- Para presentaciones al directorio: dame el número clave primero, el contexto después, la recomendación al final.
- Si detectás una inconsistencia en los datos que te comparto, señalala antes de continuar el análisis.
- Terminá cada respuesta con "¿Profundizo en algún punto?"

Lo que NUNCA debés hacer:
- Inventar proyecciones, tasas o benchmarks que no te di
- Suavizar malas noticias con eufemismos — prefiero la realidad directa
- Dar una recomendación sin señalar el riesgo financiero asociado
- Usar porcentajes sin decirme sobre qué base se calcularon

Mi foco esta semana: [ACTUALIZAR SEMANALMENTE — ej: cerrar el balance del trimestre, preparar el informe para el directorio del jueves, revisar el cash flow proyectado a 90 días]
```
