# Arquitectura del proyecto
## 1. Objetivo

Documentar la arquitectura técnica y el flujo de procesamiento de datos del proyecto integrador de análisis de perfumes, utilizando Python, SQL y Power BI.

El proyecto comprende la exploración, limpieza, almacenamiento, análisis estadístico, modelado predictivo y visualización de datos relacionados con perfumes, clientes y operaciones de venta.

## 2. Flujo general de procesamiento

El procesamiento se organiza en cinco etapas principales:

1. **Fuentes de datos:** obtención de datasets y otras fuentes de información.
2. **Python — Exploración y preparación:** análisis exploratorio (EDA), evaluación de calidad, limpieza y transformación de los datos.
3. **SQL — Almacenamiento y análisis:** carga de datos procesados en una base relacional, consultas, relaciones entre tablas, agregaciones y análisis de negocio.
4. **Python — Análisis avanzado:** recuperación de datos desde SQL, análisis estadístico, visualizaciones y desarrollo y evaluación de modelos predictivos cuando corresponda.
5. **Power BI — Visualización:** construcción de dashboards e indicadores para comunicar los resultados.

El flujo no es estrictamente lineal: las etapas pueden retroalimentarse cuando sea necesario realizar nuevas consultas, validar resultados o ajustar transformaciones.

Google Drive se utilizará para compartir los archivos de datos y GitHub para versionar el código fuente, los scripts SQL y la documentación.

## 3. Componentes tecnológicos

### 3.1. Fuentes de datos

El proyecto utilizará datasets y/o APIs que proporcionen información sobre perfumes, sus características, clientes y operaciones de venta.

Las fuentes definitivas se documentarán una vez seleccionadas y evaluadas.

### 3.2. Python — Exploración y preparación de datos

Se utilizará Python en Google Colab, principalmente con la biblioteca Pandas, para realizar:

- Carga e inspección inicial de datasets.
- Análisis exploratorio de datos (EDA).
- Análisis descriptivo preliminar.
- Identificación de valores nulos, duplicados e inconsistencias.
- Limpieza, normalización y transformación de variables.
- Validación de la calidad de los datos procesados.
- Preparación de los datos para su carga en la base de datos relacional.

### 3.3. Base de datos SQL

Se utilizará una base de datos relacional para almacenar los datos procesados y continuar el análisis mediante consultas SQL.

Sus principales responsabilidades serán:

- Almacenar la información en tablas relacionadas.
- Definir claves primarias, claves foráneas y restricciones de integridad.
- Realizar consultas utilizando filtros, JOIN, agrupaciones y funciones de agregación.
- Calcular indicadores y métricas de análisis.
- Generar conjuntos de resultados que puedan utilizarse en análisis posteriores.

El motor de base de datos y su modalidad de alojamiento se encuentran pendientes de definición.

### 3.4. Python — Análisis estadístico y predictivo

En una segunda etapa, Python se utilizará para profundizar el análisis a partir de los datos almacenados en SQL.

Las actividades previstas incluyen:

- Recuperación de información desde la base de datos.
- Análisis estadístico descriptivo e inferencial, cuando corresponda.
- Estudio de relaciones entre variables.
- Construcción de gráficos y visualizaciones.
- Desarrollo, entrenamiento y evaluación de modelos predictivos, según los objetivos del proyecto y la disponibilidad de datos adecuados.

### 3.5. Power BI — Visualización y comunicación

Power BI se utilizará para construir dashboards interactivos que permitan presentar los resultados del análisis.

Sus responsabilidades incluirán:

- Definición de indicadores clave (KPIs).
- Construcción de gráficos y visualizaciones interactivas.
- Aplicación de filtros y segmentaciones.
- Presentación de hallazgos y conclusiones relevantes.

### 3.6. Google Drive — Almacenamiento compartido

Google Drive será el espacio compartido para almacenar los datasets originales y procesados.

Los archivos originales deberán conservarse sin modificaciones para garantizar la trazabilidad y reproducibilidad del procesamiento.

### 3.7. GitHub — Control de versiones y colaboración

GitHub será el repositorio oficial del código fuente y la documentación del proyecto.

Permitirá versionar notebooks Jupyter, scripts Python, consultas SQL y documentos técnicos, además de coordinar el trabajo de los integrantes mediante ramas y pull requests.

## 4. Organización del almacenamiento

El proyecto utilizará distintos espacios de almacenamiento según la naturaleza de los archivos.

### 4.1. Google Drive

Se utilizará para almacenar y compartir:

- Datasets originales, sin modificaciones.
- Datasets procesados y validados.
- Archivos de datos intermedios que sea necesario conservar.

Se establecerá una estructura de carpetas común para los integrantes del equipo.

### 4.2. Base de datos SQL

Almacenará los datos estructurados en tablas relacionadas, con sus respectivas claves y restricciones de integridad.

La base de datos será utilizada para realizar consultas analíticas y recuperar información desde Python y, si se define conveniente, desde Power BI.

### 4.3. GitHub

Almacenará y versionará:

- Notebooks Jupyter (`notebooks/`).
- Módulos y funciones Python (`src/`).
- Scripts SQL (`sql/`).
- Documentación técnica (`docs/`).
- Archivos del proyecto Power BI que se decida versionar (`powerbi/`).
- Pruebas y validaciones (`tests/`).

Los datasets originales y las credenciales no se incorporarán al repositorio.

## 5. Integración entre componentes

### 5.1. Fuentes de datos → Python

Los datasets se cargarán en Google Colab desde las fuentes seleccionadas o desde Google Drive.

Python realizará la exploración, limpieza y preparación de la información.

### 5.2. Python → SQL

Los datos procesados y validados se cargarán en las tablas de la base de datos relacional.

El procedimiento de carga, las bibliotecas de conexión y las credenciales se definirán una vez seleccionado el motor SQL y su alojamiento.

### 5.3. SQL → Python

Python recuperará datos de la base relacional para realizar análisis estadísticos, visualizaciones y modelos predictivos.

Se procurará reutilizar consultas SQL y funciones Python para facilitar el mantenimiento del proyecto.

### 5.4. Datos analíticos → Power BI

Power BI utilizará los conjuntos de datos preparados para construir los dashboards.

La modalidad de conexión, ya sea directamente a SQL o mediante archivos exportados, se definirá según la infraestructura disponible y los requisitos del proyecto.

## 6. Reproducibilidad y buenas prácticas

El proyecto deberá permitir que cualquier integrante autorizado pueda reproducir el procesamiento y los análisis.

Para ello, se establecerán las siguientes prácticas:

1. Conservar los datasets originales sin modificaciones.
2. Documentar las fuentes de datos utilizadas.
3. Registrar las transformaciones aplicadas durante la limpieza.
4. Versionar los notebooks, scripts y consultas SQL.
5. Documentar las dependencias y configuraciones necesarias.
6. Evitar rutas absolutas específicas de una computadora o cuenta personal.
7. No incorporar contraseñas, tokens ni credenciales al código fuente.
8. Definir un orden de ejecución para los procesos de carga y análisis.
9. Utilizar semillas aleatorias cuando corresponda para favorecer la reproducibilidad de los modelos.
10. Validar que los resultados puedan obtenerse nuevamente a partir de los datos y procedimientos documentados.

## 7. Decisiones técnicas pendientes

Las siguientes decisiones se resolverán durante el desarrollo:

- Selección definitiva de las fuentes de datos.
- Selección del motor y alojamiento de la base de datos SQL.
- Definición del modelo relacional.
- Configuración de conexiones entre Google Colab y SQL.
- Definición de la estrategia de conexión con Power BI.
- Selección de técnicas estadísticas y modelos predictivos.
- Definición de la estructura compartida de Google Drive.

Las decisiones aprobadas deberán registrarse en `02_decisiones_tecnicas.md` y reflejarse en este documento cuando afecten la arquitectura.
