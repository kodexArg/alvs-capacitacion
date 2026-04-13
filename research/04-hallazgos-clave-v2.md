# Hallazgos clave — Ronda 2 de investigación

> Consolidado de 4 briefs Haiku con foco específico en: ejecutivos + Excel + Claude Desktop + abril 2026.

---

## 🚨 Alertas críticas para mañana

### Copilot con tenant corporativo — SÍ va
- **15-abril-2026**: Microsoft cortó el *free tier* de Copilot con integración nativa en Word/Excel/PowerPoint. Pero con **licencia paga vía tenant** la integración está completa y es la más profunda del mercado: vive adentro del archivo donde los datos ya están.
- El instructor tiene tenant admin y puede asignar licencias en un click → Copilot vuelve al tour como **segunda herramienta recomendada**.
- **Posicionamiento estratégico**: dos herramientas, dos lenguajes.
  - **Claude Desktop** → análisis profundo, dashboards con Artifacts, privacidad por default, archivos fuera del tenant.
  - **Copilot M365** → Excel / Word / Outlook de todos los días, adentro del archivo, datos nunca salen del tenant.
- **Demo con Copilot en vivo**: abrir un Excel en Excel (no subir a Claude), panel lateral de Copilot, un prompt ejecutivo. 2 minutos y muestra un ángulo que Claude no tiene: "ya vive acá dentro".

### ChatGPT free ahora con ads (feb 2026)
- Mencionar brevemente. No demostrar sin cuenta paga si se puede evitar.

### Free tier Claude usa Haiku 4.5
- El modelo por default en free es **Haiku 4.5**, no Sonnet/Opus.
- Igual funciona para la demo: Haiku 4.5 soporta Artifacts, file upload, XLSX nativo.
- Si el instructor tiene cuenta Pro personal, usarla para mayor velocidad y mejor calidad en razonamiento.

---

## Excel + Claude: lo que realmente funciona

### Formatos
- **CSV**: parseo instantáneo, nunca falla.
- **XLSX**: soporte nativo desde fines de 2025. Múltiples hojas OK si "Analysis Tool" está activado.
- **Macros/VBA, formato condicional, formulas**: **Claude solo ve el valor calculado, NO la fórmula**. Importante saber esto antes de demoar "explicá esta fórmula" con un archivo subido (no funciona — hay que pegar la fórmula como texto).

### Límites
- Hasta 30MB por archivo, 20 archivos por chat.
- <10MB: rápido y fluido.
- 10–50MB: funciona pero más lento.
- > 50MB: riesgo de overflow. Simplificar.

### Regla de oro
> **Excel limpio, sin macros, sin referencias externas, con encabezados claros** → funciona perfecto. Un Excel "de producción" con pivots + fórmulas + hojas enlazadas → impredecible. **Preparar una versión simplificada del archivo real antes del workshop**.

---

## Artifacts para dashboards — la jugada ganadora

### Qué son
Bloques de código que Claude renderiza en vivo al lado del chat. Soportan HTML, React, SVG, Markdown, Mermaid. Dashboards interactivos con Recharts (gráficos) + Tailwind (estilos) + React state (filtros).

### Tiempo de render
- Artifact promedio: 10–20 segundos.
- El momento de revelación cuando aparece → alto impacto visual.

### Prompt canónico para dashboard ejecutivo
```
Generá un dashboard interactivo HTML con los datos del Excel que acabo de subir.
Quiero:
1. Tarjetas (KPI cards) con: ingresos totales, margen promedio, mejor mes
2. Gráfico de barras con ingresos por mes
3. Gráfico de torta con distribución por categoría
4. Filtro desplegable para ver solo una región
Paleta: azul/gris corporativo. Usá Recharts y Tailwind. Que se vea profesional, no de tutorial.
```

### Fallas típicas + recuperación
| Falla | Señal | Fix |
|---|---|---|
| Artifact en blanco | React con error silencioso | "El gráfico no se renderizó, agregá manejo de errores y regeneralo" |
| Gráfico sin datos | JSON mal parseado | "Mostrame los datos que estás usando antes de graficar" |
| CORS error | Intentó llamada externa | Normal, recordar que artifacts son offline |
| Rate limit | Mensaje explícito | Plan B: tener 2 cuentas, o pivot a "hagamos un resumen en tabla" |

### Checklist pre-demo (obligatorio una hora antes)
1. Subir el Excel real a Claude web con la cuenta que se usará en vivo
2. Ejecutar el prompt canónico → verificar que el dashboard renderiza
3. Probar iteración en vivo ("cambialo a línea, poné colores verde y gris")
4. Desactivar ad blockers del navegador
5. Captura de pantalla del artifact funcionando como backup

---

## Pedagogía para ejecutivos — lo diferente

### El problema "¿y a mí qué?"
Ejecutivos no preguntan "¿cómo funciona?" — preguntan **"¿qué decisión me cambia esto esta semana?"**. Cada concepto debe anclarse a una decisión real.

> "El CFO ya no revisa planillas. Interpreta lo que la AI marcó como anómalo. ¿Tenés gente entrenada para eso?" — McKinsey 2026

### Credibilidad del instructor no-profesor
- **Decirlo frontal**: *"No soy capacitador, soy su jefe de sistemas. Vamos a resolver esto juntos."* → más creíble que aparentar dominio didáctico.
- **Admitir incertidumbre**: *"Esto alucinó el 40% de las veces en mis tests. ¿Qué harían ustedes con datos de clientes?"*
- **Devolver preguntas**: cuando alguien cuestiona, contestar *"Esa es la pregunta que va a hacer el directorio. ¿Cómo la contestarían ustedes?"*

### Apertura de 3 minutos — patrón probado
**No**: slide de bienvenida, agenda, objetivos de aprendizaje.
**Sí**: demo en vivo que falla. Pedir a ChatGPT un comunicado de prensa sobre la empresa → dejar que alucine datos → *"¿Quién de ustedes detecta eso antes de que llegue al directorio? Ese es el trabajo ahora"*.

### Formato socrático confirmado
Evidencia de MIT Sloan, Deloitte, BCG: dejar que el ejecutivo dirija el demo (dicta qué preguntar, cómo reformular) triplica confianza vs. presentación canned. **El instructor es el operador, ellos son los autores intelectuales**.

---

## Manual de objeciones ejecutivas (respuestas rápidas)

| Objeción | Respuesta |
|---|---|
| "Alucina" | "Sí. Por eso no lo usás para decisiones binarias de verdad/mentira. Lo usás para redactar, para idear, para marcar outliers que un humano valida. Como Excel: no decide el presupuesto, solo muestra candidatos." |
| "Es una caja negra" | "La transparencia es un horizonte de riesgo, no el problema de hoy. Deployamos con guardrails: workflows de aprobación, auditoría de outputs, firma humana. Mismo estándar que cualquier herramienta de alto impacto." |
| "Mis datos son confidenciales" | "Separás datos de la herramienta. Anonimizás o resumís antes. Usás modelos on-premise para lo sensible. Pero pregunta inversa: ¿prohibimos Excel con datos de clientes, o ingenieriamos controles?" |
| "Va a reemplazar gente" | "McKinsey 2026: AI automatiza 57% de *tareas*, no puestos. Los puestos se corren de ejecución a juicio. Tu trabajo no es cargar datos, es decidir qué significan. Esto fuerza upskilling, no recorte." |
| "Es hype" | "Puede ser. Pero los competidores no están esperando para averiguarlo. Si nos equivocamos: 4 horas y unos dólares de API. Si estamos en lo cierto y llegamos tarde: problema de directorio." |

---

## Recovery lines para demos en vivo

| Situación | Línea (castellano) |
|---|---|
| Claude inventa un número | "Fíjense que Claude inventó ese número. No estaba en los datos que pasé. Regla de oro: si no está en los datos que vimos, no es confiable." |
| Artifact no renderiza | "A veces el browser no carga el código. Dejame regenerarlo." → copiar código en tab nueva. |
| Rate limit | "Claude pide un respiro. Pasa con tráfico pico. En producción tu empresa tendría acceso dedicado." |
| WiFi lento | "WiFi se vuelve loco con tráfico compartido. En el mundo real va con tu laptop + API key, no depende de esto." |
| Prompt ejecutivo muy vago | "¿Te referís a X o a Y? Necesito hacerlo concreto para que Claude dé una respuesta útil." |
| Prompt ejecutivo muy específico sin datos | "Claude solo ve los datos que le pasamos. ¿Tenés el dato, o lo estimamos con benchmarks del sector?" |

---

## Privacidad por default (comparativo para ejecutivos)

| Herramienta | Entrena con tus datos por default? |
|---|---|
| **Claude** | ❌ NO (GDPR-friendly, privacidad on por default) |
| **Mistral Le Chat** | ❌ NO (europeo, privacy-first) |
| **ChatGPT free** | ✅ SÍ — hay que desactivar en Settings → Data Controls |
| **Gemini free** | ✅ SÍ — hay que desactivar en Settings → Privacy |
| **Copilot M365 (licencia paga)** | ❌ NO entrena con tus datos empresariales (tenant aislado). Es una de las mejores opciones para datos sensibles. |
| **DeepSeek** | Ambiguo (no declaración oficial clara) |

**Mensaje para los 4 jefes**: *"Si van a subir un archivo de la empresa, hoy, sin cambiar nada, la opción más segura es Claude. Es el que viene con privacidad prendida por default"*.

---

## Outcomes medibles al terminar las 4 horas

Al salir del workshop, cada jefe debería poder:

1. **Articular un caso de uso concreto en su área** ("en mi equipo, esto lo usaría para...")
2. **Identificar una pregunta de gobernanza** para la próxima reunión de directorio
3. **Haber visto en vivo** una alucinación y una recuperación
4. **Explicar a su equipo** por qué vale la pena probarlo (cadena de credibilidad)
5. **Definir un piloto de 90 días** acotado con criterio go/no-go

---

## Fuentes consolidadas

- Anthropic Help Center — Create/edit files, Use Claude for Excel
- MIT Sloan — AI Literacy for Executives
- McKinsey — The AI Reckoning / Superagency in the Workplace
- HBR 2026-01 — How Executives Are Thinking About AI
- Deloitte AI Forum 2025
- Gartner — Future of Leadership with AI
- Anthropic platform docs — Reduce hallucinations
- tech-insider.org — ChatGPT vs Claude vs Gemini vs DeepSeek 2026
- simplysharepoint.com — Copilot April 2026 changes
