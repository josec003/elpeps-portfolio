---
Prompt (orig):

Teniendo en cuenta mis líneas de diseño y decisiones técnicas descritas en `project-brief.md` y `project-inspiration.md` (y respetando los tokens de `assets/css/_variables.css`), analiza estos 3 portfolios de ilustradores [- https://generalcondition.com/
- https://rudocompany.com/
- https://www.vicrojo.com/].

## Volcado de entrega (archivos destino)

- `docs/prompt-analisis-galerias.md`: pega este prompt + la respuesta completa.
- `project-inspiration.md`: añade las 3 URLs analizadas y 3 bullets de “patrones transferibles” (sin copiar).
- `project-brief.md`: incorpora 2 decisiones concretas (layout + contenido) en Key Sections / Design Direction.

Objetivo pedagógico: detectar **patrones transferibles** (no copiar estética).

Para cada uno, evalúa:

1. **Diseño Visual (Awwwards criteria)**

   - Estética general (1-10)
   - Tipografía y jerarquía
   - Uso de color y contraste
   - Composición y espaciado

2. **UX de Galería**

   - Facilidad para explorar proyectos
   - Claridad de navegación
   - Información por proyecto (título, descripción, tags)
   - Call-to-actions efectivos

3. **Técnica**

   - Tipo de layout (grid, masonry, custom)
   - Responsive behavior
   - Performance (carga de imágenes)
   - Micro-interactions

4. **Insights Accionables (aplicables a mi brief)**
   - 3 patrones que puedo reutilizar sin copiar (con explicación)
   - 3 riesgos/antipatrones a evitar (con explicación)
   - 2 decisiones concretas para mi galería (layout + contenido), justificadas con mi `project-brief.md`

Devuelve:

- Tabla comparativa (Diseño / UX / Técnica)
- “Decisiones para mi proyecto” (bullets)
- Checklist de verificación (qué revisar al implementarlo)

---

Respuesta (análisis completo):

Resumen ejecutivo
- Sitios analizados: https://generalcondition.com/, https://rudocompany.com/, https://www.vicrojo.com/
- Objetivo: identificar patrones transferibles para una galería de ilustración respetando tus tokens de diseño (`assets/css/_variables.css`) y las decisiones de `project-brief.md`.

1) General Condition (generalcondition.com)

- Diseño Visual (Awwwards criteria)
  - Estética general: 8/10 — lenguaje visual audaz, jerarquía fuerte, uso de tipografía grande y bloques de imagen que funcionan como escenas.
  - Tipografía y jerarquía: Uso de tipografías grandes y contrastadas; jerarquía clara entre proyecto/entrada y descripciones.
  - Uso de color y contraste: predominio de neutros con acentos; contraste alto en CTAs.
  - Composición y espaciado: generoso uso de whitespace; composiciones en bloque que dan protagonismo a cada proyecto.

- UX de Galería
  - Facilidad para explorar: fácil — scroll vertical con proyectos claramente diferenciados; enlaces directos a case studies.
  - Claridad de navegación: navegación simple y centrada en el trabajo; la home actúa como índice visual.
  - Información por proyecto: títulos visibles; a menudo requieren entrar para ver detalle (lo cual prioriza imagen/escena sobre metadatos en el índice).
  - CTAs: claros y directos (enlaces a case studies, premios, contacto).

- Técnica
  - Tipo de layout: grid/stacked personalizado — bloques de ancho variable, módulos apilados.
  - Responsive: adapta contenidos y reordena bloques; imágenes fluidas.
  - Performance: imágenes optimizadas (webp/avif probablemente); carga progresiva visible.
  - Micro-interactions: transiciones suaves en hover, animaciones de entrada discretas.

- Insights accionables (para tu brief)
  - Patrones reutilizables:
    1. Hero-index visual por proyecto (una imagen grande por entrada) para atrapar rápidamente la atención sin saturar.
    2. Entradas que funcionan como “portales” a case studies (thumbnail → entrada detallada), dejando la home limpia.
    3. Jerarquía tipográfica contundente para titulares + descripción breve que invite al clic.
  - Riesgos a evitar:
    1. Priorizar solo estética sobre usabilidad (p. ej. miniaturas crípticas sin contexto).
    2. Imágenes excesivamente pesadas sin lazy-loading o formatos modernos.
    3. Dependencia de animaciones pesadas que rompan rendimiento móvil.

2) Rudo Company (rudocompany.com)

- Diseño Visual (Awwwards criteria)
  - Estética general: 7/10 — estilo experimental y distintivo, pero a veces rudo/caótico intencionalmente.
  - Tipografía y jerarquía: contraste alto; jerarquía variable que refuerza el tono editorial.
  - Uso de color y contraste: paleta sobria con elementos destacados; alto contraste gráfico.
  - Composición y espaciado: apuesta por layouts menos convencionales; riesgo de ruido visual en pantallas pequeñas.

- UX de Galería
  - Facilidad para explorar: interesante para exploración casual; puede ser menos directa para usuarios que buscan un resumen rápido.
  - Claridad de navegación: navegación artística; hay que acostumbrarse.
  - Información por proyecto: títulos presentes pero menos foco en metadatos; la experiencia es muy visual.
  - CTAs: suelen ser implícitos (clic en el proyecto) más que botones explícitos.

- Técnica
  - Tipo de layout: custom/experimental (combinación de grid y elementos superpuestos).
  - Responsive: funciona pero con reordenamientos menos predecibles; cuidado con accesibilidad en navegación por teclado.
  - Performance: mezcla de assets animados y multimedia; revisar lazy-loading y formatos.
  - Micro-interactions: gestos, hover intensos y transiciones creativas.

- Insights accionables
  - Patrones reutilizables:
    1. Composición asimétrica controlada para dar carácter sin perder legibilidad.
    2. Uso deliberado de micro-interacciones experimentales en proyectos destacados.
    3. Presentaciones de proyecto que combinan imagen + fragmentos tipográficos como “teaser”.
  - Riesgos a evitar:
    1. Romper la expectativa de navegación estándar (puede confundir clientes/proveedores).
    2. Animaciones o elementos que no respeten navegación por teclado.
    3. Falta de metadatos visibles (cliente, rol, año) que dificulten la evaluación rápida del work.

3) Vic Rojo (vicrojo.com)

- Diseño Visual (Awwwards criteria)
  - Estética general: 8/10 — fuerte enfoque en imágenes/ilustraciones; tono consistente y cuidado.
  - Tipografía y jerarquía: buena legibilidad; títulos claros con body copy sucinto.
  - Uso de color y contraste: paleta sobria que deja protagonismo a las imágenes; buen contraste en texto.
  - Composición y espaciado: grid fluido con módulos de imagen que escalan bien.

- UX de Galería
  - Facilidad para explorar: muy buena — thumb-to-detail claro; scroll con repetición de enlaces a proyectos.
  - Claridad de navegación: clara; separación entre trabajo y contacto/biografía.
  - Información por proyecto: thumbnails + enlaces a páginas case study con imágenes grandes y slides.
  - CTAs: directos (ver proyecto, contacto, descargar CV).

- Técnica
  - Tipo de layout: grid con sliders/carruseles en interior de proyecto; thumbnails optimizados.
  - Responsive: bien resuelto; imágenes adaptativas y slides móviles.
  - Performance: uso de formatos modernos (webp); lazy-loading probable.
  - Micro-interactions: sliders, hover states, transiciones en galerías.

- Insights accionables
  - Patrones reutilizables:
    1. Miniaturas + página de proyecto con slider para mostrar proceso y resultados.
    2. CTAs de contacto/descarga (CV) visibles y accesibles desde la galería.
    3. Repetición visual del patrón de proyecto (thumbnail consistente) para facilitar el escaneo.
  - Riesgos a evitar:
    1. Crear una galería que obliga a demasiados clics para ver información básica.
    2. Slider sin controles accesibles (p. ej. sin navegación por teclado o indicación de posición).
    3. Falta de fallback para formatos modernos en navegadores antiguos.

Tabla comparativa (Diseño / UX / Técnica)

| Sitio | Diseño (estética, tipografía, color) | UX Galería (explorar, CTA, metadatos) | Técnica (layout, responsive, performance) |
|---|---:|---:|---:|
| General Condition | 8 — Jerarquía fuerte, tipografía expresiva | 8 — Home-index visual, CTAs claros | 8 — Grid personalizado, buenas prácticas de imágenes |
| Rudo Company | 7 — Experimental, tono distintivo | 6 — Exploración creativa, menos directa | 6 — Layout custom, revisar accesibilidad |
| Vic Rojo | 8 — Imagen e ilustración en foco | 8 — Thumbs claros + pages con sliders | 8 — Grid + sliders, optimización de imágenes |

Decisiones para mi proyecto (resumen y justificación con `project-brief.md` y tokens)

- Layout (decisión concreta): adoptar una grid responsiva tipo “thumbnail portal” con hero-index por proyecto — miniatura grande en la rejilla que enlaza a case study con slider. Justificación: combina la claridad de Vic Rojo (scannability) y la teatralidad de General Condition sin copiar estética; encaja con tus objetivos de mostrar ilustración y procesos. Técnica: usar `--max-width`, `--container-padding` y las variables de tipografía para mantener consistencia.

- Contenido (decisión concreta): cada tarjeta de proyecto incluirá: título (H3), rol/servicio (meta breve), año, 1–2 tags y un teaser de 1–2 frases; la página de proyecto tendrá un slider de imágenes, una breve descripción y créditos. Justificación: equilibra imagen y metadatos (evita el antipatrón de “belleza sin contexto”) y responde a tus métricas de accesibilidad y performance en `project-brief.md`.

Checklist de verificación (qué revisar al implementarlo)

- Estructura & accesibilidad:
  - [ ] HTML semántico para la grid y artículos (`<main>`, `<section>`, `<article>`).
  - [ ] Encabezados jerárquicos correctos (H1 página → H2 secciones → H3 proyectos).
  - [ ] Navegación por teclado comprobada (tabindex, focus states visibles).

- Imágenes & performance:
  - [ ] Usar `picture` + `source` con `type=webp`/`avif` y `img` fallback.
  - [ ] Lazy-loading (`loading="lazy"`) y placeholder LQIP o blur-up.
  - [ ] Comprimir y servir imágenes responsive (srcset) según breakpoints.

- Visual & tokens:
  - [ ] Usar `--max-width`, `--container-padding`, y escala tipográfica (`--font-size-*`) para coherencia.
  - [ ] Colores de acento con `--color-primary` y estados con `--color-primary-hover`.
  - [ ] Espaciados consistentes con variables `--space-*`.

- Interacciones:
  - [ ] Micro-interactions ligeras (transiciones <= `--transition-base`).
  - [ ] Controles accesibles en sliders (botones, indicadores, aria-labels).
  - [ ] Animaciones condicionales (prefers-reduced-motion).

- Contenido & UX:
  - [ ] Cada proyecto tiene título, rol/cliente, tags y CTA claro.
  - [ ] Detalle de proyecto con navegación clara y posibilidad de volver al índice.
  - [ ] CTAs de contacto/descarga visibles desde la galería.

Notas finales
- 3 patrones transferibles (sin copiar estética): hero-index visual por proyecto; thumbnail-to-case-study; tarjetas con metadatos mínimos.
- 3 riesgos a evitar: sacrificar claridad por experimentación extrema; imágenes no optimizadas; sliders no accesibles.
- 2 decisiones concretas (layout + contenido) ya integradas arriba y justificadas con las prioridades técnicas de `project-brief.md`.

---

Fin del análisis.
