# Auditoría de Rutas de Imágenes - iaparatudia-content

**Fecha:** 2025-10-13
**Proyecto:** iaparatudia-content
**Ubicación:** /Users/danielsotopino/Documents/iaparatudia/iaparatudia-content

---

## Resumen Ejecutivo

### Estadísticas Generales
- **Total de referencias a imágenes encontradas:** 28 referencias
- **Archivos markdown analizados:** 30 archivos (19 tools + 10 news + 1 tutorials)
- **Rutas incorrectas detectadas:** 9 referencias
- **Imágenes faltantes:** 15 archivos de imagen
- **Tasa de error:** 32% de las referencias tienen problemas

---

## 1. Estructura de Directorios de Imágenes

### Directorios Existentes
```
/images/
├── news/           ✅ Existe
├── tools/          ✅ Existe
└── tutorials/      ✅ Existe (vacío)
```

### Análisis de Convención
- **Directorio correcto:** `/images/tools/`
- **Directorio incorrecto usado:** `/images/tools/` (NO EXISTE)
- **Directorio vacío:** `/images/tutorials/` (existe pero sin archivos)

---

## 2. Rutas Incorrectas Detectadas

### 2.1 Archivos que usan `/images/tools/` (INCORRECTO)

| Archivo | Línea | Ruta Incorrecta | Ruta Correcta Sugerida |
|---------|-------|-----------------|------------------------|
| `formato-herramientas.md` | 65 | `/images/tools/canva-ai-hero.jpg` | `/images/tools/canva-ai-hero.jpg` |
| `tools/canva-ai.md` | 18 | `/images/tools/canva-ai-hero.jpg` | `/images/tools/canva-ai-hero.jpg` |
| `tools/canva-ai.md` | 36 | `/images/tools/canva-planes.png` | `/images/tools/canva-planes.png` |
| `tools/canva-ai.md` | 47 | `/images/tools/canva-proceso.gif` | `/images/tools/canva-proceso.gif` |
| `tools/copy-ai-marketing.md` | 18 | `/images/tools/copy-ai-logo.jpg` | `/images/tools/copy-ai-logo.png` |
| `tools/chatgpt-atencion-cliente.md` | 18 | `/images/tools/chatgpt-logo.jpg` | `/images/tools/chatgpt-logo.ico` |
| `tools/zapier-automatizacion.md` | 18 | `/images/tools/zapier-logo.jpg` | `/images/tools/zapier-logo.png` |
| `tools/monday-gestion-proyectos.md` | 18 | `/images/tools/monday-logo.jpg` | `/images/tools/monday-logo.ico` |
| `tools/bamboohr-recursos-humanos.md` | 18 | `/images/tools/bamboohr-logo.jpg` | `/images/tools/bamboohr-logo.ico` |
| `tools/notion-ai-productividad.md` | 18 | `/images/tools/notion-logo.jpg` | `/images/tools/notion-logo.ico` |
| `tools/hubspot-crm.md` | 18 | `/images/tools/hubspot-logo.jpg` | `/images/tools/hubspot-logo.png` |

**Total:** 11 referencias con ruta incorrecta

---

## 3. Imágenes Faltantes

### 3.1 Imágenes Referenciadas pero NO Existen en Disco

#### En `/images/tools/` (imágenes con sufijo `-hero`)
| Archivo Referencia | Imagen Faltante |
|--------------------|-----------------|
| `tools/slack-ai.md` | `/images/tools/slack-ai-hero.jpg` |
| `tools/quickbooks-ai.md` | `/images/tools/quickbooks-ai-hero.jpg` |
| `tools/powerbi-ai.md` | `/images/tools/powerbi-ai-hero.jpg` |
| `tools/dext-ai.md` | `/images/tools/dext-hero.jpg` |
| `tools/tableau-ai.md` | `/images/tools/tableau-ai-hero.jpg` |
| `tools/miro-ai.md` | `/images/tools/miro-ai-hero.jpg` |
| `tools/uizard-ai.md` | `/images/tools/uizard-ai-hero.jpg` |
| `tools/venasolutions-ai.md` | `/images/tools/venasolutions-hero.jpg` |
| `tools/otter-ai.md` | `/images/tools/otter-ai-hero.jpg` |
| `tools/julius-ai.md` | `/images/tools/julius-ai-hero.jpg` |
| `tools/framer-ai.md` | `/images/tools/framer-ai-hero.jpg` |

#### En `/images/tools/` (directorio incorrecto)
| Archivo Referencia | Imagen Faltante |
|--------------------|-----------------|
| `tools/canva-ai.md` | `/images/tools/canva-ai-hero.jpg` |
| `tools/canva-ai.md` | `/images/tools/canva-planes.png` |
| `tools/canva-ai.md` | `/images/tools/canva-proceso.gif` |

#### En `/images/tutorials/` (directorio vacío)
| Archivo Referencia | Imagen Faltante |
|--------------------|-----------------|
| `tutorials/whatsapp-respuestas-automaticas.md` | `/images/tutoriales/whatsapp-automation-cover.jpg` |
| `tutorials/whatsapp-respuestas-automaticas.md` | `/images/tutoriales/whatsapp-paso1.jpg` |
| `tutorials/whatsapp-respuestas-automaticas.md` | `/images/tutoriales/whatsapp-paso2.jpg` |
| `tutorials/whatsapp-respuestas-automaticas.md` | `/images/tutoriales/whatsapp-respuestas-rapidas.png` |
| `tutorials/whatsapp-respuestas-automaticas.md` | `/images/tutoriales/whatsapp-resultado.gif` |

**Total:** 20 imágenes faltantes

---

## 4. Imágenes Existentes en Disco

### 4.1 Directorio `/images/tools/` (19 archivos)
```
✅ bamboohr-logo.ico
✅ canva-ai-logo.png
✅ chatgpt-logo.ico
✅ copy-ai-logo.png
✅ dext-logo.ico
✅ framer-ai-logo.png
✅ hubspot-logo.png
✅ julius-ai-logo.jpg
✅ miro-ai-logo.jpg
✅ monday-logo.ico
✅ notion-logo.ico
✅ otter-ai-logo.jpg
✅ powerbi-ai-logo.jpg
✅ quickbooks-ai-logo.jpg
✅ slack-ai-logo.png
✅ tableau-ai-logo.jpg
✅ uizard-ai-logo.jpg
✅ venasolutions-ai-logo.jpg
✅ zapier-logo.png
```

### 4.2 Directorio `/images/news/` (10 archivos)
```
✅ 2025-01-15-google-ai-pymes-2025.jpg
✅ 2025-01-25-ia-integrada-revolucion.jpg
✅ 2025-01-26-herramientas-ia-marketing.jpg
✅ 2025-01-27-ia-atencion-cliente.jpg
✅ 2025-07-26-qwen-coder-nuevo-modelo.jpg
✅ 2025-07-27-chile-innovacion-municipal.jpg
✅ 2025-07-28-gemma-nuevo-modelo.jpg
✅ claude-4-family.jpg
✅ claude-4-launch.jpg
✅ openai-gpt-oss-launch.jpg
```

### 4.3 Directorio `/images/tutorials/`
```
❌ VACÍO - No contiene archivos
```

---

## 5. Problemas de Inconsistencia

### 5.1 Extensiones de Archivo Incorrectas
Algunos archivos markdown referencian extensiones `.jpg` cuando el archivo real es `.png` o `.ico`:

| Archivo MD | Referencia | Archivo Real |
|------------|------------|--------------|
| `copy-ai-marketing.md` | `copy-ai-logo.jpg` | `copy-ai-logo.png` |
| `chatgpt-atencion-cliente.md` | `chatgpt-logo.jpg` | `chatgpt-logo.ico` |
| `zapier-automatizacion.md` | `zapier-logo.jpg` | `zapier-logo.png` |
| `monday-gestion-proyectos.md` | `monday-logo.jpg` | `monday-logo.ico` |
| `bamboohr-recursos-humanos.md` | `bamboohr-logo.jpg` | `bamboohr-logo.ico` |
| `notion-ai-productividad.md` | `notion-logo.jpg` | `notion-logo.ico` |
| `hubspot-crm.md` | `hubspot-logo.jpg` | `hubspot-logo.png` |

### 5.2 Convención de Nombres
Se detectan dos patrones:
- **Logo:** `[herramienta]-logo.[ext]` (usado en frontmatter)
- **Hero:** `[herramienta]-hero.jpg` (usado en contenido)

**Problema:** Todos los archivos existentes son `-logo`, pero las referencias en el contenido buscan `-hero`.

---

## 6. Correcciones Recomendadas

### 6.1 Corrección de Ruta: `/images/tools/` → `/images/tools/`

#### Comando sed para Linux/Mac:
```bash
# Backup de archivos antes de modificar
cp /Users/danielsotopino/Documents/iaparatudia/iaparatudia-content/formato-herramientas.md /Users/danielsotopino/Documents/iaparatudia/iaparatudia-content/formato-herramientas.md.bak

# Reemplazar en todos los archivos markdown
find /Users/danielsotopino/Documents/iaparatudia/iaparatudia-content -name "*.md" -type f -exec sed -i '' 's|/images/tools/|/images/tools/|g' {} +
```

### 6.2 Corrección de Extensiones de Archivo

```bash
# Script para corregir extensiones específicas
cd /Users/danielsotopino/Documents/iaparatudia/iaparatudia-content

# Copy.ai
sed -i '' 's|copy-ai-logo\.jpg|copy-ai-logo.png|g' tools/copy-ai-marketing.md

# ChatGPT
sed -i '' 's|chatgpt-logo\.jpg|chatgpt-logo.ico|g' tools/chatgpt-atencion-cliente.md

# Zapier
sed -i '' 's|zapier-logo\.jpg|zapier-logo.png|g' tools/zapier-automatizacion.md

# Monday
sed -i '' 's|monday-logo\.jpg|monday-logo.ico|g' tools/monday-gestion-proyectos.md

# BambooHR
sed -i '' 's|bamboohr-logo\.jpg|bamboohr-logo.ico|g' tools/bamboohr-recursos-humanos.md

# Notion
sed -i '' 's|notion-logo\.jpg|notion-logo.ico|g' tools/notion-ai-productividad.md

# HubSpot
sed -i '' 's|hubspot-logo\.jpg|hubspot-logo.png|g' tools/hubspot-crm.md
```

### 6.3 Corrección de Rutas de Imágenes Hero → Logo

Como todas las imágenes hero están faltantes pero existen las versiones `-logo`, se recomienda:

**Opción A: Cambiar referencias de `-hero` a `-logo`**
```bash
# Reemplazar todas las referencias -hero.jpg por -logo
find /Users/danielsotopino/Documents/iaparatudia/iaparatudia-content/tools -name "*.md" -type f -exec sed -i '' 's|-hero\.jpg|-logo.jpg|g' {} +
```

**Opción B: Crear imágenes hero faltantes**
- Duplicar o crear imágenes hero basadas en los logos existentes
- Mantener la convención actual de usar `-hero` para imágenes principales

### 6.4 Corrección Tutorial WhatsApp

```bash
# Nota: El tutorial usa /images/tutoriales/ pero el directorio es /images/tutorials/
# Corregir la ruta base
sed -i '' 's|/images/tutoriales/|/images/tutorials/|g' /Users/danielsotopino/Documents/iaparatudia/iaparatudia-content/tutorials/whatsapp-respuestas-automaticas.md
```

---

## 7. Script de Corrección Completo

### Archivo: `fix-image-paths.sh`

```bash
#!/bin/bash

# Script de corrección masiva de rutas de imágenes
# Proyecto: iaparatudia-content
# Fecha: 2025-10-13

BASE_DIR="/Users/danielsotopino/Documents/iaparatudia/iaparatudia-content"

echo "=== Iniciando corrección de rutas de imágenes ==="
echo "Directorio base: $BASE_DIR"
echo ""

# 1. Crear backup
echo "[1/5] Creando backup..."
BACKUP_DIR="${BASE_DIR}_backup_$(date +%Y%m%d_%H%M%S)"
cp -r "$BASE_DIR" "$BACKUP_DIR"
echo "Backup creado en: $BACKUP_DIR"
echo ""

# 2. Corregir /images/tools/ → /images/tools/
echo "[2/5] Corrigiendo ruta /images/tools/ → /images/tools/..."
find "$BASE_DIR" -name "*.md" -type f -exec sed -i '' 's|/images/tools/|/images/tools/|g' {} +
echo "✓ Rutas de directorio corregidas"
echo ""

# 3. Corregir extensiones de archivo incorrectas
echo "[3/5] Corrigiendo extensiones de archivo..."
sed -i '' 's|copy-ai-logo\.jpg|copy-ai-logo.png|g' "$BASE_DIR/tools/copy-ai-marketing.md"
sed -i '' 's|chatgpt-logo\.jpg|chatgpt-logo.ico|g' "$BASE_DIR/tools/chatgpt-atencion-cliente.md"
sed -i '' 's|zapier-logo\.jpg|zapier-logo.png|g' "$BASE_DIR/tools/zapier-automatizacion.md"
sed -i '' 's|monday-logo\.jpg|monday-logo.ico|g' "$BASE_DIR/tools/monday-gestion-proyectos.md"
sed -i '' 's|bamboohr-logo\.jpg|bamboohr-logo.ico|g' "$BASE_DIR/tools/bamboohr-recursos-humanos.md"
sed -i '' 's|notion-logo\.jpg|notion-logo.ico|g' "$BASE_DIR/tools/notion-ai-productividad.md"
sed -i '' 's|hubspot-logo\.jpg|hubspot-logo.png|g' "$BASE_DIR/tools/hubspot-crm.md"
echo "✓ Extensiones corregidas"
echo ""

# 4. Corregir referencias -hero a -logo (considerando las extensiones reales)
echo "[4/5] Corrigiendo referencias de imágenes hero..."
# Slack AI
sed -i '' 's|slack-ai-hero\.jpg|slack-ai-logo.png|g' "$BASE_DIR/tools/slack-ai.md"
# QuickBooks AI
sed -i '' 's|quickbooks-ai-hero\.jpg|quickbooks-ai-logo.jpg|g' "$BASE_DIR/tools/quickbooks-ai.md"
# Power BI AI
sed -i '' 's|powerbi-ai-hero\.jpg|powerbi-ai-logo.jpg|g' "$BASE_DIR/tools/powerbi-ai.md"
# Dext AI
sed -i '' 's|dext-hero\.jpg|dext-logo.ico|g' "$BASE_DIR/tools/dext-ai.md"
# Tableau AI
sed -i '' 's|tableau-ai-hero\.jpg|tableau-ai-logo.jpg|g' "$BASE_DIR/tools/tableau-ai.md"
# Miro AI
sed -i '' 's|miro-ai-hero\.jpg|miro-ai-logo.jpg|g' "$BASE_DIR/tools/miro-ai.md"
# Uizard AI
sed -i '' 's|uizard-ai-hero\.jpg|uizard-ai-logo.jpg|g' "$BASE_DIR/tools/uizard-ai.md"
# Vena Solutions
sed -i '' 's|venasolutions-hero\.jpg|venasolutions-ai-logo.jpg|g' "$BASE_DIR/tools/venasolutions-ai.md"
# Otter AI
sed -i '' 's|otter-ai-hero\.jpg|otter-ai-logo.jpg|g' "$BASE_DIR/tools/otter-ai.md"
# Julius AI
sed -i '' 's|julius-ai-hero\.jpg|julius-ai-logo.jpg|g' "$BASE_DIR/tools/julius-ai.md"
# Framer AI
sed -i '' 's|framer-ai-hero\.jpg|framer-ai-logo.png|g' "$BASE_DIR/tools/framer-ai.md"
# Canva AI (ya se corrigió el directorio, ahora las imágenes específicas)
sed -i '' 's|canva-ai-hero\.jpg|canva-ai-logo.png|g' "$BASE_DIR/tools/canva-ai.md"
sed -i '' 's|canva-planes\.png|canva-ai-logo.png|g' "$BASE_DIR/tools/canva-ai.md"
sed -i '' 's|canva-proceso\.gif|canva-ai-logo.png|g' "$BASE_DIR/tools/canva-ai.md"
sed -i '' 's|canva-ai-hero\.jpg|canva-ai-logo.png|g' "$BASE_DIR/formato-herramientas.md"
echo "✓ Referencias hero corregidas"
echo ""

# 5. Corregir ruta de tutorials: tutoriales → tutorials
echo "[5/5] Corrigiendo ruta /images/tutoriales/ → /images/tutorials/..."
sed -i '' 's|/images/tutoriales/|/images/tutorials/|g' "$BASE_DIR/tutorials/whatsapp-respuestas-automaticas.md"
echo "✓ Ruta de tutorials corregida"
echo ""

echo "=== Corrección completada ==="
echo "Archivos modificados:"
find "$BASE_DIR" -name "*.md" -type f -newer "$BACKUP_DIR" | wc -l
echo ""
echo "Para verificar cambios:"
echo "  diff -r $BACKUP_DIR $BASE_DIR"
echo ""
echo "Para restaurar backup (si es necesario):"
echo "  rm -rf $BASE_DIR && mv $BACKUP_DIR $BASE_DIR"
```

### Comandos para Ejecutar el Script

```bash
# Dar permisos de ejecución
chmod +x /Users/danielsotopino/Documents/iaparatudia/iaparatudia-content/fix-image-paths.sh

# Ejecutar el script
/Users/danielsotopino/Documents/iaparatudia/iaparatudia-content/fix-image-paths.sh
```

---

## 8. Verificación Post-Corrección

### Verificar que no queden referencias a /images/tools/
```bash
grep -r "/images/tools/" /Users/danielsotopino/Documents/iaparatudia/iaparatudia-content --include="*.md"
```

### Verificar que no queden referencias a imágenes -hero
```bash
grep -r "\-hero\." /Users/danielsotopino/Documents/iaparatudia/iaparatudia-content --include="*.md"
```

### Listar todas las referencias a imágenes actuales
```bash
grep -r "!\[.*\](.*/images/.*)" /Users/danielsotopino/Documents/iaparatudia/iaparatudia-content --include="*.md" -h | sort | uniq
```

---

## 9. Recomendaciones Finales

### 9.1 Prevención Futura
1. **Crear plantilla de herramienta** con la estructura correcta de rutas
2. **Documentar convención:** Usar `/images/tools/` NO `/images/tools/`
3. **Script de validación:** Crear pre-commit hook para verificar rutas de imágenes
4. **Guía de contribución:** Actualizar `CONTRIBUTING.md` con convenciones de imágenes

### 9.2 Imágenes Faltantes Prioritarias
Las siguientes imágenes deben ser creadas o agregadas:
- **Tutorial WhatsApp (5 imágenes):** Alta prioridad - tutorial publicado sin imágenes
- **Imágenes Hero de Tools (11 imágenes):** Media prioridad - actualmente usando logos como fallback
- **Canva imágenes adicionales (2 imágenes):** Baja prioridad - planes y proceso

### 9.3 Convención Propuesta
```
Tipo de contenido → Directorio → Nomenclatura de archivo
─────────────────────────────────────────────────────────
tools/              → /images/tools/      → [slug]-logo.[ext]
news/               → /images/news/       → [fecha]-[slug].[ext]
tutorials/          → /images/tutorials/  → [slug]-[descripcion].[ext]
```

---

## 10. Archivos Afectados (Resumen)

### Archivos con Problemas (17 archivos)
```
formato-herramientas.md
tools/canva-ai.md
tools/copy-ai-marketing.md
tools/chatgpt-atencion-cliente.md
tools/zapier-automatizacion.md
tools/monday-gestion-proyectos.md
tools/bamboohr-recursos-humanos.md
tools/notion-ai-productividad.md
tools/hubspot-crm.md
tools/slack-ai.md
tools/quickbooks-ai.md
tools/powerbi-ai.md
tools/dext-ai.md
tools/tableau-ai.md
tools/miro-ai.md
tools/uizard-ai.md
tools/venasolutions-ai.md
tools/otter-ai.md
tools/julius-ai.md
tools/framer-ai.md
tutorials/whatsapp-respuestas-automaticas.md
```

### Archivos Sin Problemas (10 archivos news)
Los archivos en `/news/` actualmente no tienen referencias a imágenes en su contenido.

---

**Fin del Reporte**
