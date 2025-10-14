# METADATA.md - Documentación de Campos de Frontmatter

**Última actualización**: 2025-10-13
**Versión**: 1.0

---

## 📋 Resumen

Este documento describe todos los campos permitidos en el frontmatter de archivos markdown de iaparatudia.

---

## 🔧 CAMPOS POR TIPO DE CONTENIDO

### Tabla Comparativa

| Campo | Herramientas | Noticias | Tutoriales | Tipo | Obligatorio |
|-------|--------------|----------|------------|------|-------------|
| `title` | ✅ | ✅ | ✅ | String | Sí |
| `description` | ✅ | ✅ | ✅ | String | Sí |
| `publishDate` | ✅ | ✅ | ✅ | Date (YYYY-MM-DD) | Sí |
| `tags` | ✅ | ✅ | ✅ | Array[String] | Sí |
| `category` | ✅ | ✅ | ✅ | String | Sí |
| `featured` | ✅ | ✅ | ✅ | Boolean | Sí |
| `logo` | ✅ | ❌ | ❌ | String (path) | Sí |
| `website` | ✅ | ❌ | ❌ | String (URL) | Sí |
| `pricing` | ✅ | ❌ | ❌ | String | Sí |
| `difficulty` | ✅ | ❌ | ✅ | String | Sí |
| `roi_estimate` | ✅ | ❌ | ❌ | String | Sí |
| `languages` | ✅ | ❌ | ❌ | Array[String] | Sí |
| `author` | ❌ | ✅ | ❌ | String | Sí |
| `image` | ❌ | ✅ | ❌ | String (path) | Sí |
| `readTime` | ❌ | ✅ | ❌ | String | Sí |
| `impact` | ❌ | ✅ | ❌ | String | Sí |
| `duration` | ❌ | ❌ | ✅ | String | Sí |
| `tools_needed` | ❌ | ❌ | ✅ | Array[String] | Sí |
| `outcome` | ❌ | ❌ | ✅ | String | Sí |
| `materials` | ❌ | ❌ | ✅ | Array[String] | No |
| `steps` | ❌ | ❌ | ✅ | Number | Sí |

---

## 📝 DESCRIPCIÓN DETALLADA DE CAMPOS

### Campos Comunes (Todos los Tipos)

#### `title`
- **Tipo**: String
- **Obligatorio**: Sí
- **Descripción**: Título principal del contenido
- **Longitud**:
  - Herramientas: 30-60 caracteres
  - Noticias: 60-80 caracteres
  - Tutoriales: 40-70 caracteres
- **Formato**: Title Case o Sentence case
- **Ejemplo**: `"HubSpot CRM con IA"`

#### `description`
- **Tipo**: String
- **Obligatorio**: Sí
- **Descripción**: Descripción breve para SEO y previews
- **Longitud**:
  - Herramientas: 100-120 caracteres
  - Noticias: 150-160 caracteres
  - Tutoriales: 60-100 caracteres
- **Ejemplo**: `"Gestiona clientes y ventas con inteligencia artificial integrada"`

#### `publishDate`
- **Tipo**: Date
- **Obligatorio**: Sí
- **Formato**: `YYYY-MM-DD` (ISO 8601)
- **Ejemplo**: `2025-01-20`
- **Nota**: Fecha de publicación en el sitio, NO fecha de creación del archivo

#### `tags`
- **Tipo**: Array de Strings
- **Obligatorio**: Sí
- **Cantidad**: 3-6 tags
- **Formato**: Title Case, separados por espacios
- **Ejemplo**: `["CRM", "Ventas", "Automatización"]`
- **Referencia**: Ver `docs/TAGS.md`

#### `category`
- **Tipo**: String (enum)
- **Obligatorio**: Sí
- **Formato**: minúsculas-con-guiones
- **Ejemplo**: `"marketing-digital"`
- **Referencia**: Ver `docs/CATEGORIES.md`

#### `featured`
- **Tipo**: Boolean
- **Obligatorio**: Sí
- **Valores**: `true` | `false`
- **Default**: `false`
- **Ejemplo**: `false`
- **Nota**: Usar `true` solo para contenido destacado (máximo 3-5 simultáneos)

---

### Campos Específicos: HERRAMIENTAS

#### `logo`
- **Tipo**: String (path)
- **Obligatorio**: Sí
- **Formato**: `/images/tools/[slug]-logo.[ext]`
- **Extensiones**: `.png`, `.jpg`, `.svg`, `.ico`
- **Ejemplo**: `"/images/tools/hubspot-crm-logo.png"`
- **Nota**: El archivo DEBE existir en el directorio

#### `website`
- **Tipo**: String (URL)
- **Obligatorio**: Sí
- **Formato**: URL completa con `https://`
- **Ejemplo**: `"https://hubspot.com"`

#### `pricing`
- **Tipo**: String (enum)
- **Obligatorio**: Sí
- **Valores**: `"gratis"` | `"freemium"` | `"pago"`
- **Definiciones**:
  - `gratis`: Completamente gratuito
  - `freemium`: Plan gratuito + planes de pago
  - `pago`: Solo planes de pago
- **Ejemplo**: `"freemium"`

#### `difficulty`
- **Tipo**: String (enum)
- **Obligatorio**: Sí (Herramientas y Tutoriales)
- **Valores**: `"principiante"` | `"intermedio"` | `"avanzado"`
- **Definiciones**:
  - `principiante`: Sin conocimientos técnicos requeridos
  - `intermedio`: Familiaridad con herramientas digitales
  - `avanzado`: Conocimientos técnicos o especialización
- **Ejemplo**: `"intermedio"`

#### `roi_estimate`
- **Tipo**: String
- **Obligatorio**: Sí
- **Formato**: `"X-Y horas/semana"`
- **Ejemplo**: `"4-5 horas/semana"`
- **Nota**: SIEMPRE usar "horas/semana" para consistencia

#### `languages`
- **Tipo**: Array de Strings
- **Obligatorio**: Sí
- **Valores**: Nombres de idiomas en español
- **Ejemplo**: `["Español", "Inglés", "Portugués"]`
- **Orden**: Por relevancia para el público objetivo

---

### Campos Específicos: NOTICIAS

#### `author`
- **Tipo**: String
- **Obligatorio**: Sí
- **Default**: `"IA para tu día"`
- **Ejemplo**: `"IA para tu día"`
- **Nota**: Cambiar solo si hay autor específico

#### `image`
- **Tipo**: String (path)
- **Obligatorio**: Sí
- **Formato**: `/images/news/YYYY-MM-DD-slug.jpg`
- **Ejemplo**: `"/images/news/2025-01-20-claude-nuevo-modelo.jpg"`
- **Nota**: Debe coincidir con el nombre del archivo markdown

#### `readTime`
- **Tipo**: String
- **Obligatorio**: Sí
- **Formato**: `"X min"`
- **Cálculo**: ~200-250 palabras = 1 minuto
- **Ejemplo**: `"3 min"`

#### `impact`
- **Tipo**: String (enum)
- **Obligatorio**: Sí
- **Valores**: `"alto"` | `"medio"` | `"bajo"`
- **Definiciones**:
  - `alto`: Cambios significativos, afecta a muchos negocios
  - `medio`: Actualizaciones importantes, tendencias consolidadas
  - `bajo`: Noticias menores, consejos específicos
- **Ejemplo**: `"alto"`

---

### Campos Específicos: TUTORIALES

#### `duration`
- **Tipo**: String
- **Obligatorio**: Sí
- **Formato**: `"X minutos"` o `"X-Y minutos"`
- **Ejemplo**: `"5 minutos"` o `"10-15 minutos"`
- **Nota**: Incluir tiempo de lectura + ejecución

#### `tools_needed`
- **Tipo**: Array de Strings
- **Obligatorio**: Sí
- **Descripción**: Lista de herramientas requeridas
- **Ejemplo**: `["WhatsApp Business", "Smartphone"]`
- **Nota**: Mencionar si son gratuitas o de pago en el contenido

#### `outcome`
- **Tipo**: String
- **Obligatorio**: Sí
- **Descripción**: Resultado específico que logrará el usuario
- **Ejemplo**: `"Responder 80% de consultas automáticamente"`
- **Nota**: Debe ser medible si es posible

#### `materials`
- **Tipo**: Array de Strings (paths)
- **Obligatorio**: No (opcional)
- **Formato**: `["/downloads/nombre-archivo.pdf"]`
- **Ejemplo**: `["/downloads/plantillas-whatsapp.pdf"]`
- **Default**: `[]` (array vacío)

#### `steps`
- **Tipo**: Number
- **Obligatorio**: Sí
- **Descripción**: Número de pasos principales del tutorial
- **Ejemplo**: `4`
- **Nota**: Debe coincidir con las secciones "Paso X" en el contenido

---

## 🔍 VALIDACIÓN

### Reglas Generales
1. Todos los campos obligatorios DEBEN estar presentes
2. Tipos de datos deben coincidir exactamente
3. Valores enum deben ser exactos (case-sensitive)
4. Fechas en formato ISO (YYYY-MM-DD)
5. URLs completas con protocolo
6. Paths de imágenes deben existir

### Ejemplo de Validación con Zod (usado en web)
```typescript
// src/content/config.ts
import { z, defineCollection } from 'astro:content';

const toolsCollection = defineCollection({
  schema: z.object({
    title: z.string(),
    description: z.string().max(120),
    logo: z.string(),
    website: z.string().url(),
    category: z.enum(['productividad', 'marketing-digital', ...]),
    pricing: z.enum(['gratis', 'freemium', 'pago']),
    difficulty: z.enum(['principiante', 'intermedio', 'avanzado']),
    tags: z.array(z.string()).min(3).max(6),
    featured: z.boolean(),
    publishDate: z.date(),
    roi_estimate: z.string(),
    languages: z.array(z.string()),
  }),
});
```

---

## 📋 EJEMPLOS COMPLETOS

### Herramienta
```yaml
---
title: "HubSpot CRM con IA"
description: "Gestiona clientes y ventas con inteligencia artificial integrada"
logo: "/images/tools/hubspot-crm-logo.png"
website: "https://hubspot.com"
category: "ventas"
pricing: "freemium"
difficulty: "intermedio"
tags: ["CRM", "Ventas", "Automatización"]
featured: true
publishDate: 2024-07-25
roi_estimate: "4-5 horas/semana"
languages: ["Español", "Inglés"]
---
```

### Noticia
```yaml
---
title: "Claude 4 llega con nuevas capacidades para pequeños negocios"
description: "El nuevo modelo de IA de Anthropic promete revolucionar la atención al cliente con análisis contextual mejorado"
publishDate: 2025-01-20
author: "IA para tu día"
tags: ["Claude", "Anthropic", "IA", "Atención al Cliente"]
featured: false
image: "/images/news/2025-01-20-claude-nuevo-modelo.jpg"
readTime: "3 min"
impact: "alto"
category: "tecnologia-ia"
---
```

### Tutorial
```yaml
---
title: "Automatizar respuestas de WhatsApp Business en 5 minutos"
description: "Configura mensajes automáticos para atender clientes 24/7"
duration: "5 minutos"
difficulty: "principiante"
tools_needed: ["WhatsApp Business", "Smartphone"]
publishDate: 2025-01-20
category: "atencion-cliente"
outcome: "Responder 80% de consultas automáticamente"
materials: ["/downloads/plantillas-whatsapp.pdf"]
steps: 4
tags: ["WhatsApp Business", "Automatización", "Atención al Cliente"]
featured: false
---
```

---

## 🚨 Errores Comunes

1. **Fechas incorrectas**: `2025/01/20` ❌ → `2025-01-20` ✅
2. **URLs sin protocolo**: `hubspot.com` ❌ → `https://hubspot.com` ✅
3. **Tags con guiones**: `["atencion-cliente"]` ❌ → `["Atención al Cliente"]` ✅
4. **Enums en mayúsculas**: `pricing: "FREEMIUM"` ❌ → `pricing: "freemium"` ✅
5. **ROI sin unidad**: `"4-5 horas"` ❌ → `"4-5 horas/semana"` ✅
6. **Campos faltantes**: Omitir campo obligatorio
7. **Rutas de imágenes incorrectas**: `/images/tools/` ❌ → `/images/tools/` ✅

---

**Mantenido por**: Equipo editorial iaparatudia
**Revisión**: Trimestral
**Última revisión**: 2025-10-13
