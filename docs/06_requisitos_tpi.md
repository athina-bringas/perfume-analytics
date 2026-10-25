# Requisitos del Trabajo Práctico Integrador
## 1. Objetivo y fuentes

Este documento reúne los requisitos académicos, los entregables, los criterios de evaluación y las condiciones de presentación del Trabajo Práctico Integrador (TPI) del bootcamp de Análisis de Datos.

**Fuentes de referencia:**
- `Pautas TPI.pdf`: pautas oficiales, entregables y rúbrica de evaluación.
- `Pautas PI – Resumen Clase.pdf`: indicaciones y aclaraciones brindadas durante la clase.
- Apuntes personales de clase: información complementaria sobre entrega y certificación.

## 2. Características generales del TPI

- **Modalidad:** trabajo grupal de tres integrantes.
- **Temática elegida:** análisis de datos del universo de perfumes.
- **Herramientas seleccionadas:** Python, SQL y Power BI.
- **Alcance:** problemática concreta, objetivos definidos y dimensión realizable dentro del plazo disponible.

La formación permite seleccionar herramientas según las características del proyecto. Aunque se recomienda concentrarse en dos cuando el tiempo o los conocimientos son limitados, nuestro equipo utilizará las tres, por lo que deberá cumplir con los entregables correspondientes.

## 3. Entregables obligatorios

### 3.1. Informe técnico (PDF)

Documento que explique el desarrollo técnico completo del proyecto, incluyendo:

- Problemática, contexto y objetivos.
- Fuentes de datos y procedimientos de extracción, incluidas las conexiones a APIs cuando corresponda.
- Exploración, limpieza, transformaciones y funciones implementadas en Python.
- Diseño de la base de datos, carga de información y consultas SQL.
- Integración y flujo de datos entre herramientas.
- Modelado, transformaciones, medidas DAX y visualizaciones en Power BI.
- Análisis estadísticos o predictivos realizados, si corresponde.
- Resultados, interpretación, conclusiones y recomendaciones.

Debe explicar los procedimientos y decisiones técnicas que sustentan el análisis, de manera que el trabajo pueda comprenderse y reproducirse.

### 3.2. Presentación de resultados

Presentación en PowerPoint o Google Slides orientada a negocio o cliente, centrada en:

- Problemática y objetivos.
- Principales hallazgos.
- Conclusiones.
- Recomendaciones y posibles mejoras.

Debe priorizar el valor de los resultados por encima del detalle técnico.

### 3.3. Código fuente y archivos técnicos

| Herramienta | Entregable | Contenido |
|---|---|---|
| SQL | `ddl.sql` | Estructura de la base de datos mediante `CREATE TABLE`, sin sentencias `INSERT`. |
| SQL | `analisis.sql` | Consultas y scripts de exploración, limpieza y análisis. |
| Python | `.ipynb` | Notebooks estructurados, documentados y con buenas prácticas, incluyendo funciones reutilizables. |
| Power BI | `dashboard.pbix` | Proyecto de Power BI con el modelo y los dashboards. |
| Power BI | PDF de medidas DAX | Listado de medidas y fórmulas utilizadas. |

Se podrá utilizar Google Colab para desarrollar los notebooks de Python.

### 3.4. Video de presentación

Video de **10 a 15 minutos**, utilizando la presentación como soporte, que explique:

- Problemática y objetivos.
- Metodología y herramientas.
- Resultados principales.
- Conclusiones y recomendaciones.

## 4. Criterios de evaluación

La evaluación se realizará según la rúbrica oficial de `Pautas TPI.pdf`.

### 4.1. Ponderaciones

| Dimensión | Peso |
|---|---:|
| Calidad del análisis | 25 % |
| Originalidad y creatividad | 10 % |
| Presentación y documentación | 10 % |
| Código y replicabilidad | 10 % |
| Integración de herramientas | 15 % |
| Comunicación y entrega | 15 % |
| Dominio técnico | 15 % |
| **Total** | **100 %** |

### 4.2. Escala de evaluación

Cada criterio contempla tres niveles: **Excelente (3 puntos)**, **Bueno (2 puntos)** y **Necesita mejorar (1 punto)**.

| Calificación final | Nivel |
|---|---|
| ≥ 8,50 | Excelente |
| ≥ 7,00 | Bueno |
| ≥ 6,00 | Aprobado |
| Menor a 6,00 | Necesita mejorar |

### 4.3. Criterios para alcanzar el nivel Excelente

**Calidad del análisis (25 %)**
- Interpretar los datos y extraer conclusiones significativas relacionadas con el contexto.
- Resolver problemas mediante razonamiento estructurado, evaluación de alternativas y justificación de soluciones.

**Originalidad y creatividad (10 %)**
- Proponer enfoques originales e innovadores.
- Aplicar técnicas avanzadas de manera pertinente y con valor analítico.

**Presentación y documentación (10 %)**
- Organizar y comunicar la información con claridad y coherencia.
- Presentar materiales profesionales, bien estructurados y sin errores.

**Código y replicabilidad (10 %)**
- Desarrollar código limpio, eficiente y con buenas prácticas.
- Documentar el proyecto para permitir la reproducción de los resultados.

**Integración de herramientas (15 %)**
- Utilizar Python, SQL y Power BI de manera equilibrada y coherente.
- Garantizar un flujo de datos adecuado y la interoperabilidad entre herramientas.

**Comunicación y entrega (15 %)**
- Realizar una presentación clara, segura, sintética y adaptada a la audiencia.
- Explicar las decisiones, dificultades y aprendizajes del proyecto.

**Dominio técnico (15 %)**
- **Power BI:** modelo de datos adecuado (estrella o similar), relaciones correctas y sin ambigüedades, dashboards relevantes y DAX avanzado.
- **SQL:** consultas analíticas optimizadas, utilizando CTE y funciones de ventana cuando resulten pertinentes.
- **Python:** bibliotecas apropiadas, código modular y eficiente, buenas prácticas y documentación del flujo de trabajo mediante comentarios, README o notebooks.

## 5. Fechas y modalidad de entrega

### 5.1. Fechas

- **Primera entrega:** 19/12/2026.
- **Segunda entrega:** en la próxima edición, con fecha pendiente de confirmación.
- **Zona horaria de referencia:** España.

La prioridad del equipo será realizar la primera entrega. Se deberá confirmar la hora exacta de cierre.

### 5.2. Procedimiento de entrega

La entrega será **asincrónica**. Según las aclaraciones de clase, se deberá:

1. Publicar el proyecto en el foro correspondiente, respetando el formato indicado.
2. Completar el formulario de entrega, uno por grupo.

Se deberán verificar las instrucciones vigentes antes de realizar la presentación.

### 5.3. Corrección y devolución

La devolución se realizará dentro de las tres semanas posteriores al cierre de entrega de la edición correspondiente e incluirá la evaluación detallada y la calificación final.

Los trabajos entregados fuera de plazo serán corregidos en la siguiente edición, según las pautas oficiales.

## 6. Requisitos de certificación

Para obtener el certificado del bootcamp se requiere:

1. **Entregar y aprobar el TPI.**
2. **Completar al menos el 90 % del contenido obligatorio** de la plataforma.

El proyecto puede entregarse antes de alcanzar el 90 % de avance; los contenidos pendientes podrán completarse posteriormente dentro del período de acceso.

Según los apuntes de clase, el acceso al contenido es de **dos años**. Se deberá verificar la vigencia correspondiente a cada integrante.

## 7. Checklist final de entrega

### 7.1. Documentación y presentación

- [ ] Informe técnico completo en PDF.
- [ ] Presentación de resultados orientada a negocio.
- [ ] Video de presentación de 10 a 15 minutos.

### 7.2. Código y archivos técnicos

- [ ] `ddl.sql` con sentencias `CREATE TABLE` y sin `INSERT`.
- [ ] `analisis.sql` con los scripts y consultas de análisis.
- [ ] Notebooks Python `.ipynb` organizados y documentados.
- [ ] `dashboard.pbix` funcional.
- [ ] PDF con las medidas y fórmulas DAX.

### 7.3. Calidad y cumplimiento

- [ ] Requisitos y criterios de la rúbrica oficial verificados.
- [ ] Resultados coherentes con los objetivos y las conclusiones.
- [ ] Código, procesamiento e integración de herramientas revisados para facilitar su reproducción.

### 7.4. Presentación final

- [ ] Fecha y hora límite confirmadas.
- [ ] Archivos finales completos, accesibles y verificados.
- [ ] Publicación realizada en el foro correspondiente.
- [ ] Formulario grupal completado.
- [ ] Entrega registrada correctamente.
