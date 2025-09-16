# LinkedIn Jobs Data Pipeline  

Este repositorio contiene un **pipeline de datos de extremo a extremo** desarrollado en **Databricks + Azure**, que procesa ofertas de empleo de **LinkedIn** y las disponibiliza para su análisis en **Power BI**.  

## 🚀 Funcionalidades principales  
- Ingesta de ofertas de empleo desde LinkedIn (staging → bronze).  
- Limpieza y estandarización de datos en la capa **Silver**.  
- Modelado dimensional en la capa **Gold** (tablas de hechos y dimensiones).  
- Almacenamiento en **Azure Data Lake (Delta Lake)**.  
- Parametrización:  
  - Tipo de empleo (Data Scientist, Data Engineer, etc.).  
  - Frecuencia de ejecución (diaria o mensual).  
- Visualización final en **Power BI**.  

## 🏗️ Arquitectura  
El pipeline sigue la estructura **medallion** (Bronze → Silver → Gold):  

1. **Job Ingesta** → captura de datos y almacenamiento en *Bronze*.  
2. **Job Limpieza** → transformaciones y normalización (*Silver*).  
3. **Job Modelado** → creación de tablas optimizadas para BI (*Gold*).  


## 🛠️ Tecnologías utilizadas  
- **Azure Data Lake Storage (ADLS)**  
- **Databricks (PySpark, Delta Lake, Jobs)**  
- **Python**  
- **Power BI**

## 🖼️ Diagrama del Pipeline

![Diagrama del pipeline](./Diagrama sin título.drawio.png)

## 📜 Licencia  
Este proyecto se distribuye bajo la licencia **MIT**. Consulta el archivo [LICENSE](LICENSE) para más información.  
