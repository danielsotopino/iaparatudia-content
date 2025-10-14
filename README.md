# iaparatudia-content

Repositorio de contenido markdown para [iaparatudia.cl](https://iaparatudia.cl) - Plataforma de herramientas de IA para PyMEs en Chile y Latinoamérica.

---

## 📋 Estructura del Repositorio

```
iaparatudia-content/
├── templates/          # Templates formales para crear contenido
│   ├── template-herramienta.md
│   ├── template-noticia.md
│   └── template-tutorial.md
├── docs/               # Documentación y guías
│   ├── TAGS.md         # Taxonomía oficial de tags
│   ├── METADATA.md     # Especificación de campos frontmatter
│   ├── CATEGORIES.md   # Categorías autorizadas
│   └── IMAGE_AUDIT.md  # Auditoría de imágenes
├── tools/              # Herramientas de IA documentadas (19)
├── news/               # Noticias sobre IA (10)
├── tutorials/          # Tutoriales paso a paso (1)
├── images/             # Recursos multimedia
│   ├── tools/          # Logotipos de herramientas
│   ├── news/           # Imágenes de noticias
│   └── tutorials/      # Imágenes de tutoriales
├── formato-herramientas.md  # Guía de formato (legacy)
└── CONTRIBUTING.md     # Guía de contribución
```

---

## 🚀 Inicio Rápido

### Para Crear Nuevo Contenido

1. **Copia el template apropiado**:
   ```bash
   # Para herramienta
   cp templates/template-herramienta.md tools/nombre-herramienta.md

   # Para noticia
   cp templates/template-noticia.md news/$(date +%Y-%m-%d)-titulo-noticia.md

   # Para tutorial
   cp templates/template-tutorial.md tutorials/nombre-tutorial.md
   ```

2. **Completa el frontmatter** siguiendo los comentarios en el template

3. **Escribe el contenido** siguiendo la estructura del template

4. **Valida** que sigue las convenciones en `docs/`

### Recursos Importantes

- 📖 **Templates**: `/templates/` - Usa estos para crear contenido
- 📚 **Tags**: `docs/TAGS.md` - Lista oficial de tags y convenciones
- 🏷️ **Metadata**: `docs/METADATA.md` - Especificación de campos
- 📁 **Categorías**: `docs/CATEGORIES.md` - Categorías autorizadas

---

## 📝 Convenciones

### Naming
- **Herramientas**: `nombre-herramienta.md` (slug minúsculas con guiones)
- **Noticias**: `YYYY-MM-DD-titulo-noticia.md` (fecha ISO + slug)
- **Tutoriales**: `nombre-tutorial.md` (slug minúsculas con guiones)
- **Imágenes**:
  - Tools: `/images/tools/slug-logo.[ext]`
  - News: `/images/news/YYYY-MM-DD-slug.[ext]`
  - Tutorials: `/images/tutorials/slug-descripcion.[ext]`

### Formato
- **Fechas**: `YYYY-MM-DD` (ISO 8601)
- **Tags**: Title Case Con Espacios (ej: `["IA", "PyMEs", "Marketing"]`)
- **Categorías**: `minusculas-con-guiones` (ej: `marketing-digital`)
- **URLs**: Siempre con `https://`

### Frontmatter
Ver `docs/METADATA.md` para especificación completa de campos.

**Campos obligatorios comunes**:
- `title`, `description`, `publishDate`, `tags`, `category`, `featured`

**Específicos por tipo**:
- **Herramientas**: `logo`, `website`, `pricing`, `difficulty`, `roi_estimate`, `languages`
- **Noticias**: `author`, `image`, `readTime`, `impact`
- **Tutoriales**: `duration`, `difficulty`, `tools_needed`, `outcome`, `steps`

---

## 📊 Estado Actual

- **Herramientas**: 19 documentadas
- **Noticias**: 10 publicadas
- **Tutoriales**: 1 disponible
- **Formato**: ✅ 100% estandarizado
- **Rutas de imágenes**: ✅ 100% correctas

### Categorías Disponibles

**Herramientas**: `productividad`, `marketing-digital`, `atencion-cliente`, `ventas`, `analisis`, `comunicacion`, `operaciones`, `finanzas`, `recursos-humanos`, `diseno`, `automatizacion`

**Noticias**: `tecnologia-ia`, `marketing`, `atencion-cliente`, `productividad`, `recursos-humanos`, `finanzas`, `gobierno-digital`, `diseno`

---

## 🤝 Cómo Contribuir

1. **Lee la documentación**:
   - `docs/TAGS.md` - Para usar tags correctos
   - `docs/METADATA.md` - Para campos obligatorios
   - `docs/CATEGORIES.md` - Para elegir categoría correcta

2. **Usa los templates**: Siempre partir de `/templates/`

3. **Sigue las convenciones**: Naming, formato de fechas, capitalización

4. **Valida tu contenido**:
   ```bash
   # Verificar que no hay rutas incorrectas
   grep -r "/images/herramientas/" --include="*.md"  # No debe retornar nada

   # Verificar formato de tags
   grep "tags:" tu-archivo.md  # Deben estar en Title Case
   ```

5. **Commit y PR**: Usa mensajes descriptivos

---

## 🔧 Comandos Útiles

### Validación

```bash
# Listar todas las categorías usadas
grep "^category:" tools/*.md news/*.md | cut -d'"' -f2 | sort | uniq

# Listar todos los tags únicos
grep "^tags:" tools/*.md news/*.md | sort | uniq

# Verificar imágenes faltantes
find . -name "*.md" -exec grep -l "!\[.*\](.*/images/.*)" {} \; | while read f; do echo "=== $f ==="; grep "!\[.*\](.*/images/.*)" "$f"; done

# Contar contenido por tipo
echo "Herramientas: $(ls tools/*.md | wc -l)"
echo "Noticias: $(ls news/*.md | wc -l)"
echo "Tutoriales: $(ls tutorials/*.md | wc -l)"
```

### Búsqueda

```bash
# Buscar herramientas por categoría
grep "category: \"productividad\"" tools/*.md

# Buscar por tag
grep -l "\"IA\"" tools/*.md news/*.md

# Buscar por fecha
ls news/2025-01-*.md
```

---

## 📚 Documentación Adicional

- **TAGS.md**: Taxonomía completa de tags, ejemplos y guías
- **METADATA.md**: Especificación técnica de todos los campos
- **CATEGORIES.md**: Categorías autorizadas con criterios de selección
- **IMAGE_AUDIT.md**: Auditoría de rutas de imágenes y correcciones aplicadas
- **CONTRIBUTING.md**: Guía de contribución completa

---

## 🔗 Enlaces Relacionados

- **Sitio Web**: [iaparatudia.com](https://iaparatudia.com)
- **Repositorio Web**: [iaparatudia-web](../iaparatudia-web)
- **Agentes de IA**: [iaparatudia-agent](../iaparatudia-agent)
- **Documentación del Proyecto**: [CLAUDE.md](../CLAUDE.md)

---

## 📈 Métricas de Calidad

| Métrica | Estado |
|---------|--------|
| Formato consistente | ✅ 100% |
| Rutas de imágenes correctas | ✅ 100% |
| Templates documentados | ✅ 3/3 |
| Documentación completa | ✅ Sí |
| Tags estandarizados | ✅ Sí |

---

## ⚠️ Notas Importantes

### Imágenes
- **SIEMPRE** usar `/images/tools/`, NO `/images/herramientas/`
- **SIEMPRE** usar `/images/tutorials/`, NO `/images/tutoriales/`
- Verificar que las imágenes existan antes de referenciarlas
- Preferir `.png` para logos con transparencia

### Tags
- Usar Title Case (Primera Letra Mayúscula)
- Separar con espacios, NO guiones
- 3-6 tags por contenido
- Ver `docs/TAGS.md` para lista completa

### Categorías
- Solo UNA categoría por contenido
- Usar la más específica
- Ver `docs/CATEGORIES.md` para guías de decisión

---

## 🆘 Soporte

¿Tienes dudas sobre formato o convenciones?

1. Revisa los templates en `/templates/`
2. Consulta la documentación en `/docs/`
3. Mira ejemplos existentes en `/tools/` o `/news/`
4. Lee `CLAUDE.md` en la raíz del proyecto para contexto completo

---

**Última actualización**: 2025-10-13
**Mantenido por**: Equipo iaparatudia
