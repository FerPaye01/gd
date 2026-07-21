# 📊 Plan: Conversión del Curso "Gobierno de Datos" a Diapositivas PowerPoint

> **Curso:** Data Power: Impulsando Osinergmin con la Gobernanza de Datos  
> **Institución:** Universidad Corporativa Osinergmin  
> **Autor del plan:** Oficina de Gobierno de Datos  
> **Fecha:** Julio 2026  
> **Estado:** 🟡 En planificación

---

## 🎯 Objetivo

Convertir el contenido interactivo del reproductor SCORM HTML (`03-reproductor-curso.html`) en **6 presentaciones PowerPoint** (`.pptx`), una por cada módulo, listas para ser usadas en capacitaciones presenciales, virtuales síncronas o como material de consulta imprimible.

---

## 📐 Decisiones de Diseño

| Parámetro | Decisión |
|-----------|----------|
| **Formato** | `.pptx` (Microsoft PowerPoint / compatible Google Slides) |
| **Relación de aspecto** | 16:9 (widescreen) |
| **Paleta de colores** | Azul oscuro institucional (`#091e42` → `#1e40af`) + acentos verdes y cyan |
| **Tipografía** | Inter / Calibri (fallback) |
| **Fondo base** | Gradiente oscuro azul-marino (igual al reproductor HTML) |
| **Generación** | Script Python con `python-pptx` |
| **Archivos de salida** | Carpeta `diapositivas/` en la raíz del proyecto |

---

## 🗂️ Estructura de Archivos de Salida

```
gobierno-datos-curso-v-preliminar/
└── diapositivas/
    ├── Modulo-01-Fundamentos-y-Marco.pptx
    ├── Modulo-02-Roles-y-Responsabilidades.pptx
    ├── Modulo-03-Arquitectura-e-Interoperabilidad.pptx
    ├── Modulo-04-Gestion-de-la-Calidad.pptx
    ├── Modulo-05-Metadatos-y-Trazabilidad.pptx
    └── Modulo-06-Seguridad-y-Etica-del-Dato.pptx
```

---

## 📋 Inventario de Contenido por Módulo

### Módulo 1 — Fundamentos y Marco de Gobierno de Datos

**Título SCORM:** `1.1. Introducción al Gobierno de Datos`  
**Total de slides en HTML:** 11  

| # | Tipo | Título de la diapositiva |
|---|------|--------------------------|
| 1 | Portada (Welcome) | Gobierno de Datos — Introducción y Marco de Trabajo |
| 2 | Intro | Módulo 1: Fundamentos y Marco de Gobierno de Datos en el Estado Peruano |
| 3 | Contenido | Valor Público: Beneficios del Gobierno de Datos |
| 4 | Contenido | El Cambio de Paradigma: De "Archivo" a "Activo" |
| 5 | Contenido | Marco Legal y Plataformas del Estado (DL 1412, PIDE, PNDA, GeoPerú) |
| 6 | Contenido | Del Caos a la Sinfonía (metáfora del director de orquesta) |
| 7 | Contenido | Confianza en las Decisiones |
| 8 | Contenido | El Ecosistema del Estado (engranajes) |
| 9 | Ejercicio | Ejercicio 1: El Rompecabezas del Ecosistema (drag & drop → tabla estática) |
| 10 | Ejercicio | Ejercicio 2: Beneficios del Gobierno de Datos (fill-in → completar párrafo) |
| 11 | Ejercicio | Ejercicio 3: Caso Práctico — Decisión Estratégica (aventura) |
| 12 | Cierre | ¡Felicitaciones! Has completado la actividad 1.1 |

**Conceptos clave a mantener:**
- Datos como activo estratégico vs. residuo administrativo
- DL N° 1412 (Ley de Gobierno Digital)
- Estrategia Nacional 2026-2030 (madurez nivel 4)
- PIDE / PNDA / GeoPerú
- Fuente Única de Verdad (SSOT)

---

### Módulo 2 — Roles y Responsabilidades

**Título SCORM:** `2.1. El Ecosistema Humano`  
**Total de slides en HTML:** ~10  

| # | Tipo | Título de la diapositiva |
|---|------|--------------------------|
| 1 | Portada | Gobierno de Datos — El Ecosistema Humano: Roles y Responsabilidades |
| 2 | Intro | Módulo 2: Roles, Responsabilidades y Modelos Operativos |
| 3 | Contenido | La Cadena de Suministro del Dato — 8 Roles Oficiales (PI-59) |
| 4 | Contenido | Roles de Negocio y Estrategia (Alta Dirección, OGD, Líder del Dato, Dueño) |
| 5 | Contenido | Roles Técnicos y de Soporte (Steward, Custodio, BI/Analítica, Usuario) |
| 6 | Contenido | El OGD y la Gobernanza No Invasiva (Robert Seiner) |
| 7 | Contenido | ¿Quién cocina nuestros datos? (flujo Granja → Transporte → Mesa) |
| 8 | Contenido | El Oficial de Gobierno de Datos y el Comité (Res. SGTD 001-2022 y 002-2023) |
| 9 | Contenido | Referencia de Roles — Diagrama Org Chart |
| 10 | Ejercicio | Ejercicios (matching de roles + caso práctico) |
| 11 | Cierre | ¡Felicitaciones! Has completado la actividad 2.1 |

**Conceptos clave a mantener:**
- 8 roles según PI-59 de Osinergmin
- Gobernanza No Invasiva (formalizar lo que ya haces)
- Res. SGTD N° 001-2022 y 002-2023-PCM
- Síndrome de la "Propiedad Difusa"
- Analogía gastronómica (Granja → Transporte → Mesa)

---

### Módulo 3 — Arquitectura e Interoperabilidad

**Título SCORM:** `3.1. Arquitectura de Plataformas`  
**Total de slides en HTML:** ~10  

| # | Tipo | Título de la diapositiva |
|---|------|--------------------------|
| 1 | Portada | Gobierno de Datos — Arquitectura, Plataformas e Interoperabilidad |
| 2 | Intro | Módulo 3: La Caja de Herramientas y Refinamiento de Datos |
| 3 | Contenido | Construyendo las Tuberías — DL N° 1246 y el Principio "Una Sola Vez" |
| 4 | Contenido | La Pirámide de Refinamiento (Capa Bronce / Plata / Oro) |
| 5 | Contenido | Los Enfoques de Implementación (Top-Down / Bottom-Up / Colaborativo) |
| 6 | Contenido | El Ciclo de Vida del Dato (PI-59) y la Deuda Técnica |
| 7 | Contenido | Interoperabilidad (PIDE) y el Fin del "Mensajero No Remunerado" |
| 8 | Contenido | Arquitectura de Apertura — PNDA y GeoPerú |
| 9 | Ejercicio | Ejercicio 1: Ordenando la Caja de Herramientas |
| 10 | Ejercicio | Ejercicio 2: Enfoques y Capas de Refinamiento |
| 11 | Ejercicio | Ejercicio 3: Caso Práctico — Decisión Arquitectónica |
| 12 | Cierre | ¡Felicitaciones! Has completado la actividad 3.1 |

**Conceptos clave a mantener:**
- DL N° 1246 (principio "Una Sola Vez")
- PIDE / PNDA / GeoPerú (detalles técnicos)
- Capa Bronce / Plata / Oro (PI-59)
- Glosario / Diccionario / Catálogo / Linaje de datos
- Hub-and-Spoke (DAMA-DMBOK2)
- Datos Maestros: DNI (RENIEC), RUC (SUNAT), Ubigeo (INEI)
- Estrategia "Remodelar la casa sin mudarse" (sistemas legacy + APIs)

---

### Módulo 4 — Gestión de la Calidad del Dato

**Título SCORM:** `4.1. Dimensiones de Calidad`  
**Total de slides en HTML:** ~9  

| # | Tipo | Título de la diapositiva |
|---|------|--------------------------|
| 1 | Portada | Gobierno de Datos — Gestión de la Calidad del Dato |
| 2 | Intro | Módulo 4: Dimensiones de Calidad y Reglas de Negocio |
| 3 | Contenido | Las 6 Dimensiones de Calidad del Dato (DAMA-DMBOK2) |
| 4 | Contenido | Exactitud / Completitud / Consistencia |
| 5 | Contenido | Oportunidad / Unicidad / Validez |
| 6 | Contenido | Reglas de Calidad y Perfiles de Datos |
| 7 | Contenido | El Ciclo de Mejora Continua de la Calidad |
| 8 | Ejercicio | Ejercicios de calidad del dato |
| 9 | Cierre | ¡Felicitaciones! Has completado la actividad 4.1 |

**Conceptos clave a mantener:**
- 6 dimensiones de calidad (DAMA-DMBOK2)
- Reglas de negocio como validaciones
- Perfilado de datos (data profiling)
- Ciclo de mejora continua

---

### Módulo 5 — Seguridad y Ética

**Título SCORM:** `5.1. Uso seguro, responsable y ético de los datos`  
**Total de slides en HTML:** 14  

| # | Tipo | Título de la diapositiva |
|---|------|--------------------------|
| 1 | Portada | Uso seguro, responsable y ético de los datos |
| 2 | Intro | ¿Qué debo considerar antes de consultar, modificar, compartir o utilizar un dato? |
| 3 | Contenido | Tener acceso no significa poder usar el dato para cualquier finalidad |
| 4 | Contenido | No todos los datos requieren el mismo nivel de protección |
| 5 | Contenido | Antes de utilizar o compartir un dato, verifica |
| 6 | Contenido | Utiliza solo los datos necesarios |
| 7 | Contenido | Prácticas seguras en el trabajo cotidiano |
| 8 | Contenido | Datos personales y privacidad (Ley N° 29733) |
| 9 | Contenido | Ocultar no siempre significa proteger |
| 10 | Contenido | Uso ético de los datos y la inteligencia artificial |
| 11 | Contenido | ¿Qué hago si detecto una exposición o uso inadecuado? |
| 12 | Ejercicio | Actividad: ¿Uso adecuado o situación de riesgo? |
| 13 | Contenido | Caso práctico: compartir con urgencia |
| 14 | Cierre | Ideas clave |

**Conceptos clave a mantener:**
- Condiciones y finalidad del acceso a datos
- Niveles de protección (Público / Uso interno / Restringido / Personal)
- Minimización de datos y prácticas seguras cotidianas
- Protección de datos personales (Ley N° 29733) y uso ético de IA
- Protocolo de reporte de incidentes y seguridad

---

### Módulo 6 — Seguridad y Ética del Dato

**Título SCORM:** `6.1. Anonimización y Privacidad`  
**Total de slides en HTML:** ~9  

| # | Tipo | Título de la diapositiva |
|---|------|--------------------------|
| 1 | Portada | Gobierno de Datos — Seguridad y Ética del Dato |
| 2 | Intro | Módulo 6: Anonimización, Privacidad y Uso Ético de los Datos |
| 3 | Contenido | Marco Legal de Privacidad — Ley N° 29733 (Protección de Datos Personales) |
| 4 | Contenido | Clasificación de la Información (Pública / Reservada / Confidencial) |
| 5 | Contenido | Técnicas de Anonimización y Seudonimización |
| 6 | Contenido | Ética del Dato — Principios para el Uso Responsable |
| 7 | Contenido | Seguridad de la Información en el Marco del Dato Gobernado |
| 8 | Ejercicio | Ejercicios de seguridad y ética |
| 9 | Cierre | ¡Felicitaciones! Has completado el curso completo |

**Conceptos clave a mantener:**
- Ley N° 29733 (Protección de Datos Personales en Perú)
- Anonimización vs. seudonimización
- Clasificación de la información
- Principios éticos en el uso de datos públicos

---

## 🛠️ Plan de Implementación Técnica

### Prerrequisitos

```bash
pip install python-pptx Pillow
```

### Estructura del Script

```
scripts/
├── generar_pptx.py          # Script principal
├── contenido_modulos.py     # Datos de cada diapositiva (extraídos del HTML)
└── estilos.py               # Definición de colores, fuentes y layouts
```

### Diseño de cada Diapositiva PowerPoint

Cada módulo seguirá esta estructura de layouts:

```
┌─────────────────────────────────────────────┐
│  SLIDE 1: PORTADA                           │
│  ┌──────────────────────────────────────┐   │
│  │  [Logo LC | Osinergmin]         [M#] │   │
│  │                                      │   │
│  │     🗄️  GOBIERNO DE DATOS           │   │
│  │     Módulo X: Título del Módulo      │   │
│  │     Subtítulo                        │   │
│  └──────────────────────────────────────┘   │
└─────────────────────────────────────────────┘

┌─────────────────────────────────────────────┐
│  SLIDES DE CONTENIDO                        │
│  ┌──────────────────────────────────────┐   │
│  │  Módulo X | Slide N/Total  [LC Logo] │   │  ← Header
│  │  ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ │   │  ← Línea divisora
│  │                                      │   │
│  │  📌 TÍTULO DE LA DIAPOSITIVA        │   │
│  │                                      │   │
│  │  • Punto 1                           │   │
│  │  • Punto 2                           │   │
│  │  • Punto 3                           │   │
│  │                                      │   │
│  │  [imagen si aplica]                  │   │
│  └──────────────────────────────────────┘   │
└─────────────────────────────────────────────┘

┌─────────────────────────────────────────────┐
│  SLIDES DE EJERCICIO                        │
│  ┌──────────────────────────────────────┐   │
│  │  [Header estándar]                   │   │
│  │  ✏️  EJERCICIO: Nombre               │   │
│  │                                      │   │
│  │  Instrucción: ...                    │   │
│  │                                      │   │
│  │  ┌─────────┐   ┌─────────┐          │   │
│  │  │Opción A │   │Opción B │          │   │
│  │  └─────────┘   └─────────┘          │   │
│  │                                      │   │
│  │  ✅ Respuesta correcta: ...          │   │
│  └──────────────────────────────────────┘   │
└─────────────────────────────────────────────┘
```

### Paleta de Colores (Constantes del Script)

```python
COLORS = {
    "bg_dark":       "091e42",   # Fondo principal (azul muy oscuro)
    "bg_mid":        "1e40af",   # Fondo medio (azul institucional)
    "accent_green":  "10b981",   # Verde esmeralda (acentos positivos)
    "accent_cyan":   "38bdf8",   # Cyan (datos/tecnología)
    "accent_purple": "c084fc",   # Violeta (roles/gobernanza)
    "accent_amber":  "f59e0b",   # Ámbar (advertencias/ejercicios)
    "accent_pink":   "ec4899",   # Rosa (evaluaciones)
    "text_white":    "FFFFFF",   # Texto principal
    "text_muted":    "94a3b8",   # Texto secundario
    "logo_blue":     "3b82f6",   # Azul logo LC/Osinergmin
}
```

---

## 📏 Especificaciones Técnicas del .pptx

| Elemento | Especificación |
|----------|---------------|
| **Tamaño de slide** | 33.87 cm × 19.05 cm (16:9) |
| **Fuente título** | Inter Bold / Calibri Bold, 28–36pt |
| **Fuente cuerpo** | Inter Regular / Calibri, 16–20pt |
| **Fuente subtítulo** | Inter SemiBold / Calibri, 20–24pt |
| **Margen** | 2.5 cm por cada lado |
| **Fondo** | Degradado sólido (usando forma de fondo) |
| **Imágenes** | Copiadas desde `imagenes/modulo-0X/` al .pptx |
| **Script de narración** | Incluido como "Notas del presentador" en cada slide |

---

## ✅ Checklist de Tareas

### Fase 1 — Preparación
- [ ] Instalar `python-pptx` y `Pillow` (`pip install python-pptx Pillow`)
- [ ] Crear carpeta `scripts/` en la raíz del proyecto
- [ ] Crear carpeta `diapositivas/` en la raíz del proyecto
- [ ] Crear archivo `scripts/estilos.py` con paleta de colores y helpers

### Fase 2 — Extracción de Contenido
- [ ] Crear `scripts/contenido_modulos.py` con el contenido textual limpio de cada slide
  - [ ] Módulo 1: extraer títulos, bullets y scripts de narración
  - [ ] Módulo 2: extraer 8 roles + contenido de ejercicios
  - [ ] Módulo 3: extraer arquitectura + capas Bronce/Plata/Oro
  - [ ] Módulo 4: extraer 6 dimensiones de calidad
  - [ ] Módulo 5: extraer tipos de metadatos + linaje
  - [ ] Módulo 6: extraer marco legal + técnicas anonimización

### Fase 3 — Generación del PPTX
- [ ] Crear `scripts/generar_pptx.py` con la lógica principal
- [ ] Implementar función `crear_slide_portada(prs, modulo)`
- [ ] Implementar función `crear_slide_contenido(prs, slide_data)`
- [ ] Implementar función `crear_slide_ejercicio(prs, ejercicio_data)`
- [ ] Implementar función `crear_slide_cierre(prs, modulo)`
- [ ] Implementar inclusión de imágenes desde la carpeta `imagenes/`
- [ ] Agregar scripts de narración como notas del presentador
- [ ] Agregar barra de progreso en el footer de cada slide

### Fase 4 — Revisión y Ajuste
- [ ] Revisar que cada módulo tenga su número correcto de slides
- [ ] Verificar que las imágenes se inserten correctamente
- [ ] Verificar legibilidad del texto (contraste sobre fondo oscuro)
- [ ] Revisar notas del presentador en todos los slides
- [ ] Probar apertura en Microsoft PowerPoint y Google Slides

### Fase 5 — Entrega
- [ ] Guardar los 6 archivos `.pptx` en la carpeta `diapositivas/`
- [ ] Subir los archivos al repositorio de GitHub
- [ ] Documentar instrucciones de uso en este mismo archivo

---

## 📁 Referencias de Contenido

| Archivo fuente | Descripción |
|----------------|-------------|
| [`03-reproductor-curso.html`](./03-reproductor-curso.html) | Fuente principal — contiene los `modulesSlidesData` con todo el contenido HTML |
| [`04-seccion-01-introduccion.html`](./04-seccion-01-introduccion.html) | Introducción del curso: competencia, estructura, familiarización |
| [`05-seccion-02-contenido.html`](./05-seccion-02-contenido.html) | Vista de módulos con tarjetas de actividades |
| [`06-evaluacion.html`](./06-evaluacion.html) | Evaluaciones por módulo (banco de preguntas) |
| `imagenes/modulo-01/` | Imágenes del Módulo 1 (valor-publico.png, activo.png, archivo.png, etc.) |
| `imagenes/modulo-02/` | Imágenes del Módulo 2 |
| `imagenes/modulo-03/` | Imágenes del Módulo 3 (arquitectura-rag.png) |
| `imagenes/modulo-04/` | Imágenes del Módulo 4 |
| `imagenes/modulo-05/` | Imágenes del Módulo 5 |
| `imagenes/modulo-06/` | Imágenes del Módulo 6 |
| `css/theme.css` | Variables CSS del tema (colores, fuentes) |
| `js/` | Scripts JavaScript del reproductor |

---

## 🗓️ Cronograma Estimado

| Fase | Duración estimada | Responsable |
|------|-------------------|-------------|
| Preparación del entorno | 30 min | Dev |
| Extracción de contenido (6 módulos) | 3–4 horas | Dev |
| Generación del script Python | 2–3 horas | Dev |
| Generación de los 6 PPTX | 15 min (automático) | Script |
| Revisión visual de los 6 archivos | 1–2 horas | Revisor |
| Ajustes finales y entrega | 1 hora | Dev |
| **Total estimado** | **~8–10 horas** | |

---

## 📝 Notas Adicionales

1. **Ejercicios interactivos:** Los ejercicios de drag-and-drop y fill-in del HTML se convertirán a slides estáticas mostrando la pregunta + la respuesta correcta marcada (ya que PowerPoint no es interactivo de la misma forma). Para mantener la interactividad en PowerPoint, se podría usar animaciones de "aparecer" en las respuestas.

2. **Scripts de narración:** Todos los textos de `script:` del HTML se copiarán como notas del presentador en cada slide. Esto permitirá usarlas en modo presentador o para producir un audio narrado posteriormente.

3. **Imágenes pesadas:** Las imágenes de la carpeta `imagenes/modulo-01/` son de alta resolución (hasta 6 MB). Se recomienda comprimir con Pillow antes de insertar en el PPTX para mantener el archivo en un tamaño razonable.

4. **Compatibilidad:** Los `.pptx` generados serán compatibles con:
   - Microsoft PowerPoint 2016 o superior
   - Google Slides (importación)
   - LibreOffice Impress

---

*Plan generado el 14 de julio de 2026 — Data Power: Impulsando Osinergmin con la Gobernanza de Datos — Osinergmin*
