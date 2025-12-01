Análisis Exploratorio de Datos (EDA) de Airbnb CDMX

## Descripción General del Proyecto

Este proyecto consiste en un Análisis Exploratorio de Datos (EDA) detallado utilizando un conjunto de datos públicos de listados de Airbnb en **Ciudad de México**. El objetivo principal es ayudar a un inversor ficticio a decidir dónde comprar una propiedad para alquilarla en Airbnb.
## Objetivos del Análisis

1.  **Entendimiento del Mercado:** Determinar la distribución de precios y la oferta de alojamientos en las diferentes zonas de la ciudad.
2.  **Factores Determinantes del Precio:** Identificar las variables clave (ej. tipo de habitación, número de reseñas, ubicación) que influyen en el precio por noche.
3.  **Limpieza y Preprocesamiento:** Aplicar técnicas de manejo de valores nulos y atípicos para asegurar la calidad del dataset.

 Fuente de Datos

* **Dataset:** listings.csv
* **Origen:** Inside Airbnb
* **Tamaño:** 10 columnas y 26401 filas

##  Metodología de EDA

El análisis se llevó a cabo siguiendo una estructura rigurosa para garantizar la calidad de los datos y la relevancia de los hallazgos:

1.  **Inspección Inicial:** Revisión de tipos de datos, valores únicos y conteo de valores nulos.
2.  **Manejo de Datos Faltantes:** Se eliminaron datos NaN usando Dropna en columnas donde estos datos podrían sesgar el analisis. También se uso fillna en algunas filas donde no habian reviews por ser nuevas propiedades.
3.  **Análisis Univariado:** Visualización de distribuciones de variables clave como el `price`, `reviews_per_month'
4.  **Análisis Bivariado y Multivariado:**
    * Relación entre **Precio** y **Ubicación** usando mapas o gráficos de caja por barrio
    * Impacto de la **Puntuación de Reseñas** en la disponibilidad y el precio.
5.  **Detección de Valores Atípicos:** Identificación y tratamiento de precios extremadamente altos para evitar sesgos en la media.

##  Resultados e Insights Clave


* **Insight 1 (Precios):** El **entire home** resultó ser el más caro, con un precio promedio de **$1173** por noche. 
* **Insight 2 (Demanda):** La demanda en barrios como Cuauhtemoc y Coyoacan resultaron ser los lugares donde eligen alojarse mas frecuentemente. 
* **Insight 3 (Inversión):** Se realizo una busqueda en la cual detectara los lugares con un precio menor al promedio y una demanda mensual mayor a la promedio para elegir un lugar en el cual invertir.
* **Insight 4 (Sugerencia):** **Priorizar el Tipo de Propiedad:** Invertir en listados de tipo **Entire Home**.
**Enfoque Geográfico:** Concentrar la búsqueda de compra en el barrio **Venustiano Carranza**.

## 💻 Herramientas y Tecnologías

* **Lenguaje de Programación:** Python 
* **Entorno de Desarrollo:** Google Colab
* **Librerías Clave:**
    * `pandas` 
    * `numpy` 
    * `plotly` 
    * `geopandas`

