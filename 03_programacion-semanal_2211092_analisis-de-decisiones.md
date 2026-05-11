### Programación Semanal de la UEA Análisis de Decisiones (Teoría)
### Licenciatura en Administración — Unidad Iztapalapa

**Clave:** 2211092 | **Trimestre:** 2026-P | **Sesiones:** Lunes y Miércoles, 14:00–16:00 h  
**Periodo:** 6 de mayo – 22 de julio de 2026 | **Salón:** Anexo A-Sala K  
**Profesor:** Dr. Jesús Zavala Ruiz | **Asesorías:** Martes 20:00–22:00 h vía Telegram (previa solicitud)

---

#### I. Estructura General del Trimestre

| Semana | Fechas | Sesión | Tema Central | Actividades Principales | Entregables |
|--------|--------|--------|-------------|------------------------|-------------|
| **1** | 6–8 may | 1 | Presentación del curso. Fundamentos históricos de la Investigación de Operaciones. Elementos de un acto de decisión. | - Encuadre administrativo y académico<br>- Lectura guiada: Rangel (2012), pp. 11-13<br>- Activación de cuentas institucionales | - Práctica 0.1: Configuración de entorno (R, RStudio, RMarkdown) |
| | | 2 | Matriz de pagos y concepto de dominación. Tipología de problemas de decisión. | - Ejercicio manual: construcción de matriz de pagos (Ej. 1, Rangel)<br>- Introducción a estructuras de datos en R para decisiones | - Práctica 1.1: Primer reporte en RMarkdown (transcripción Ej. 1) |
| **2** | 13–15 may | 3 | Metodología de estructuración de problemas de decisión. Encuadre sistemático. | - Taller: aplicación del "machote" de encuadre a casos administrativos<br>- Discusión: certeza vs. incertidumbre | - Tarea 2.1: Encuadre manual de 3 problemas (cuaderno) |
| | | 15 may | 4 | Implementación computacional de la estructuración. Introducción a funciones en R. | - Práctica guiada: codificación de matriz de pagos en R<br>- Depuración básica y generación de reportes | - Práctica 2.1: Archivo *Estructura_1.Rmd* en GitHub |
| **3** | 20–22 may | 5 | Criterios no probabilísticos I: Maximin (Wald) y Maximax. Fundamentos filosóficos. | - Análisis comparativo de actitudes frente al riesgo<br>- Resolución manual de Ej. 2 (Rangel, pp. 18-21) | - Tarea 3.1: Síntesis conceptual + glosario Unidad 2 |
| | | 22 may | 6 | Criterios no probabilísticos II: Hurwicz (índice α) y Savage (minimax regret). | - Cálculo de matriz de pérdida de oportunidad<br>- Práctica: implementación de los cuatro criterios en R | - Práctica 3.1: Script *Criterios_Incertidumbre.Rmd* |
| **4** | 27–29 may | 7 | Integración de criterios bajo incertidumbre. Análisis de dominancia y selección estratégica. | - Caso aplicado: decisión de inversión en PYME<br>- Socialización de dudas en plenaria | - Tarea 3.2: Resolución de Grupo de Ejercicios 2 (Rangel) |
| | | 29 may | 8 | **Evaluación formativa**. Retroalimentación y cierre de Unidad 2. | - **Quiz 1** (15 min, conceptual)<br>- Revisión de prácticas con rúbrica | - Entrega de portafolio parcial (semanas 1-4) |
| **5** | 3–5 jun | 9 | Criterios probabilísticos I: Laplace y Máxima Posibilidad. Distribuciones a priori. | - Construcción de distribuciones subjetivas<br>- Ejercicio: asignación de probabilidades a estados de la naturaleza | - Tarea 4.1: Ejercicios de probabilidad subjetiva |
| | | 5 jun | 10 | Regla de Bayes (VEM) y Pérdida de Oportunidad Esperada (POE). | - Cálculo manual y en R del VEM y POE<br>- Verificación: VEM + POE = constante | - Práctica 4.1: *VEM_POE.Rmd* con Ej. 5-6 (Rangel) |
| **6** | 10–12 jun | 11 | Valor Esperado de la Información Perfecta (VEIP): Métodos 1 y 2. Costo de la incertidumbre. | - Cálculo del VEIP como diferencia GEC – VEM<br>- Interpretación administrativa del VEIP | - Tarea 4.2: Cálculo de VEIP en 3 casos aplicados |
| | | 12 jun | 12 | Análisis de sensibilidad: regiones de preferencia y estabilidad de la decisión óptima. | - Graficación de regiones de preferencia en R<br>- Discusión: robustez de la decisión | - Práctica 4.2: *Sensibilidad.Rmd* con gráfica de preferencias |
| **7** | 17–19 jun | 13 | Árboles de decisión: estructura cronológica, nodos y inducción regresiva. | - Construcción manual de árbol (Ej. 9, Rangel)<br>- Identificación de rutas óptimas | - Tarea 5.1: Árbol de decisión dibujado + justificación |
| | | 19 jun | 14 | **PRIMER EXAMEN PARCIAL** (Teórico-Práctico). Implementación de árboles en R. | - **Examen 1** (60 min): conceptos + resolución de problema<br>- Introducción a paquetes `data.tree` o `DiagrammeR` | - Entrega de práctica 5.1: *Arbol_Decision.Rmd* |
| **8** | 24–26 jun | 15 | Decisiones con experimentación: probabilidades a posteriori y Teorema de Bayes. | - Actualización bayesiana con datos muestrales<br>- Ejercicio: urnas (Ej. 11, Rangel) | - Tarea 6.1: Cálculo de probabilidades a posteriori |
| | | 26 jun | 16 | Valor Esperado de la Información Muestral (VEIM). Análisis costo-beneficio de la experimentación. | - Comparación VEIP vs. VEIM<br>- Caso: estudio de mercado con confiabilidad parcial | - Práctica 6.1: *Bayes_Updating.Rmd* |
| **9** | 1–3 jul | 17 | Teoría de la utilidad: función de utilidad del dinero y actitud frente al riesgo. | - Método de Neumann-Morgenstern (EMC)<br>- Construcción de curva de utilidad personalizada | - Tarea 7.1: Determinación de su propia función de utilidad |
| | | 3 jul | 18 | Decisiones secuenciales y análisis en forma extensiva vs. forma normal. | - Resolución de problema multi-etapa (Ej. 16, Rangel)<br>- Comparación metodológica | - **Tarea Integradora**: Caso aplicado a administración pública/privada |
| **10** | 8–10 jul | 19 | Síntesis del curso. Integración de modelos y reflexión epistemológica. | - Presentación de casos integradores (equipos)<br>- Discusión: límites del análisis cuantitativo en decisiones reales | - Entrega de portafolio final (todos los .Rmd + tareas manuales digitalizadas) |
| | | 10 jul | 20 | **SEGUNDO EXAMEN PARCIAL** (Práctico-Computacional). Cierre administrativo. | - **Examen 2** (90 min): resolución de problema completo en RStudio Cloud<br>- Retroalimentación final y orientaciones para evaluación de recuperación | - Encuesta de satisfacción del curso |

#### II. Calendario de Evaluaciones

| Evaluación | Fecha | Modalidad | Ponderación | Contenidos |
|-----------|-------|-----------|-------------|------------|
| **Quiz Formativo 1** | 29 may (S8) | Presencial, 15 min | 5% | Unidades 1-2: conceptos básicos, matriz de pagos, criterios no probabilísticos |
| **Primer Examen Parcial** | 19 jun (S14) | Presencial, 60 min | 35% | Unidades 1-4: estructuración, incertidumbre, riesgo, VEIP, sensibilidad |
| **Segundo Examen Parcial** | 10 jul (S20) | RStudio Cloud, 90 min | 35% | Unidades 5-7: árboles de decisión, experimentación, utilidad, decisiones secuenciales |
| **Tareas y Prácticas** | Continuo | GitHub / Telegram / RStudio Cloud | 25% | 8 tareas manuales + 8 prácticas computacionales (con rúbricas) |
| **TOTAL** | | | **100%** | |

> **Nota sobre Evaluación de Recuperación:**  
> Se aplicará conforme al calendario institucional (última semana de julio). Requisitos: (1) asistencia ≥80%, (2) entrega del portafolio completo, (3) transcripción manual de conceptos y ejercicios de las Unidades 1-3 de Rangel (2012). El examen de recuperación será presencial, de 2 horas, con resolución de 2 problemas de análisis de decisiones con enfoque metodológico explícito.

#### III. Recursos Bibliográficos por Unidad 

| Unidad | Bibliografía Obligatoria | Recursos Complementarios |
|--------|--------------------------|--------------------------|
| **1-2** | Rangel (2012), pp. 11-24 | - Ibiza (2018): Tutorial Google Drive<br>- Boccardo & Ruiz (2019): RMarkdown intro |
| **3-4** | Rangel (2012), pp. 25-54 | - Howard (1988): *Decision analysis: practice and promise*<br>- Wickham: *Advanced R*, cap. 22 (Debugging) |
| **5-6** | Rangel (2012), pp. 55-75 | - Raiffa (1978): *Análisis de la Decisión Empresarial*<br>- Paquete `radiant` para análisis interactivo |
| **7** | Rangel (2012), pp. 76-95 | - Keeney (1982): *Decision Analysis: An overview*<br>- `DiagrammeR` para visualización de árboles |

> **Acceso institucional**: Todos los recursos están disponibles vía Biblioteca Digital UAM (bidi.uam.mx) o mediante enlaces DOI estables. Se priorizan versiones de acceso abierto legítimo.
