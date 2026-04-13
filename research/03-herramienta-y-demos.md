# Herramienta gratuita + Wow demos (Haiku brief)

> Recomendaciones concretas para la plataforma hands-on y los momentos "magia".

## 1. Herramienta primaria recomendada: **Claude (free tier)**

**Justificación**:

- **Sin fricción**: funciona en claude.ai con solo email — sin verificación por SMS (a diferencia de ChatGPT).
- **Custom instructions en free tier**: Claude permite system prompts explícitos; el usuario pega una persona y funciona. ChatGPT tiene custom instructions enterradas en settings.
- **Español nativo**: maneja modismos y tono en español mejor que Gemini free.
- **Defaults corporativos amigables**: controles de privacidad transparentes; funciona en browsers corporativos sin fricción de IT.
- **Límites aceptables**: ~40 mensajes por ventana de 5h — alcanza para 15–30 usuarios en 4h.
- **Extended thinking gratis**: añade un hook "wow" al mostrar razonamiento paso a paso.

> **Gotcha**: los límites se aprietan en horario pico PT (5–11am PT = ~9am–3pm Argentina). Probable que afecte el workshop. **Verificar el día del curso** y tener plan B (Gemini) como respaldo.

### Rechazados

| Herramienta | Motivo |
|---|---|
| **ChatGPT** | Verificación + custom instructions escondidas + cap de 10 msgs/5h en GPT-4o free |
| **Microsoft Copilot** | Update de abril 2026 removió Word/Excel/PowerPoint del free tier — solo chat web ahora |
| **Gemini** | Sin system prompts en chat free (solo en AI Studio, UX aparte) |
| **DeepSeek** | Chat web básico, sin custom instructions |
| **Le Chat (Mistral)** | No expone system prompts |

## 2. Qué expone system prompts en free tier

| Plataforma | System prompt free? | Cómo |
|---|---|---|
| **Claude** | ✅ | Al inicio de la conversación; persiste en ese thread; Projects lo consolida |
| **ChatGPT** | ✅ (enterrado) | Settings > Custom Instructions |
| **Gemini** | ⚠️ | Solo en AI Studio (sign-in separado) |
| **Copilot** | ❌ | No expuesto |
| **DeepSeek** | ❌ | API-only |
| **Le Chat** | ❌ | No feature nativa |

## 3. Wow demos cortas (<3' cada una)

1. **Resumir PDF de 20 páginas** → subir una política interna o informe, pedir 3 bullets. Pain point clásico de oficina.
2. **Hilo de emails → to-do list** → pegar 4–5 emails desordenados; extraer decisiones, preguntas abiertas, action items con responsables.
3. **Explicar fórmula de Excel** → tomar un `=SUMPRODUCT(IF(...))` feo y pedir explicación línea por línea. Toca *su* trabajo = magia.
4. **Extraer datos de screenshot** → foto de un formulario o tabla caótica → JSON/CSV.
5. **Traducir preservando tono** → email marketing cheeky EN → ES corporativo/casual/divertido. Side-by-side.
6. **Código a español** → pegar macro VBA, pedir explicación para alguien que no programa.

**Recomendación**: elegir 3, no más. Dos cortas + una que toque su dolor específico.

## 4. Demos "magia" largas (5–10')

### Opción A — Sitio de itinerario de viaje (eurotrip2026)

Alineada con el proyecto que el usuario ya tiene: **eurotrip2026.kodexarg.com**.

- Mostrar el sitio como producto terminado (30").
- Volver atrás: "esto se construyó en un fin de semana con AI como copiloto".
- Demo en vivo: pedirle a Claude un itinerario para un destino del público, tono específico, budget.
- Revelar la iteración: "hacelo más nightlife" → regenera.
- **Cierre conceptual**: no es que la AI haga todo — es que quien sabe qué pedir construye 10x más rápido.
- **Por qué funciona**: concreto, aspiracional, relatable, usa un artefacto real del instructor.

### Opción B — Estrategia de contenido para problema real del negocio

- Pegar un brief de lanzamiento.
- Pedir: thread de Twitter 30", blog 200 palabras, 3 FAQ.
- Iterar: "el blog más técnico" → regenera.
- **Por qué funciona**: ROI inmediato, aplicación directa al trabajo.

**Recomendación**: **Opción A** como headliner (ya existe, es del instructor, genera identificación). Opción B como backup si el público es muy corporativo/formal.

## 5. Gotchas 2025–2026

- **Claude**: solo Sonnet en free tier (no Opus). Fine para principiantes.
- **ChatGPT**: GPT-4o free cap 10 msgs/5h → usuarios pueden chocar el límite en una red compartida.
- **Copilot**: update de abril 2026 removió integración profunda con M365 del free tier.
- **Gemini**: no hay free API tier; solo web.
- **DeepSeek**: 5M tokens gratis one-time, web chat pelado.

**Shift clave 2026**: Copilot free ya no sirve para "AI en Word/Excel". Si el plan era bankear en eso, hay que replantear.

## 6. Checklist de setup

- Herramienta primaria: **Claude** en claude.ai
- Backup: **Gemini** en gemini.google.com
- Prep de demos:
  - Pre-cargar PDFs de muestra, emails, screenshots
  - Testear custom instructions en Claude **antes** del workshop
  - Tener 5–6 prompts pre-escritos (copy-paste, no improvisar — consistencia con 15–30 personas)
- Español: nativo, sin modo separado
- IT corporativo: sin instalaciones, sin VPN, cualquier browser moderno

## Fuentes

- chatgpt.com/pricing
- freeacademy.ai/blog/claude-free-plan-limits-2026
- simplysharepoint.com — Microsoft 365 Copilot April 2026 changes
- mydeepseekapi.com — DeepSeek free tier
- spliiit.com — alternativas gratuitas a ChatGPT
