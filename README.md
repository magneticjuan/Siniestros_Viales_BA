## Proyecto: Análisis de Comportamiento de Siniestros Viales en Buenos Aires

Este repositorio alberga los recursos y resultados de un proyecto de análisis de siniestros viales en la ciudad de Buenos Aires. El objetivo principal es comprender y presentar de manera efectiva el comportamiento de estos incidentes, aprovechando herramientas de análisis de datos y visualización para generar información útil y acciones orientadas a la seguridad vial.

### Estructura del Repositorio

- **Archivos de Código:**
  - `ETL_Lesiones.py`: Este script implementa el proceso de Extracción, Transformación y Carga (ETL) de datos relacionados con lesiones derivadas de siniestros viales.
  - `ETL_Homicidios.py`: Similar al script anterior, se ocupa del ETL de datos sobre homicidios en siniestros viales.
  - `EDA.py`: Contiene el Análisis Exploratorio de Datos (EDA), que incluye limpieza, visualización y estadísticas descriptivas.
  - `dashboard.pbix`: Archivo del dashboard interactivo creado en Power BI.

- **Datasets:**
  - `lesiones.xlsx`: Archivo Excel que contiene datos sobre lesiones en siniestros viales.
  - `homicidios.xlsx`: Archivo Excel con datos sobre homicidios en siniestros viales.
  
- **CSV:**
  - Archivos CSV resultantes del proceso de ETL para lesiones y homicidios, respectivamente.

### Descripción de los Códigos

1. **ETL_Lesiones.py** y **ETL_Homicidios.py**:
   - Estos scripts realizan la extracción de datos de los archivos de Excel mencionados, seguido de la transformación y carga de los mismos.
   - Utilizan librerías como pandas para el manejo de datos y numpy para operaciones numéricas.
   - Funciones como `read_excel` de pandas se emplean para leer los datos desde los archivos.
   - Realizan tareas de limpieza y normalización de datos, eliminando columnas innecesarias y almacenando los resultados en archivos CSV.

2. **EDA.py**:
   - Contiene el Análisis Exploratorio de Datos (EDA) para los conjuntos de datos de lesiones y homicidios.
   - Utiliza pandas para manipular y analizar los datos, y seaborn y matplotlib para la visualización.
   - Funciones como `describe()` y `countplot()` de seaborn se utilizan para generar estadísticas descriptivas y visualizaciones de los datos, respectivamente.

### Power BI Dashboard

El archivo `dashboard.pbix` contiene un dashboard interactivo creado en Power BI. Este dashboard presenta visualmente los hallazgos del análisis de datos realizado en los scripts Python. Proporciona una vista intuitiva y fácil de entender del comportamiento de los siniestros viales en Buenos Aires.

**Notas Adicionales sobre el Dashboard:**
- Al abrir el dashboard, se encontrarán medidas creadas con fórmulas DAX planificadas para su uso en la creación de KPIs. Sin embargo, debido a limitaciones de rendimiento en la máquina del autor, estas medidas no fueron ejecutadas.
- Las medidas incluidas son:
  - **Semestre Actual**: Calcula las métricas del semestre actual.
  - **Semestre Anterior**: Calcula las métricas del semestre anterior.
  - **Varianza entre Semestres**: Calcula la diferencia entre las métricas del semestre actual y el semestre anterior.
- Se invita al usuario a intentar utilizar estas medidas para crear KPIs y analizar aún más los datos.

### Instrucciones de Uso

1. Descargue o clone este repositorio en su máquina local.
2. Ejecute los scripts de Python en el orden especificado para llevar a cabo el proceso de ETL y análisis de datos.
3. Abra el archivo `dashboard.pbix` en Power BI para explorar el dashboard interactivo.
4. Siga las instrucciones dentro del dashboard para filtrar y visualizar los datos según sus necesidades.

### Requerimientos

- Python 3.x
- Bibliotecas de Python: pandas, seaborn, matplotlib
- Power BI Desktop (para visualizar y editar el dashboard)