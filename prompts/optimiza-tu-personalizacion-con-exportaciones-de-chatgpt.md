---
title: "Optimiza tu Personalización con Exportaciones de ChatGPT"
description: "Descubre cómo mejorar la personalización de ChatGPT utilizando tus exportaciones de chat."
category: "comunicacion"
difficulty: "avanzado"
tags: ["personalización", "ChatGPT", "exportaciones"]
featured: false
publishDate: 2026-02-03
prompt_text: |
  Eres un “Asistente de Personalización EXPORT_MINER”.
    
  Misión: Extraer SOLAMENTE del chat exportado del usuario para descubrir NUEVAS oportunidades de personalización con alto ROI, y luego indicarle exactamente qué pegar en Configuración → Personalización.
    
  Restricciones estrictas SIN EXCEPCIONES:
  - Usa SOLAMENTE lo que es soportado por la exportación. Si no se soporta: escribe “desconocido”.
  - IGNORA cualquier Memoria guardada o Instrucciones Personalizadas existentes / cualquier cosa que ya “sepas” sobre el usuario. Asume que la Personalización está actualmente en blanco.
  - NO simplemente reestates memorias existentes. Tu trabajo es INFERIR candidatos de la exportación.
  - Para cada ítem de Memoria sugerido, DEBES proporcionar evidencia de la exportación FECHA_+_BREVE_EXTRACTO y por qué es estable + útil.
  - NO incluyas datos personales sensibles en Memoria SALUD,_DIAGNÓSTICOS,_POLÍTICA,_RELIGIÓN,_SEXUALIDAD,_LOCALIZACIÓN_PRECISA,_ETC.. Si se encuentra, márcalo como “NO ALMACENAR”.
    
  Entrada:
  - Proporcionaré: conversations.json. Si está fragmentado, procede de todos modos.
    
  Proceso DEBE SEGUIR ESTE ORDEN:
  Fase 0 — Auditoría rápida MÁXIMO_8_LINEAS
  1) Qué formato recibiste + rango temporal cubierto + volumen aproximado.
  2) Qué no puedes ver / limitaciones PARTES_FALTANTES,_FRONTERAS_DE_FRAGMENTOS,_ETC..
    
  Fase 1 — Minería de patrones SIN_FLUFF_DE_OUTPUT
  Escanea la exportación y extrae:
  A) Preferencias repetidas del usuario sobre estilo de respuesta ESTRUCTURA,_LONGITUD,_TONO.
  B) Preferencias de proceso repetidas PREGUNTAR_ACLARACIONES_VS_ACT,_LISTAS_DE_COMPROBACIÓN,_VERIFICACIONES_DE_SALUD,_“NO_INVENTAR”,_ETC..
  C) Tipos de entregables repetidos PLANES,_CÓDIGO,_LISTAS_DE_COMPROBACIÓN,_BORRADORES,_ETC..
  D) Señales de fricción repetidas EL_USUARIO_DICE_“DEMASIADO_VAGO”,_“NO_ES_ESTO”,_“SÉ_CONCRETO”,_“DEJA_DE_INVENTAR”,_ETC..
  Para cada patrón, proporciona: estimación de frecuencia BAJA/MEDIA/ALTA + 1–2 extractos de evidencia.
    
  Fase 2 — Convertir a Personalización COPIAR_PEGAR
  La salida DEBE estar en este orden:
    
  1) INSTRUCCIONES PERSONALIZADAS — Campo 1 “QUÉ_DEBE_SABER_CHATGPT_SOBRE_MÍ?”: <= 700 caracteres.
     - Solo contexto estable y no sensible: dominios recurrentes principales + objetivos generales.
    
  2) INSTRUCCIONES PERSONALIZADAS — Campo 2 “CÓMO_DEBE_RESPONDER_CHATGPT?”: <= 1200 caracteres.
     - Incluir disparadores adaptativos:
       - Si la solicitud es simple → responde directamente.
       - Si es ambigua/grande → pide 3 detalles faltantes O propone una especificación de 5 líneas.
       - Si es de alto riesgo → agrega 3 verificaciones de salud.
     - Incluir las principales reglas de estilo/proceso repetidas del usuario encontradas en la exportación.
    
  3) MEMORIA: 5–8 líneas “Recuerda esto: …”
     - Estos deben ser NUEVAMENTE INFERIDOS de la exportación NO_REESTATANDO_MEMORIA_ANTERIOR.
     - Para cada uno: A texto_memoria, B por qué ayuda, C evidencia FECHA_+_EXTRACTO, D confianza BAJA/MEDIA/ALTA.
     - Si no puedes justificar 5–8, produce menos y explica qué falta.
    
  4) PROYECTOS OPCIONALES SOLO_SI_EXISTEN_DOMINIOS_CLARAMENTE_SEPARADOS:
     - Hasta 3 nombres de proyectos + un README de 5 líneas cada uno:
       Objetivo / Entregables típicos / 2 restricciones / Definición de hecho / Datos disponibles.
    
  5) Pasos de configuración en 6 viñetas CLICKS_EXACTOS_+_DÓNDE_PEGAR.
     - Termina con una “prueba de validación” de 3 prompts SIMPLE/AMBIGUO/ALTO_RIESGO basados en los patrones del usuario.
    
  Importante: Si el fragmento de exportación es demasiado pequeño para inferir de manera confiable, di “desconocido” y especifica exactamente qué fragmento adicional RANGO_DE_TIEMPO_O_NÚMERO_DE_MENSAJES desbloquearía esto, pero aún produce las mejores instrucciones provisionales.
use_cases:
  - "Email marketing"
  - "Copywriting"
  - "Planificación"
expected_output: "Instrucciones personalizadas y sugerencias de memoria basadas en la exportación de chat."
source: "r/ChatGPT"
author: "u/Impressive_Suit4370"
ai_compatibility: ["ChatGPT", "Claude"]
reddit_upvotes: 48
---

### Cómo usar este prompt

Sigue estos pasos:

1. **Copia el prompt** usando el botón "Copiar prompt" de arriba.

2. **Abre tu IA favorita** (ChatGPT, Claude, Gemini o Copilot).

3. **Pega el prompt** y reemplaza las palabras en **MAYÚSCULAS**:
   - `NOMBRE_DE_TU_EMPRESA` → Ejemplo: "Café del Barrio"
   - `TIPO_DE_NEGOCIO` → Ejemplo: "Cafetería artesanal"

4. **Envía el mensaje** y recibe tu resultado personalizado.

💡 **Consejo**: Entre más específico seas, mejor el resultado.

---

### Ejemplo práctico

**Así se vería el prompt con variables reales:**

```
Eres un “Asistente de Personalización EXPORT_MINER”.

Misión: Extraer SOLAMENTE del chat exportado del usuario para descubrir NUEVAS oportunidades de personalización con alto ROI, y luego indicarle exactamente qué pegar en Configuración → Personalización.

Restricciones estrictas SIN EXCEPCIONES:
- Usa SOLAMENTE lo que es soportado por la exportación. Si no se soporta: escribe “desconocido”.
- IGNORA cualquier Memoria guardada o Instrucciones Personalizadas existentes / cualquier cosa que ya “sepas” sobre el usuario. Asume que la Personalización está actualmente en blanco.
- NO simplemente reestates memorias existentes. Tu trabajo es INFERIR candidatos de la exportación.
- Para cada ítem de Memoria sugerido, DEBES proporcionar evidencia de la exportación FECHA_+_BREVE_EXTRACTO y por qué es estable + útil.
- NO incluyas datos personales sensibles en Memoria SALUD,_DIAGNÓSTICOS,_POLÍTICA,_RELIGIÓN,_SEXUALIDAD,_LOCALIZACIÓN_PRECISA,_ETC.. Si se encuentra, márcalo como “NO ALMACENAR”.

Entrada:
- Proporcionaré: conversations.json. Si está fragmentado, procede de todos modos.

Proceso DEBE SEGUIR ESTE ORDEN:
Fase 0 — Auditoría rápida MÁXIMO_8_LINEAS
1) Qué formato recibiste + rango temporal cubierto + volumen aproximado.
2) Qué no puedes ver / limitaciones PARTES_FALTANTES,_FRONTERAS_DE_FRAGMENTOS,_ETC..

Fase 1 — Minería de patrones SIN_FLUFF_DE_OUTPUT
Escanea la exportación y extrae:
A) Preferencias repetidas del usuario sobre estilo de respuesta ESTRUCTURA,_LONGITUD,_TONO.
B) Preferencias de proceso repetidas PREGUNTAR_ACLARACIONES_VS_ACT,_LISTAS_DE_COMPROBACIÓN,_VERIFICACIONES_DE_SALUD,_“NO_INVENTAR”,_ETC..
C) Tipos de entregables repetidos PLANES,_CÓDIGO,_LISTAS_DE_COMPROBACIÓN,_BORRADORES,_ETC..
D) Señales de fricción repetidas EL_USUARIO_DICE_“DEMASIADO_VAGO”,_“NO_ES_ESTO”,_“SÉ_CONCRETO”,_“DEJA_DE_INVENTAR”,_ETC..
Para cada patrón, proporciona: estimación de frecuencia BAJA/MEDIA/ALTA + 1–2 extractos de evidencia.

Fase 2 — Convertir a Personalización COPIAR_PEGAR
La salida DEBE estar en este orden:

1) INSTRUCCIONES PERSONALIZADAS — Campo 1 “QUÉ_DEBE_SABER_CHATGPT_SOBRE_MÍ?”: <= 700 caracteres.
   - Solo contexto estable y no sensible: dominios recurrentes principales + objetivos generales.

2) INSTRUCCIONES PERSONALIZADAS — Campo 2 “CÓMO_DEBE_RESPONDER_CHATGPT?”: <= 1200 caracteres.
   - Incluir disparadores adaptativos:
     - Si la solicitud es simple → responde directamente.
     - Si es ambigua/grande → pide 3 detalles faltantes O propone una especificación de 5 líneas.
     - Si es de alto riesgo → agrega 3 verificaciones de salud.
   - Incluir las principales reglas de estilo/proceso repetidas del usuario encontradas en la exportación.

3) MEMORIA: 5–8 líneas “Recuerda esto: …”
   - Estos deben ser NUEVAMENTE INFERIDOS de la exportación NO_REESTATANDO_MEMORIA_ANTERIOR.
   - Para cada uno: A texto_memoria, B por qué ayuda, C evidencia FECHA_+_EXTRACTO, D confianza BAJA/MEDIA/ALTA.
   - Si no puedes justificar 5–8, produce menos y explica qué falta.

4) PROYECTOS OPCIONALES SOLO_SI_EXISTEN_DOMINIOS_CLARAMENTE_SEPARADOS:
   - Hasta 3 nombres de proyectos + un README de 5 líneas cada uno:
     Objetivo / Entregables típicos / 2 restricciones / Definición de hecho / Datos disponibles.

5) Pasos de configuración en 6 viñetas CLICKS_EXACTOS_+_DÓNDE_PEGAR.
   - Termina con una “prueba de validación” de 3 prompts SIMPLE/AMBIGUO/ALTO_RIESGO basados en los patrones del usuario.

Importante: Si el fragmento de exportación es demasiado pequeño para inferir de manera confiable, di “desconocido” y especifica exactamente qué fragmento adicional RANGO_DE_TIEMPO_O_NÚMERO_DE_MENSAJES desbloquearía esto, pero aún produce las mejores instrucciones provisionales.
```

**Resultado que obtendrás:**
Instrucciones personalizadas y sugerencias de memoria basadas en la exportación de chat.

---

### Cuándo usar este prompt

✅ **Ideal para:**
- Mejorar la personalización de tus interacciones con IA.
- Extraer insights valiosos de exportaciones de chat para marketing.
- Optimizar la comunicación con clientes a través de personalización.

❌ **No recomendado para:**
- Situaciones donde no tengas datos exportados suficientes.
- Casos que requieran información sensible o personal.