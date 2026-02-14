# Worldwide Seismic Events Data Pipeline
A comprehensive end-to-end ETL analytics pipeline for earthquake data processing, leveraging Microsoft Fabric, Data Factory, PySpark, and Power BI to transform raw retail data into actionable business insights.

### Architecture Overview
This solution implements a modern data pipeline that ingests, transforms, and visualizes seismic data across the following components:

<b>Microsoft Fabric:</b> Performs data transformation and business logic processing using <b> Medallion architecture </b>  
<b>Fabric Data Factory:</b> Orchestrates data movement and pipeline workflows using scheduling to batch process data every day from source.  
<b>Power BI:</b> Delivers an interactive dashboard on earthquake data aggregation for country-wise insights. 

<b>Data Source:</b> <a href="https://www.usgs.gov/programs/earthquake-hazards">US Geographical Survey website</a>

### Notebooks:
<b>Bronze Notebook:</b> This notebook focuses on ingesting raw earthquake data from the USGS API. It performs minimal processing to store data in its raw format.

<b>Silver Notebook:</b> Processes data from the Bronze layer by cleaning, transforming, and consolidating the seismic event data. It prepares the data for aggregation in the gold layer to be used for analytics.

<b>Gold Notebook:</b> In this final processing stage, the notebook aggregates the data to create analytics-ready datasets optimized for high-value insights in tools like Power BI


![retail_1]()    
    
