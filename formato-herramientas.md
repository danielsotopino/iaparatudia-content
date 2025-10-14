# Formato para Herramientas de IA

## Estructura del archivo Markdown

### Frontmatter (YAML)
```yaml
---
title: "Nombre de la herramienta"
description: "Descripción breve de la herramienta"
logo: "/images/tools/nombre-logo.png"
website: "URL del sitio web"
category: "categoría-principal"
pricing: "tipo-de-precio"
difficulty: "nivel-de-dificultad"
tags: ["tag1", "tag2", "tag3"]
featured: false
publishDate: YYYY-MM-DD
roi_estimate: "estimación-de-roi"
languages: ["Idioma"]
---
```

### Estructura de headings

1. **H3 (`###`)**: Título principal con descripción breve
2. **H4 (`####`)**: Secciones principales:
   - ¿Qué hace exactamente?
   - Beneficios
   - Desventajas
   - Cuánto cuesta
   - Cuánto tiempo te ahorra
   - Cómo empezar (3 pasos)
   - ¿Para qué tipo de negocio sirve?

### Elementos incluidos

- **Imágenes**: Con sintaxis `![alt](/ruta/imagen)`
- **Listas**: Con viñetas (`-`) y numeradas (`1.`)
- **Texto destacado**: Con `**texto**`
- **Emojis**: ✅ para beneficios, ❌ para limitaciones
- **Comparaciones**: Formato "Antes vs Después"
- **Pasos numerados**: Para tutoriales
- **Categorización de negocios**: Con emojis de verificación

## Ejemplo de implementación

```markdown
---
title: "Canva AI"
description: "Crea diseños profesionales con inteligencia artificial"
logo: "/images/tools/canva-ai-logo.png"
website: "https://canva.com"
category: "marketing-digital"
pricing: "freemium"
difficulty: "principiante"
tags: ["Redes sociales", "Marketing", "Presentaciones"]
featured: false
publishDate: 2024-07-25
roi_estimate: "2-3 horas/día"
languages: ["Español"]
---

### Canva AI: Diseños profesionales sin ser diseñador

![Canva AI Interface](/images/tools/canva-ai-hero.jpg)

#### ¿Qué hace exactamente?
Descripción de la funcionalidad principal.

#### Beneficios
- Beneficio 1
- Beneficio 2
- Beneficio 3

#### Desventajas
- Limitación 1
- Limitación 2

#### Cuánto cuesta
- **Plan gratuito**: Características básicas
- **Plan premium**: Características completas

#### Cuánto tiempo te ahorra
**Antes**: Tiempo estimado sin la herramienta
**Con la herramienta**: Tiempo estimado con la herramienta

#### Cómo empezar (3 pasos)
1. Paso 1
2. Paso 2
3. Paso 3

#### ¿Para qué tipo de negocio sirve?
✅ Negocio tipo 1
✅ Negocio tipo 2
❌ Negocio no recomendado
```

## Notas importantes

- Mantener consistencia en el formato
- Usar imágenes relevantes y de alta calidad
- Incluir información práctica y accionable
- Estructurar la información de manera clara y fácil de navegar
- Usar emojis para mejorar la legibilidad
- Mantener un tono profesional pero accesible
