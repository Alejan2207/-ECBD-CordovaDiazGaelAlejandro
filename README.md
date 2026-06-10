# Extracción de Conocimiento en Bases de Datos - 9B

## Datos generales

**Alumno:** Gael Alejandro Córdova Díaz  
**Materia:** Extracción de Conocimiento en Bases de Datos  
**Cuatrimestre / Grupo:** 9° B  
**Repositorio:** `-ECBD-CordovaDiazGaelAlejandro`

---

## Descripción general

Este repositorio reúne las prácticas, laboratorios, datasets y producto integrador desarrollados durante la materia **Extracción de Conocimiento en Bases de Datos**. El contenido está organizado para evidenciar el uso de herramientas de análisis de datos, limpieza de información, procesamiento con Python, consultas, visualización de resultados y construcción de un Data Warehouse.

A lo largo del proyecto se trabajan diferentes conjuntos de datos con el propósito de aplicar procesos de extracción, transformación, carga, análisis e interpretación de información. Además, se incluyen notebooks de laboratorio donde se practican conceptos relacionados con el modelo DIKW, limpieza de datos, exploración de datasets, análisis con pandas, generación de gráficas y consultas orientadas a la toma de decisiones.

El repositorio también contiene un producto principal enfocado en la creación e implementación de un **Data Warehouse de ventas** usando PostgreSQL, Jupyter Notebook y Python. Este producto permite demostrar el flujo completo desde la creación de tablas dimensionales y tabla de hechos, hasta la carga de datos, consultas SQL y visualización de indicadores clave.

---

## Objetivo

Aplicar técnicas de extracción, limpieza, transformación, análisis y visualización de datos mediante el uso de Python, Jupyter Notebook, PostgreSQL y librerías especializadas, con el fin de convertir datos en información útil para la interpretación, generación de conocimiento y apoyo a la toma de decisiones.

---

## Estructura del repositorio

```text
Extraccion_9B/
│
├── Dataset/
│   ├── clientes.csv
│   ├── productos.csv
│   ├── regiones.csv
│   ├── tiempo.csv
│   ├── ventas.csv
│   ├── dataset_sucio_practica.csv
│   ├── Data_Limpio_Factura.csv
│   ├── netflix_titles.csv
│   ├── test.csv
│   └── ventas-por-factura.csv
│
├── Notebooks/
│   ├── ProductoDW.ipynb
│   ├── Lab01.ipynb
│   ├── Lab02.ipynb
│   ├── Lab03.ipynb
│   ├── Lab04-DIKW.ipynb
│   ├── Lab05_DIKW_Netflix.ipynb
│   ├── Lab06.ipynb
│   ├── Lab07.ipynb
│   ├── Lab09.ipynb
│   ├── Lab10.ipynb
│   └── dfClientes_metadata.json
│
└── README.md
```

---

## Datasets utilizados

Los datasets se encuentran dentro de la carpeta `Dataset/` y se utilizan en diferentes prácticas y análisis de la materia.

| Dataset | Descripción general |
|---|---|
| `clientes.csv` | Contiene información de clientes utilizada para prácticas de análisis y para la dimensión de clientes en el Data Warehouse. |
| `productos.csv` | Contiene información de productos, categorías y precios, utilizada en análisis de ventas y en el modelo dimensional. |
| `regiones.csv` | Contiene información de regiones y ciudades para analizar ventas por ubicación geográfica. |
| `tiempo.csv` | Contiene información temporal como fechas, meses y año, utilizada para análisis por periodos. |
| `ventas.csv` | Contiene registros de ventas relacionados con clientes, productos, regiones y tiempo. |
| `dataset_sucio_practica.csv` | Dataset utilizado para ejercicios de limpieza, revisión de datos faltantes, duplicados y transformación de información. |
| `Data_Limpio_Factura.csv` | Dataset limpio relacionado con datos de facturación. |
| `ventas-por-factura.csv` | Dataset utilizado para análisis de ventas a partir de facturas. |
| `netflix_titles.csv` | Dataset utilizado para prácticas de análisis exploratorio, clasificación e interpretación de información. |
| `test.csv` | Dataset complementario utilizado para ejercicios y pruebas dentro de los laboratorios. |

---

## Herramientas utilizadas

- **Python:** lenguaje utilizado para procesamiento, análisis y visualización de datos.
- **Jupyter Notebook:** entorno utilizado para desarrollar y documentar las prácticas de análisis.
- **pandas:** librería utilizada para lectura de CSV, limpieza, transformación y manipulación de DataFrames.
- **Matplotlib:** librería utilizada para generar gráficas e indicadores visuales.
- **SQLAlchemy:** librería utilizada para conectar Python con bases de datos.
- **psycopg2-binary:** controlador utilizado para la conexión entre Python y PostgreSQL.
- **PostgreSQL:** gestor de base de datos utilizado para la implementación del Data Warehouse.
- **pgAdmin:** herramienta gráfica para administrar PostgreSQL, crear bases de datos, tablas y ejecutar consultas SQL.
- **Git / GitHub:** herramientas de control de versiones y almacenamiento del proyecto.

---

## Notebooks incluidos

| Notebook | Descripción general |
|---|---|
| `Lab01.ipynb` | Práctica inicial de análisis y manejo de datos. |
| `Lab02.ipynb` | Ejercicios de procesamiento y exploración de información. |
| `Lab03.ipynb` | Práctica de análisis y transformación de datos. |
| `Lab04-DIKW.ipynb` | Aplicación del modelo DIKW: datos, información, conocimiento y sabiduría. |
| `Lab05_DIKW_Netflix.ipynb` | Análisis del dataset de Netflix aplicando interpretación y organización de información. |
| `Lab06.ipynb` | Ejercicios de limpieza, procesamiento o análisis de datos. |
| `Lab07.ipynb` | Práctica de análisis con datasets de la carpeta `Dataset/`. |
| `Lab09.ipynb` | Laboratorio de análisis y consultas sobre información procesada. |
| `Lab10.ipynb` | Práctica final o complementaria de análisis de datos. |
| `ProductoDW.ipynb` | Notebook del producto principal: creación, carga, consulta y visualización de un Data Warehouse con PostgreSQL y Python. |

---

## Instrucciones de ejecución general

### 1. Descargar o clonar el repositorio

Descargar el proyecto y abrir la carpeta principal:

```bash
git clone <URL_DEL_REPOSITORIO>
cd Extraccion_9B
```

Si el proyecto se entrega como archivo comprimido, solo se debe descomprimir la carpeta `Extraccion_9B`.

### 2. Abrir Jupyter Notebook

Desde Anaconda Navigator, JupyterLab o terminal, abrir Jupyter Notebook dentro de la carpeta del proyecto:

```bash
jupyter notebook
```

Después entrar a la carpeta `Notebooks/` y abrir el notebook que se desea ejecutar.

### 3. Instalar librerías necesarias

En caso de no tener las librerías instaladas, ejecutar en una celda de Jupyter:

```python
!pip install pandas matplotlib sqlalchemy psycopg2-binary
```

### 4. Ejecutar notebooks de laboratorio

Para los laboratorios generales, abrir el notebook correspondiente y ejecutar las celdas en orden. Los archivos CSV deben estar disponibles en la carpeta `Dataset/`.

Ejemplo de lectura de dataset:

```python
import pandas as pd

df = pd.read_csv("../Dataset/netflix_titles.csv")
df.head()
```

### 5. Ejecutar el producto de Data Warehouse

Para ejecutar el notebook `ProductoDW.ipynb`, primero se debe tener instalado PostgreSQL y creada una base de datos llamada:

```text
datawarehouse_ventas
```

Después, en el notebook se configura la conexión a PostgreSQL:

```python
usuario = "postgres"
password = "123456"
host = "localhost"
puerto = "5432"
base_datos = "datawarehouse_ventas"
```

Posteriormente, ejecutar las celdas en orden para:

1. Conectar Python con PostgreSQL.
2. Crear tablas de dimensión y tabla de hechos.
3. Simular o importar datos desde CSV.
4. Limpiar y transformar datos con pandas.
5. Cargar los datos al Data Warehouse.
6. Ejecutar consultas SQL.
7. Generar gráficas e indicadores.

---

## Capturas o imágenes de los análisis

Las evidencias visuales de los análisis se encuentran principalmente como salidas dentro de los notebooks. Entre los resultados generados se incluyen:

- Tablas de datos cargadas desde archivos CSV.
- Revisión de valores nulos y tipos de datos.
- Consultas SQL ejecutadas desde Jupyter y PostgreSQL.
- Reportes con uniones entre tablas de dimensión y tabla de hechos.
- Gráfica de ventas por región.
- Gráfica de productos más vendidos.
- Gráfica de ventas por mes.
- Resultados de análisis exploratorio en los notebooks de laboratorio.

Si se desea documentar las imágenes fuera del notebook, se recomienda crear una carpeta llamada `Imagenes/` o `Capturas/` y guardar ahí las evidencias exportadas. Ejemplo:

```text
Extraccion_9B/
├── Capturas/
│   ├── ventas_por_region.png
│   ├── productos_mas_vendidos.png
│   └── ventas_por_mes.png
```

Posteriormente, se pueden insertar en el README de la siguiente forma:

```markdown
![Ventas por región](Capturas/ventas_por_region.png)
![Productos más vendidos](Capturas/productos_mas_vendidos.png)
![Ventas por mes](Capturas/ventas_por_mes.png)
```

---

## Resultados generales obtenidos

Durante el desarrollo de las prácticas se trabajó con diferentes datasets para aplicar técnicas de análisis y procesamiento de información. En los notebooks se realizan actividades como lectura de archivos CSV, exploración de datos, limpieza, transformación, validación, consultas y visualización de resultados.

En el producto de Data Warehouse se logró crear una estructura dimensional con tablas de clientes, productos, regiones y tiempo, además de una tabla de hechos para registrar las ventas. A partir de esta estructura fue posible realizar análisis como ventas por región, productos más vendidos y ventas por mes.

Estos resultados permiten observar cómo los datos pueden organizarse para generar información más clara y útil, facilitando la interpretación de indicadores y apoyando la toma de decisiones.

---

## Conclusiones generales

El desarrollo de este repositorio permitió aplicar de manera práctica los conceptos vistos en la materia de Extracción de Conocimiento en Bases de Datos. A través de los diferentes laboratorios y datasets se comprendió la importancia de limpiar, organizar y transformar los datos antes de analizarlos.

El uso de Jupyter Notebook facilitó la documentación del proceso, ya que permite combinar código, resultados, tablas y gráficas en un mismo entorno. Además, el uso de Python y pandas permitió manipular la información de manera eficiente.

La implementación del Data Warehouse mostró cómo una base de datos orientada al análisis puede organizar la información en dimensiones y hechos, permitiendo generar consultas más claras e indicadores útiles. Este tipo de solución es importante porque ayuda a convertir datos dispersos en información estructurada para la toma de decisiones.

En general, las prácticas del repositorio fortalecen habilidades en análisis de datos, manejo de datasets, visualización de información y uso de herramientas de bases de datos, competencias importantes para el desarrollo de software y la gestión de información.

---
