# TAGS.md - Taxonomía Oficial de Tags

**Última actualización**: 2025-10-13
**Versión**: 1.0

---

## 📋 Propósito

Este documento define las convenciones y formato para tags en iaparatudia. Los tags ayudan a:
- Categorizar contenido para búsqueda y filtrado
- Mejorar SEO
- Relacionar contenido temático
- Facilitar navegación del usuario

---

## 🎯 Convenciones Obligatorias

### Formato Estándar
- **Capitalización**: Title Case (Primera Letra Mayúscula En Cada Palabra)
- **Separación**: Usar espacios, NO guiones ni underscores
- **Idioma**: Español (excepto nombres propios, marcas y acrónimos)
- **Cantidad**: 3-6 tags por contenido
- **Longitud**: Máximo 3 palabras por tag

### Ejemplos Correctos
✅ "Análisis de Datos"
✅ "Atención al Cliente"
✅ "CRM"
✅ "WhatsApp Business"
✅ "Gestión de Proyectos"

### Ejemplos Incorrectos
❌ "análisis-de-datos" (minúsculas con guiones)
❌ "ATENCIÓN AL CLIENTE" (mayúsculas completas)
❌ "crm" (minúsculas cuando es acrónimo conocido)
❌ "herramienta-de-gestion-de-proyectos-para-equipos" (demasiado largo)

---

## 📚 TAGS EXISTENTES (Ejemplos por Categoría)

> **Nota**: Estas listas son ejemplos, NO exhaustivas. Puedes agregar nuevos tags siguiendo las convenciones.

### Categoría: Herramientas y Plataformas
*Nombres de herramientas específicas*
- CRM
- BI
- ERP
- WhatsApp Business
- Google Workspace
- Microsoft Copilot
- Slack
- Notion
- Zapier
- HubSpot

### Categoría: Funcionalidades
*Qué hace la herramienta o tecnología*
- Automatización
- Integración
- Productividad
- Análisis de Datos
- Visualización de Datos
- Transcripción
- Copywriting
- Prototipado
- No-Code
- IA Generativa
- Colaboración
- Chatbots
- Resúmenes

### Categoría: Áreas de Negocio
*Departamento o función empresarial*
- Ventas
- Marketing
- Atención al Cliente
- Recursos Humanos
- Finanzas
- Contabilidad
- Gestión de Proyectos
- Diseño Web
- Diseño UI
- Redes Sociales
- Operaciones
- Soporte

### Categoría: Tipos de Contenido/Salida
*Qué tipo de output genera*
- Documentos
- Informes
- Presentaciones
- Mapas Mentales
- Diagramas
- Maquetas
- Contenido
- Facturación
- Nómina

### Categoría: Tecnologías/Conceptos (Noticias)
*Tecnologías específicas o conceptos de IA*
- Código Abierto
- Modelos Abiertos
- Multimodal
- Desarrollo
- Programación
- Investigación
- Lenguaje Natural
- Machine Learning

### Categoría: Empresas/Marcas (Noticias)
*Organizaciones relevantes*
- Claude
- Anthropic
- OpenAI
- Google
- Microsoft
- Alibaba
- Meta

### Categoría: Modelos de IA (Noticias)
*Nombres específicos de modelos*
- GPT-4
- Claude Sonnet
- Gemma-3
- Qwen3-Coder
- GPT-OSS

### Categoría: Temas Sociales/Políticos (Noticias)
*Aspectos regulatorios o sociales*
- Política IA
- Ética
- Gobernanza
- Regulación
- Privacidad

### Categoría: Geografía (Noticias)
*Cuando la ubicación es relevante*
- Chile
- Latinoamérica
- PyMEs
- Global

---

## 🔄 MAPEO DE TAGS DEPRECADOS

Si encuentras estos tags antiguos, reemplázalos:

| Tag Antiguo | Tag Nuevo | Razón |
|-------------|-----------|-------|
| "ia" | "IA" | Acrónimo debe estar en mayúsculas |
| "pymes" | "PyMEs" | Formato correcto del acrónimo |
| "atencion-cliente" | "Atención al Cliente" | Usar espacios y tildes |
| "analisis" | "Análisis" o "Análisis de Datos" | Usar tildes y ser específico |
| "chatbot" | "Chatbots" | Preferir plural |
| "rrhh" | "Recursos Humanos" | Usar nombre completo |
| "codigo-abierto" | "Código Abierto" | Usar espacios y tildes |
| "minciencia" | "MinCiencia" | Capitalización correcta |
| "google-workspace" | "Google Workspace" | Usar espacios para marcas |
| "microsoft-copilot" | "Microsoft Copilot" | Usar espacios para marcas |

---

## ✏️ Guía para Elegir Tags

### Para Herramientas
1. **Nombre de la herramienta** (si es conocida): "HubSpot", "Notion"
2. **Funcionalidad principal**: "CRM", "Automatización"
3. **Área de aplicación**: "Ventas", "Marketing"
4. **Salida/Output**: "Informes", "Documentos" (opcional)

**Ejemplo**: HubSpot CRM
```yaml
tags: ["CRM", "Ventas", "Automatización", "Marketing"]
```

### Para Noticias
1. **Tecnología o empresa protagonista**: "Claude", "OpenAI"
2. **Concepto/tecnología principal**: "Código Abierto", "Multimodal"
3. **Impacto o área afectada**: "PyMEs", "Desarrollo"
4. **Región** (si es relevante): "Chile", "Latinoamérica"

**Ejemplo**: Lanzamiento Claude 4
```yaml
tags: ["Claude", "Anthropic", "IA", "Empresas", "Desarrollo"]
```

### Para Tutoriales
1. **Herramienta usada**: "WhatsApp Business", "Notion"
2. **Acción realizada**: "Automatización", "Integración"
3. **Área de aplicación**: "Atención al Cliente", "Productividad"

**Ejemplo**: Automatizar WhatsApp
```yaml
tags: ["WhatsApp Business", "Automatización", "Atención al Cliente"]
```

---

## 🚫 Tags No Permitidos

Evitar tags que sean:

### Demasiado Genéricos
❌ "Inteligencia Artificial" → Usar "IA"
❌ "Tecnología" → Obvio por el contexto del sitio
❌ "Herramienta" → Redundante
❌ "Software" → Redundante

### Información que va en Frontmatter
❌ "Gratis" → Usar campo `pricing`
❌ "Freemium" → Usar campo `pricing`
❌ "Principiante" → Usar campo `difficulty`
❌ "Nuevo" → Obvio por `publishDate`
❌ "2025" → Usar `publishDate`
❌ "Destacado" → Usar campo `featured`

### Redundantes o Duplicados
❌ "Análisis" y "Análisis de Datos" → Elegir uno
❌ "CRM" y "Gestión de Clientes" → Elegir uno
❌ "AI" y "IA" → Usar solo "IA"

---

## 🆕 Cómo Agregar Nuevos Tags

### Criterios de Aprobación
Un nuevo tag debe cumplir:
1. **Necesario**: No existe tag similar
2. **Específico**: Define claramente un concepto o herramienta
3. **Reutilizable**: Aplicable a múltiples contenidos
4. **Seguir convenciones**: Title Case, español, máximo 3 palabras

### Proceso
1. Verificar que no existe tag similar en este documento
2. Aplicar formato según convenciones
3. Usar en el contenido
4. Si se vuelve común (3+ usos), agregarlo a este documento

### Ejemplo
**Nuevo modelo de IA aparece**: "Llama 3"
- ✅ Válido como nuevo tag
- Formato correcto: "Llama 3"
- Categoría: Modelos de IA
- Se puede usar inmediatamente

---

## 📊 Estadísticas Actuales

- **Tags únicos en uso**: ~80
- **Tags estandarizados**: ~65
- **Promedio por herramienta**: 3-4 tags
- **Promedio por noticia**: 5-7 tags
- **Promedio por tutorial**: 3 tags

---

## 🔍 Búsqueda y Validación

### Verificar si un Tag Existe
```bash
# Buscar tag en todos los archivos
grep -r "\"Nombre Tag\"" tools/ news/ tutorials/
```

### Encontrar Tags Inconsistentes
```bash
# Buscar tags en minúsculas (probablemente incorrectos)
grep -r "tags:.*[a-z]-[a-z]" tools/ news/ tutorials/
```

### Listar Todos los Tags Únicos
```bash
grep -h "^tags:" tools/*.md news/*.md tutorials/*.md | sort | uniq
```

---

## 📝 Notas para Agentes de IA

Si eres un agente generando contenido:
1. **SIEMPRE** usar Title Case
2. **SIEMPRE** separar con espacios, no guiones
3. **Preferir** tags existentes cuando sea posible
4. **Puedes** crear nuevos tags siguiendo las convenciones
5. **Evitar** tags redundantes con frontmatter
6. **Limitar** a 3-6 tags por contenido

---

**Mantenido por**: Equipo editorial iaparatudia
**Revisión**: Trimestral
**Última revisión**: 2025-10-13
