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
Este repositorio alberga un dashboard interactivo desarrollado en Power BI, destinado al análisis de datos relacionados con siniestros viales en Buenos Aires. El dashboard consta de cinco hojas, cada una diseñada para proporcionar una perspectiva específica de los datos.

#### Portada
La hoja de portada ofrece una visión general del documento y facilita la navegación entre las distintas pestañas del dashboard.

#### Información General
Esta hoja presenta gráficos que permiten analizar el número de víctimas de siniestros viales, con la capacidad de filtrar los datos según diversos criterios como el año, el tipo de vehículo involucrado, la gravedad del accidente y la parte responsable del mismo.

#### Análisis Adicional
En esta sección se incluyen gráficos complementarios que proporcionan una comprensión más profunda de los datos. Se exploran variables como la edad de las víctimas, su rol en el accidente y el tipo de vehículo que conducían, permitiendo la interacción mediante filtros adicionales basados en el sexo de las víctimas.

#### Indicadores Clave de Rendimiento (KPI's)
La hoja de KPI's presenta cuatro métricas fundamentales para evaluar la situación de los siniestros viales en Buenos Aires. Estos KPI's se calcularon mediante el uso de funciones DAX (Data Analysis Expressions), lo que garantiza precisión y flexibilidad en los cálculos. Los indicadores son los siguientes:

1. **Reducción de Homicidios**: Evalúa si se alcanzó una disminución del 10% en los homicidios relacionados con siniestros viales.
2. **Reducción de Accidentes Fatales de Motociclistas**: Analiza si se logró reducir en un 7% la cantidad de accidentes fatales involucrando motociclistas entre los años 2020 y 2021.
3. **Proporción de Accidentes con Más de una Víctima**: Muestra la proporción de accidentes con múltiples víctimas en relación con el total de accidentes registrados.
4. **Reducción de Accidentes Graves**: Este KPI busca determinar si se logró una reducción del 10% en los accidentes que resultaron en lesiones graves o fatales.

#### Análisis de Inteligencia Artificial (IA)
La última hoja del dashboard contiene un análisis avanzado utilizando herramientas de inteligencia artificial. Este análisis busca identificar y explicar la influencia de diversas variables en otras de importancia dentro del contexto de los siniestros viales.

El dashboard es altamente interactivo, permitiendo a los usuarios aplicar filtros y observar cambios en tiempo real en las visualizaciones. Este enfoque dinámico facilita un análisis exhaustivo y personalizado de los datos, brindando una plataforma efectiva para la toma de decisiones informadas en materia de seguridad vial.

### Instrucciones de Uso

1. Descargue o clone este repositorio en su máquina local.
2. Ejecute los scripts de Python en el orden especificado para llevar a cabo el proceso de ETL y análisis de datos.
3. Abra el archivo `dashboard.pbix` en Power BI para explorar el dashboard interactivo.
4. Siga las instrucciones dentro del dashboard para filtrar y visualizar los datos según sus necesidades.

### Requerimientos

- Python 3.11
- Bibliotecas de Python: pandas, seaborn, matplotlib
- Power BI Desktop (para visualizar y editar el dashboard)
