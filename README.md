# Proyecto_Analisis_Estudiantes
Repositorio dedicado a la elaboración de proyecto de clonación de repositorio para la reproductibilidad de trabajos de código python

Este proyecto consiste en un análisis exploratorio de datos (EDA) realizado sobre un conjunto de datos de rendimiento académico estudiantil.

El objetivo principal es demostrar la reproducibilidad de proyectos de análisis de datos mediante el uso de:

- Git y GitHub para control de versiones.
- Entornos virtuales de Python.
- Gestión de dependencias mediante `requirements.txt`.
- Jupyter Lab para el desarrollo del análisis.

El notebook contiene procesos de exploración, validación, transformación y visualización de datos orientados a identificar patrones sobre el desempeño académico de una población estudiantil.

---

# Dataset

## Nombre del dataset

Students Performance Dataset

## Fuente

Dataset público sobre desempeño académico estudiantil.

Archivo utilizado:

```
StudentsPerformance.csv
```

## Descripción

El conjunto de datos contiene información de 1000 estudiantes y 8 variables:

- Género.
- Grupo étnico.
- Nivel educativo de los padres.
- Tipo de alimentación.
- Curso de preparación para examen.
- Calificación de matemáticas.
- Calificación de lectura.
- Calificación de escritura.

Durante el análisis también se construye una nueva variable denominada:

```
Average_Final
```

que representa el promedio general de las tres materias evaluadas.

---

# Objetivo

Analizar el comportamiento académico de una población estudiantil mediante técnicas básicas de análisis exploratorio de datos.

Los objetivos específicos son:

- Verificar la integridad del dataset.
- Detectar valores nulos y registros duplicados.
- Analizar distribuciones de variables categóricas y numéricas.
- Construir una métrica global de rendimiento académico.
- Clasificar estudiantes según su desempeño.
- Comparar grupos de estudiantes.
- Responder preguntas de análisis mediante estadísticas descriptivas.
- Generar visualizaciones que apoyen la interpretación de los resultados.

---

# Requisitos

Se requiere:

- Python 3.x
- Git
- Jupyter Lab

Las dependencias necesarias para reproducir el entorno de trabajo se encuentran en:

```
requirements.txt
```

---

# Instalación

## Clonar el repositorio

```bash
git clone URL_DEL_REPOSITORIO
```

## Entrar al proyecto

```bash
cd nombre-del-repositorio
```

## Crear el entorno virtual

```bash
python -m venv .venv
```

## Activar el entorno virtual

### Windows

```bash
.venv\Scripts\activate
```

### Linux / MacOS

```bash
source .venv/bin/activate
```

## Instalar dependencias

```bash
pip install -r requirements.txt
```

---

# Ejecución

Con el entorno virtual activado:

```bash
jupyter lab
```

o

```bash
python -m jupyter lab
```

Posteriormente abrir:

```
src/Analysis.ipynb
```

En caso de que Jupyter solicite seleccionar un kernel, elegir el correspondiente al entorno virtual creado para el proyecto.

---

# Análisis realizados

El notebook desarrolla las siguientes etapas:

## 1. Exploración inicial

- Número de registros.
- Número de variables.
- Tipos de datos.
- Valores nulos.
- Registros duplicados.
- Estadística descriptiva.

## 2. Validación de integridad

Se verificó la presencia de:

- Valores faltantes.
- Filas duplicadas.
- Columnas duplicadas.
- Valores fuera de rango esperado.

## 3. Análisis de variables categóricas

Se analizaron:

- Distribución de género.
- Distribución de grupos.
- Nivel educativo de los padres.
- Curso de preparación.
- Tipo de alimentación.

## 4. Análisis de variables numéricas

Se evaluaron:

- Matemáticas.
- Lectura.
- Escritura.

Considerando rangos, estadísticas descriptivas y comportamiento general.

## 5. Construcción de nuevas variables

Se creó:

```
Average_Final
```

como promedio general del estudiante.

También se construyó una clasificación de desempeño académico basada en rangos de calificación.

## 6. Respuesta a preguntas de análisis

Entre otras:

- ¿Qué materia presenta el mayor promedio?
- ¿Influye el curso de preparación en el rendimiento?
- ¿Qué porcentaje alcanza calificaciones sobresalientes?
- ¿Qué grupo obtiene los mejores resultados?

## 7. Visualización de datos

Se implementaron:

- Matriz de nulos.
- Gráfico de barras por grupo.
- Gráfico de pastel para distribución de género.

---

# Resultados y conclusiones

Los principales hallazgos del análisis fueron:

- El dataset presenta una integridad completa, sin valores nulos ni registros duplicados.
- La materia con mejor promedio general es Lectura (Reading Score).
- Los estudiantes que completaron el curso de preparación obtienen mejores resultados promedio.
- Aproximadamente el 20% de los estudiantes alcanza un rendimiento sobresaliente o superior.
- El grupo E presenta el mayor promedio académico.
- El grupo A presenta el menor promedio académico.
- Existe una tendencia creciente en los promedios conforme avanzan los grupos de A a E.

En general, el análisis muestra cómo técnicas básicas de exploración y procesamiento de datos pueden utilizarse para identificar patrones académicos que podrían apoyar la toma de decisiones dentro de una institución educativa.

---

# Reproducibilidad

Este proyecto fue diseñado para ser completamente reproducible.

Cualquier usuario puede obtener los mismos resultados siguiendo los siguientes pasos:

1. Clonar el repositorio.
2. Crear un entorno virtual.
3. Instalar las dependencias mediante `requirements.txt`.
4. Ejecutar el notebook principal.

De esta manera se obtiene un entorno equivalente al utilizado durante el desarrollo original del análisis.

---

# Autor

Ari Leonardo Hernández Huerta  

Proyecto académico orientado a:

- Análisis exploratorio de datos.
- Reproducibilidad de proyectos.
- Gestión de dependencias.
- Uso de Git y GitHub como sistema de control de versiones.


Notas finales: 
Algunos commit que no tienen la nomenclatura habitual son merges o sincronizaciones entre los commits realizados de y por GitHub (vía sitio web) junto con los commits del proyecto local, pero ningún otro cambio se hizo en esas actualizaciones.
