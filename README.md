# AQI_Analyzer
### This project pulls hourly data for the past 4 years for 3000 coordinates across the city. That is effectively one coordinate for every 2 square kilometers and more than 80 million records.


## The Problem
Air quality in the city of Mumbai has deteriorated in the past few years and poses a significant threat to public health, leading to respiratory diseases, cardiovascular conditions, and premature deaths. Pollutants such as particulate matter (PM2.5 and PM10), nitrogen dioxide (NO₂), sulfur dioxide (SO₂), carbon monoxide (CO), and ground-level ozone (O₃) are prevalent, originating from sources like vehicle emissions, industrial activities, and construction dust.

## How I got the Idea 
Every time I visit my hometown Mumbai, I can feel & see the air being worse than the last time. Some say it's because of ongoing construction projects, some say it's increased traffic in the city. It is possibly a combination of many such factors. The first step in identifying key factors is to find trends and patterns, and then figure out the underlying cause. That's the idea of the project.

## The Solution
To solve this issue, it is first neccessary to analyze when where and how air pollution occurs in the city. This project aims to develop a comprehensive air pollution monitoring and analysis system for Mumbai, utilizing advanced technologies to collect, visualize, and interpret air quality data. The goal is to empower policymakers, health officials, and the public with actionable insights to mitigate air pollution and its adverse health effects.

Data Ingestion: Data is ingested from a public API source: Open Weather Map. I picked 3000 coordinates all over the city and pulled hourly air quality data for the past 4 years using a python script, before uploading it into an Azure Blob.

Data Transformation: I took the data in my Azure Blob and processed it in Azure Data Factory, configured the data according to my database model, and loaded more than 80 million records into a SQL database.

Data Visualization: I redirected the data in my SQL database to PowerBI, where I built a dashboard showcasing a time-series analysis for locations all over the city.


## Technologies used

### Python: 
Pulled data using a public API. Uploaded to Azure Blob using Azure CLI.

### Azure Key Vault: 
Stored all API keys & credentials here for safekeeping and easy accessibility.

### Azure Blob Storage: 
Dumped raw, unstructured json data here.
![image](https://github.com/user-attachments/assets/6a19e695-f6f6-4cea-8c7d-2d45c12a221e)



### Azure Data Factory: 
Transformed data according to the data model specifications.
![ADF Workflow](https://github.com/user-attachments/assets/88333076-687a-4b64-aa9c-7780dda3ab27)


### SQL Database: 
Created a database to store 80+ million records in a structured manner.

### PowerBI: 
Visualized the data, enabling users to gain valuable insights.
![image](https://github.com/user-attachments/assets/7eb7eb2c-151c-44fc-a5d9-80695a7e25bb)

