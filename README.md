# Worldwide Seismic Events Data Pipeline
A comprehensive end-to-end ETL analytics pipeline for earthquake data processing, leveraging Microsoft Fabric, Data Factory, PySpark, and Power BI to transform raw retail data into actionable business insights.   

## Architecture Overview    
    
![architecture](https://github.com/user-attachments/assets/77005bf6-f616-49fa-93d5-0bd235ae0789)    

This solution implements a modern data pipeline that ingests, transforms, and visualizes seismic data across the following components:      
    
<b>Microsoft Fabric:</b> Performs data transformation and business logic processing using <b> Medallion architecture </b>    
   
<b>Fabric Data Factory:</b> Orchestrates data movement and pipeline workflows using scheduling to batch process data every day from source.      
     
![data_factory](https://github.com/user-attachments/assets/6caf60a3-996a-4179-9aa4-46049933567a)  
   
![schedule](https://github.com/user-attachments/assets/9985c25a-72e0-407f-a50d-45208f6adb1c)     
   
<b>Power BI:</b> Delivers an interactive dashboard on earthquake data aggregation for country-wise insights.   

       
## Data Source:    
<a href="https://www.usgs.gov/programs/earthquake-hazards" target="_blank">US Geographical Survey website</a>     
<a href="https://earthquake.usgs.gov/fdsnws/event/1/" target="_blank">Earthquake API documentation</a>

      
## Notebooks:    
<b>Bronze Notebook:</b> This notebook focuses on ingesting raw earthquake data from the USGS API. It performs minimal processing to store data in its raw format.   

<b>Silver Notebook:</b> Processes data from the Bronze layer by cleaning, transforming, and consolidating the seismic event data. It prepares the data for aggregation in the gold layer to be used for analytics.   

<b>Gold Notebook:</b> In this final processing stage, the notebook aggregates the data to create analytics-ready datasets optimized for high-value insights in tools like Power BI   

      
## Visualisation on Power BI    
    
![erqk](https://github.com/user-attachments/assets/4e5c6b30-0fb4-4c5d-91c2-595a55b120d5)

 

  
    
