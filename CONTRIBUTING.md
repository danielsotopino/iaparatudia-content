# Cómo Crear una Noticia para @iaparatudia

Este documento explica cómo crear y estructurar una noticia para el sitio web de IA para tu día.

## Estructura de una Noticia

Las noticias se crean como archivos Markdown (`.md`) en el directorio `news/`.

Cada noticia debe seguir esta estructura:

### 1. Encabezado YAML (Front Matter)

Al comienzo del archivo, incluye un bloque YAML con la siguiente información:

```yaml
---
title: "Título de la noticia"
description: "Breve descripción (150-160 caracteres)"
publishDate: YYYY-MM-DD (Fecha de publicación en formato ISO)
author: "IA para tu día" (O el nombre del autor real si aplica)
tags: ["tag1", "tag2", "tag3"] (3-6 tags relevantes)
featured: false (true si es una noticia destacada)
readTime: "X min" (Estimación del tiempo de lectura)
impact: "alto" (impacto de la noticia: "alto", "medio", "bajo")
category: "categoria" (Categoría principal, ej: "tecnologia-ia", "marketing", "atencion-cliente")
image: "/images/news/nombre-del-archivo-de-la-noticia.jpg" (Ruta a la imagen principal de la noticia, debe tener el mismo nombre que el archivo de la noticia)
---
```

Ejemplo real:

```yaml
---
title: "Claude 4 llega con nuevas capacidades para pequeños negocios"
description: "El nuevo modelo de IA de Anthropic promete revolucionar la atención al cliente"
publishDate: 2025-01-20
author: "IA para tu día"
tags: ["claude", "chatbots", "atencion-cliente"]
featured: true
image: "/images/news/2025-01-20-claude-nuevo-modelo.jpg"
readTime: "3 min"
impact: "alto"
category: "atencion-cliente"
---
```

### 2. Contenido Principal

Después del encabezado YAML, escribe el contenido de la noticia en Markdown. Aquí hay algunos elementos importantes:

#### Título Principal (H1)
El primer encabezado debe ser un H1 (`#`) que coincida con el título del front matter.

#### Subtítulos
Usa encabezados H2 (`##`) para las secciones principales de la noticia.

#### Listas
Puedes usar listas ordenadas (`1.`, `2.`) o desordenadas (`-`, `*`) para enumerar puntos clave.

#### Enlaces
Para enlazar a recursos externos, usa la sintaxis: `[texto del enlace](URL)`.

#### Imágenes
Si necesitas insertar una imagen en el cuerpo del artículo (no en el front matter), usa:
`![Texto alternativo](ruta/a/la/imagen.jpg)`

### 3. Buenas Prácticas

- **Claridad y Objetividad:** Escribe de forma clara y concisa. Prioriza la información más importante al principio.
- **Valor Práctico:** Enfócate en cómo la noticia afecta a las PyMEs y cómo pueden aplicarla.
- **Estructura Clara:** Divide el contenido en secciones con subtítulos para facilitar la lectura.
- **Lenguaje Natural:** Usa un lenguaje cercano y natural, evitando tecnicismos innecesarios.
- **Longitud Recomendada:** Aproximadamente 400-600 palabras, lo que equivale a 2-4 minutos de lectura.
- **Fecha de Publicación:** Asegúrate de que la `publishDate` sea la fecha en que se debe publicar la noticia, no necesariamente la fecha actual de creación.
- **Imágenes:** Cada noticia debe tener una imagen principal. La imagen debe guardarse en el directorio `images/news/` y tener el mismo nombre que el archivo de la noticia (incluyendo la fecha y la extensión `.jpg`).

### 4. Categorías y Etiquetas

#### Categorías Principales:
- `tecnologia-ia`
- `marketing`
- `atencion-cliente`
- `productividad`
- `recursos-humanos`
- `finanzas`
- `gobierno-digital`
- `diseno`

#### Tags:
Utiliza entre 3 y 6 tags que describan de forma precisa el contenido de la noticia. Trata de usar tags ya existentes en otras noticias si son relevantes.

### 5. Impacto

Clasifica el impacto de la noticia como:
- `alto`: Cambios significativos o herramientas que afectan a muchos negocios.
- `medio`: Actualizaciones importantes de herramientas o tendencias consolidadas.
- `bajo`: Noticias menores, consejos específicos o pequeñas actualizaciones.

### 6. Destacados

Utiliza `featured: true` para noticias que sean particularmente importantes o que representen tendencias clave del momento.

### 7. Tiempo de Lectura

Estima el tiempo de lectura en minutos. Un párrafo corto equivale a aproximadamente 20-30 segundos de lectura.

## Ejemplo Completo

```markdown
---
title: "Título de la Noticia"
description: "Descripción breve de la noticia (150-160 caracteres)"
publishDate: 2025-07-30
author: "IA para tu día"
tags: ["tag1", "tag2", "tag3", "tag4"]
featured: false
readTime: "3 min"
impact: "medio"
category: "marketing"
image: "/images/news/2025-07-30-titulo-de-la-noticia.jpg"
---

# Título de la Noticia

Introducción breve y atractiva a la noticia.

## Sección Principal 1

Contenido detallado de la primera sección.

## Sección Principal 2

Contenido detallado de la segunda sección.

## Conclusión

Resumen de los puntos clave y su importancia para las PyMEs.
```