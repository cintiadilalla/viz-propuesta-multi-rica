# viz-propuesta-multimetrica
Análisis comparativo de 4 alternativas para visualizar métricas de distinta magnitud en un gráfico de líneas compartido. Desarrollado como parte de un proyecto de diseño de panel comercial.

# Propuesta de visualización para gráfico multimétrica

## Objetivo

Este documento surge durante la validación de la primera versión de un panel de métricas.

El problema identificado estaba en un gráfico de líneas que utilizaba una escala compartida para cinco métricas con magnitudes muy diferentes. Esto provocaba que las métricas de menor volumen quedaran visualmente “aplanadas”, dificultando su lectura e interpretación.

Aunque técnicamente el gráfico era correcto, desde el punto de vista analítico perdía capacidad de comunicación.

El objetivo de esta propuesta fue:

- Analizar alternativas de visualización más adecuadas para métricas heterogéneas.
- Comparar ventajas y limitaciones de cada enfoque.
- Priorizar legibilidad e interpretación sin perder contexto de negocio.
- Transformar una observación de validación en una recomendación concreta y accionable.

La intención no fue únicamente señalar un problema, sino proponer una mejora sustentada visual y conceptualmente.

---

## Datos

Los datos utilizados fueron anonimizados para preservar información sensible de la empresa.

Provienen de bases operativas internas del sistema corporativo y representan métricas de seguimiento comercial y operativo utilizadas en el panel original.

Las métricas incluidas son:

- **Visitas**: volumen de interacciones o consultas registradas.
- **Inmobiliarias**: cantidad de inmobiliarias activas o participantes.
- **Inmobiliarias nuevas**: altas registradas en el período.
- **Referidos**: operaciones o contactos provenientes de derivaciones.
- **Incumplimientos**: eventos asociados a desvíos o incumplimientos registrados.

Los valores fueron mantenidos únicamente con fines demostrativos para reproducir el comportamiento visual del problema original.

---

## Metodología

Se desarrolló un documento interactivo en HTML para comparar distintas estrategias de visualización aplicadas sobre el mismo conjunto de datos.

### Alternativas evaluadas

#### 1. Eje dual
- Separación entre métricas de alto y bajo volumen utilizando dos escalas.
- Permite mantener valores absolutos en un único gráfico.

#### 2. Índice normalizado
- Todas las series parten desde base 100.
- Facilita comparar tendencias y ritmos de cambio independientemente de la magnitud.

#### 3. Small multiples *(opción recomendada)*
- Un mini-gráfico independiente por métrica.
- Cada serie utiliza su propia escala vertical.
- Maximiza legibilidad y evita distorsiones visuales.

#### 4. Sparklines
- Visualización compacta orientada a lectura ejecutiva rápida.
- Prioriza tendencia y valor actual.

### Herramientas utilizadas

- HTML5
- Claude
- GitHub Pages para publicación y distribución

### Criterio de evaluación

Las alternativas fueron comparadas considerando:

- Legibilidad
- Interpretación correcta de tendencias
- Riesgo de ambigüedad visual
- Escalabilidad
- Uso eficiente del espacio
- Facilidad de lectura para distintos perfiles de usuario

---

## Conclusiones

La evaluación mostró que utilizar una escala compartida para métricas con magnitudes muy distintas afecta significativamente la capacidad de interpretación del gráfico.

La alternativa de **Small multiples** fue seleccionada como recomendación principal porque:

- evita el aplanamiento de series,
- mejora la lectura individual de cada métrica,
- reduce ambigüedades visuales,
- y permite aprovechar completamente el espacio de representación de cada serie.

Aunque requiere mayor espacio vertical y vuelve menos inmediata la comparación entre magnitudes absolutas, el beneficio en claridad analítica resulta superior para este caso de uso.

El valor agregado de esta propuesta no estuvo únicamente en identificar una limitación visual, sino en traducir una observación funcional en una mejora concreta de experiencia analítica y comunicación de datos.
