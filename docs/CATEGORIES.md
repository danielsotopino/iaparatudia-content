# CATEGORIES.md - Categorías Autorizadas

**Última actualización**: 2025-10-13
**Versión**: 1.0

---

## 📋 Propósito

Este documento define las categorías oficiales para organizar el contenido de iaparatudia. Cada pieza de contenido debe tener exactamente UNA categoría principal.

---

## 🎯 CATEGORÍAS PARA HERRAMIENTAS

| Categoría | Slug | Descripción | Ejemplos |
|-----------|------|-------------|----------|
| **Productividad** | `productividad` | Herramientas para mejorar eficiencia personal y de equipos | Notion, Monday, Slack |
| **Marketing Digital** | `marketing-digital` | Herramientas para marketing, redes sociales, publicidad | Canva, Copy.ai, Meta Business |
| **Atención al Cliente** | `atencion-cliente` | Herramientas para soporte, chatbots, CRM de servicio | ChatGPT, Freshdesk, Zendesk |
| **Ventas** | `ventas` | CRM, pipeline de ventas, prospección | HubSpot CRM, Pipedrive, Salesforce |
| **Análisis** | `analisis` | BI, visualización de datos, analytics | Tableau, Power BI, Julius AI |
| **Comunicación** | `comunicacion` | Email, mensajería, videoconferencias | Slack, Zoom, Microsoft Teams |
| **Operaciones** | `operaciones` | Gestión de proyectos, procesos, workflows | Monday, Asana, Trello |
| **Finanzas** | `finanzas` | Contabilidad, facturación, FP&A | QuickBooks, Dext, Banco Estado |
| **Recursos Humanos** | `recursos-humanos` | RRHH, nómina, reclutamiento, evaluaciones | BambooHR, Factorial, Buk |
| **Diseño** | `diseno` | Diseño gráfico, web, UI/UX, prototipado | Figma, Framer, Uizard |
| **Automatización** | `automatizacion` | Herramientas de integración y automatización | Zapier, Make, n8n |

---

## 🎯 CATEGORÍAS PARA NOTICIAS

| Categoría | Slug | Descripción | Ejemplos |
|-----------|------|-------------|----------|
| **Tecnología IA** | `tecnologia-ia` | Lanzamientos de modelos, avances tecnológicos en IA | GPT-5, Claude 4, Gemini Pro |
| **Marketing** | `marketing` | Tendencias y herramientas de marketing digital | Nuevas funciones en Meta Ads, Google Ads IA |
| **Atención al Cliente** | `atencion-cliente` | Innovaciones en servicio al cliente, chatbots | Automatización de soporte, nuevos CRM |
| **Productividad** | `productividad` | Herramientas y técnicas para mejorar productividad | Integraciones, nuevas funciones Notion |
| **Recursos Humanos** | `recursos-humanos` | RRHH, gestión de talento, bienestar laboral | Plataformas de reclutamiento con IA |
| **Finanzas** | `finanzas` | Fintech, contabilidad automatizada, análisis financiero | IA en contabilidad, apps de facturación |
| **Gobierno Digital** | `gobierno-digital` | Políticas públicas, regulación, iniciativas gubernamentales | Estrategia Nacional de IA Chile |
| **Diseño** | `diseno` | Tendencias en diseño, nuevas herramientas creativas | Figma AI, generadores de diseño |

---

## 🎯 CATEGORÍAS PARA TUTORIALES

| Categoría | Slug | Descripción | Ejemplos de Tutoriales |
|-----------|------|-------------|------------------------|
| **Atención al Cliente** | `atencion-cliente` | Configurar chatbots, automatizar respuestas | "Automatizar WhatsApp Business" |
| **Marketing** | `marketing` | Crear campañas, diseñar contenido | "Crear posts con Canva AI" |
| **Productividad** | `productividad` | Optimizar workflows, organizar tareas | "Configurar Notion para equipos" |
| **Finanzas** | `finanzas` | Automatizar contabilidad, reportes financieros | "Conectar QuickBooks con banco" |
| **Recursos Humanos** | `recursos-humanos` | Gestionar empleados, automatizar nómina | "Automatizar onboarding en BambooHR" |
| **Diseño** | `diseno` | Crear diseños, prototipar, editar | "Diseñar landing page en Framer" |
| **Automatización** | `automatizacion` | Conectar herramientas, crear workflows | "Integrar CRM con email en Zapier" |

---

## 📏 REGLAS DE USO

### Regla 1: Una Sola Categoría
Cada contenido debe tener **exactamente UNA** categoría principal.

❌ **Incorrecto**: `category: ["ventas", "marketing"]`
✅ **Correcto**: `category: "ventas"`

### Regla 2: Elegir la Más Específica
Si una herramienta sirve para múltiples áreas, elegir la función principal.

**Ejemplo**: HubSpot tiene marketing y ventas
- **Categoría correcta**: `"ventas"` (función principal: CRM)
- **Tags**: `["CRM", "Ventas", "Marketing", "Automatización"]` (funciones secundarias)

### Regla 3: Formato Obligatorio
- **Siempre** en minúsculas
- **Siempre** con guiones (no espacios, no underscores)
- **Siempre** sin tildes

❌ **Incorrecto**: `"Atención al Cliente"`, `"atencion_cliente"`, `"ATENCION-CLIENTE"`
✅ **Correcto**: `"atencion-cliente"`

### Regla 4: Consistencia Semántica
Usar la categoría que mejor describe el **problema que resuelve** o **área de aplicación**, no la tecnología.

**Ejemplo**: Un chatbot para ventas
- ❌ `"comunicacion"` (tecnología)
- ✅ `"ventas"` (área de aplicación)

---

## 🔍 GUÍA DE DECISIÓN

### ¿Cómo Elegir la Categoría Correcta?

#### Para Herramientas
1. **¿Cuál es la función principal?** (no todas las funciones)
2. **¿Qué problema resuelve primero?**
3. **¿En qué departamento se usa más?**

**Ejemplo: Slack AI**
- Funciones: Comunicación, búsqueda con IA, resúmenes
- Problema principal: Comunicación de equipos
- Departamento: Toda la empresa, pero comunicación es core
- **Categoría**: `"comunicacion"`

**Ejemplo: Tableau**
- Funciones: BI, visualización, dashboards
- Problema principal: Analizar datos para decisiones
- Departamento: Análisis/BI
- **Categoría**: `"analisis"`

#### Para Noticias
1. **¿Qué tema principal aborda?**
2. **¿A qué área impacta más?**
3. **¿Es sobre tecnología o aplicación?**

**Ejemplo: "Google lanza herramientas IA para PyMEs"**
- Tema: Lanzamiento de tecnología
- Impacto: Tecnología en general
- **Categoría**: `"tecnologia-ia"`

**Ejemplo: "Cómo la IA está transformando el marketing en Latinoamérica"**
- Tema: Aplicación de IA
- Impacto: Marketing
- **Categoría**: `"marketing"`

#### Para Tutoriales
1. **¿Qué resultado obtiene el usuario?**
2. **¿En qué área de su negocio lo aplicará?**

**Ejemplo: "Automatizar respuestas de WhatsApp"**
- Resultado: Atención automatizada
- Área de aplicación: Servicio al cliente
- **Categoría**: `"atencion-cliente"`

---

## 🔄 CATEGORÍAS RELACIONADAS

Algunas categorías son similares. Usar esta guía para decidir:

### `marketing-digital` vs `diseno`
- **Marketing Digital**: Herramientas para campañas, ads, contenido de marketing
- **Diseño**: Herramientas para diseño gráfico, web, UI/UX
- **Ejemplo**: Canva → `"marketing-digital"` (aunque diseña, su uso principal es marketing)
- **Ejemplo**: Figma → `"diseno"` (herramienta profesional de diseño)

### `ventas` vs `atencion-cliente`
- **Ventas**: CRM, prospección, pipeline, cerrar ventas
- **Atención al Cliente**: Soporte post-venta, tickets, chatbots de ayuda
- **Ejemplo**: HubSpot CRM → `"ventas"`
- **Ejemplo**: Zendesk → `"atencion-cliente"`

### `analisis` vs `finanzas`
- **Análisis**: BI general, visualización de cualquier tipo de datos
- **Finanzas**: Específico de contabilidad, facturación, análisis financiero
- **Ejemplo**: Tableau → `"analisis"` (BI general)
- **Ejemplo**: QuickBooks → `"finanzas"` (contabilidad específica)

### `productividad` vs `operaciones`
- **Productividad**: Herramientas personales o de equipo pequeño
- **Operaciones**: Gestión de procesos, proyectos complejos, workflows empresariales
- **Ejemplo**: Notion → `"productividad"` (personal/equipo)
- **Ejemplo**: Monday → `"operaciones"` (gestión de proyectos empresarial)

### `comunicacion` vs `productividad`
- **Comunicación**: Enfoque en comunicación entre personas (chat, video, email)
- **Productividad**: Enfoque en organización, tareas, documentos
- **Ejemplo**: Slack → `"comunicacion"`
- **Ejemplo**: Notion → `"productividad"`

---

## ❌ CATEGORÍAS DEPRECADAS

Estas categorías se usaban antes pero ya no:

| Categoría Antigua | Reemplazar Por | Razón |
|-------------------|----------------|-------|
| `tecnología` | `tecnologia-ia` | Falta tilde, ser más específico |
| `gobierno` | `gobierno-digital` | Ser más específico |
| `marketing` (en herramientas) | `marketing-digital` | Consistencia |

---

## ➕ AGREGAR NUEVAS CATEGORÍAS

### Criterios para Nueva Categoría
1. **Necesidad**: ¿Hay 5+ herramientas/noticias que no encajan en existentes?
2. **Diferenciación**: ¿Es suficientemente diferente de las existentes?
3. **Permanencia**: ¿Es una categoría duradera o temporal?
4. **Claridad**: ¿Los usuarios entenderán qué va en esta categoría?

### Proceso
1. Verificar que no existe categoría similar
2. Definir claramente el alcance
3. Proponer en issue/PR con justificación
4. Si se aprueba, agregar a este documento
5. Actualizar schemas en `iaparatudia-web/src/content/config.ts`

---

## 📊 ESTADÍSTICAS

### Herramientas
- Total de categorías: 11
- Más usada: `productividad` (~20%)
- Menos usada: `automatizacion` (~3%)

### Noticias
- Total de categorías: 8
- Más usada: `tecnologia-ia` (~40%)
- Menos usada: `gobierno-digital` (~5%)

---

## 🔍 VERIFICACIÓN

### Verificar Categorías en Uso
```bash
# Listar categorías de herramientas
grep "^category:" tools/*.md | sort | uniq -c | sort -rn

# Listar categorías de noticias
grep "^category:" news/*.md | sort | uniq -c | sort -rn
```

### Encontrar Categorías Inválidas
```bash
# Buscar categorías no autorizadas
grep "^category:" tools/*.md news/*.md tutorials/*.md | \
  grep -v "productividad\|marketing-digital\|atencion-cliente\|ventas\|analisis\|comunicacion\|operaciones\|finanzas\|recursos-humanos\|diseno\|automatizacion\|tecnologia-ia\|marketing\|gobierno-digital"
```

---

## 📝 NOTAS PARA AGENTES DE IA

Al generar contenido:
1. **SIEMPRE** usar formato `minusculas-con-guiones`
2. **ELEGIR** solo UNA categoría (la más específica)
3. **VERIFICAR** que la categoría exista en este documento
4. **SI** no estás seguro, usar:
   - Herramientas → `productividad` (default seguro)
   - Noticias → `tecnologia-ia` (default seguro)
5. **TAGS** pueden incluir temas secundarios

---

**Mantenido por**: Equipo editorial iaparatudia
**Revisión**: Trimestral
**Última revisión**: 2025-10-13
