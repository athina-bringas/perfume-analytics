# Diccionario de datos
## 1. Objetivo

Documentar la estructura, el significado y las restricciones de los datos utilizados en el proyecto de análisis de perfumes.

Este documento servirá como referencia para las etapas de exploración, limpieza, almacenamiento, análisis estadístico y visualización.

## 2. Estado del modelo de datos

**Estado:** En definición.

El modelo de datos se completará progresivamente a medida que se seleccionen las fuentes, se definan las variables y se diseñe el esquema relacional.

Los nombres de tablas y campos registrados durante esta etapa serán preliminares hasta su validación.

## 3. Criterios de documentación

Para cada campo se registrarán las siguientes propiedades:

- **Campo:** nombre utilizado en el modelo de datos.
- **Tipo de dato:** tipo previsto para su almacenamiento.
- **Descripción:** significado de la variable.
- **Valores permitidos:** dominio o restricciones aplicables.
- **Admite nulos:** indica si puede contener valores faltantes.
- **Origen:** fuente de datos o transformación de la que proviene.
- **Observaciones:** reglas de negocio, validaciones o aclaraciones relevantes.

También se documentarán las claves primarias, claves foráneas y relaciones entre tablas.

## 4. Entidades del modelo

Las entidades preliminares del proyecto incluyen:

- `perfumes`: información y características de los perfumes.
- `customers`: información de los clientes.
- `sales`: operaciones de compra o venta.

La definición definitiva de las entidades y sus relaciones se realizará durante el diseño del modelo relacional.

## 5. Diccionario de campos

**Pendiente:** completar una vez validada la estructura de cada entidad.

## 6. Relaciones entre entidades

**Pendiente:** documentar las claves primarias, claves foráneas y cardinalidades del modelo relacional.

## 7. Reglas de calidad y transformación

**Pendiente:** registrar las reglas de limpieza, normalización, tratamiento de nulos, duplicados y variables derivadas.

## 8. Mantenimiento

El diccionario deberá actualizarse cuando se incorporen, eliminen o modifiquen campos, tipos de datos, restricciones o relaciones.

Los cambios relevantes en el diseño deberán mantenerse consistentes con los scripts SQL y la documentación de arquitectura.
