# Manual de colaboración

## 1. Objetivo
Establecer un procedimiento común para que los integrantes del TPI puedan desarrollar, compartir, revisar e integrar cambios utilizando GitHub y Google Colab.

## 2. Herramientas
- **GitHub:** repositorio oficial del código fuente y la documentación.
- **Google Colab:** entorno principal de desarrollo y ejecución de notebooks Python.
- **Google Drive:** almacenamiento compartido de datasets.

## 3. Conceptos básicos de Git y GitHub

| Concepto | Definición |
|---|---|
| Repositorio | Espacio donde se almacenan y versionan los archivos del proyecto. |
| Rama (branch) | Línea independiente de desarrollo. |
| main | Rama principal que contiene la versión estable del proyecto. |
| Commit | Registro de un conjunto de cambios. |
| Push | Envío de commits locales al repositorio remoto. |
| Pull | Obtención e integración de cambios del repositorio remoto en una copia local. |
| Pull request | Solicitud para revisar e integrar cambios de una rama en otra. |
| Merge | Integración de cambios entre ramas. |
| Conflicto | Situación que requiere resolver cambios incompatibles antes de integrarlos. |

## 4. Reglas de colaboración
1. La rama `main` representa la versión oficial y estable.
2. Cada tarea de desarrollo se realiza en una rama independiente creada desde una versión actualizada de `main`.
3. Los cambios se integran mediante pull requests.
4. Antes de integrar, verificar el funcionamiento del código.
5. No modificar simultáneamente el mismo notebook sin coordinación.
6. No subir datasets originales, credenciales ni archivos temporales.
7. Utilizar mensajes de commit claros y consistentes.

## 5. Convención para los commits
Se adopta una versión sencilla de Conventional Commits, con mensajes en español y verbo en modo imperativo.

Formato:

```text
tipo: descripción del cambio
```

Tipos principales:
- `feat`: incorpora una nueva funcionalidad.
- `fix`: corrige un error.
- `docs`: modifica documentación.
- `refactor`: reorganiza código sin modificar su comportamiento.
- `test`: incorpora o modifica pruebas.
- `chore`: tareas de mantenimiento y configuración.

Ejemplos:

```text
docs: agrega manual de colaboración
feat: implementa limpieza de datos
fix: corrige tratamiento de valores nulos
test: agrega pruebas de validación
```

## 6. Flujo general de trabajo
1. Consultar las tareas pendientes y los cambios recientes del proyecto.
2. Crear una rama de trabajo desde una versión actualizada de `main`.
3. Desarrollar los cambios en los archivos correspondientes.
4. Ejecutar y verificar el código.
5. Guardar los cambios mediante commits.
6. Publicar la rama en GitHub.
7. Crear un pull request hacia `main`.
8. Solicitar la revisión de otro integrante.
9. Integrar los cambios aprobados.
10. Crear una nueva rama desde `main` actualizada para la siguiente tarea.

## 7. Organización de archivos
- `notebooks/`: notebooks de extracción, limpieza y análisis.
- `src/`: funciones y módulos Python reutilizables.
- `sql/`: scripts SQL.
- `docs/`: documentación del proyecto.
- `powerbi/`: archivos y documentación de Power BI.
- `tests/`: pruebas y validaciones.

## 8. Consideraciones sobre Google Colab
- Cada integrante dispone de su propio entorno de ejecución.
- Las variables y archivos temporales de una sesión no se comparten automáticamente.
- Los cambios en el código deben guardarse explícitamente en GitHub.
- Guardar un notebook en GitHub no equivale a ejecutar su código.
- Antes de integrar cambios, comprobar que el notebook pueda ejecutarse desde el inicio.

## 9. Consideraciones sobre Google Drive
- Los datasets originales se almacenan en una carpeta compartida.
- No se deben sobrescribir los archivos originales.
- Las rutas de acceso se configurarán mediante un procedimiento común.
- Los archivos generados deben almacenarse en ubicaciones acordadas.

## 10. Procedimientos pendientes de documentar
Los siguientes procedimientos se completarán después de realizar pruebas de integración:
- Acceso al repositorio privado.
- Creación de ramas desde GitHub.
- Apertura de notebooks desde GitHub en Google Colab.
- Guardado de notebooks en la rama correspondiente.
- Creación y revisión de pull requests.
- Resolución de conflictos.
- Configuración de rutas compartidas de Google Drive.
- Recuperación de una versión anterior.

## 11. Mantenimiento
El manual deberá actualizarse cuando cambien las herramientas, los procedimientos o las reglas de colaboración.
