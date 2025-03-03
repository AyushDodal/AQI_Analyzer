# AQI_Analyzer


## The Problem
Air quality in the city of Mumbai has deteriorated in the past few years and poses a significant threat to public health, leading to respiratory diseases, cardiovascular conditions, and premature deaths. Pollutants such as particulate matter (PM2.5 and PM10), nitrogen dioxide (NO₂), sulfur dioxide (SO₂), carbon monoxide (CO), and ground-level ozone (O₃) are prevalent, originating from sources like vehicle emissions, industrial activities, and construction dust.

## The Solution
To solve this issue, it is first neccessary to analyze when where and how air pollution occurs in the city. This project aims to develop a comprehensive air pollution monitoring and analysis system for Mumbai, utilizing advanced technologies to collect, visualize, and interpret air quality data. The goal is to empower policymakers, health officials, and the public with actionable insights to mitigate air pollution and its adverse health effects.

Access the website here: https://ayushdodal.github.io/AQI_Analyzer/

## Technologies used

Python: Pulled data using a public API. Uploaded to Azure Blob using Azure CLI.

Azure Key Vault: Stored all API keys & credentials here for safekeeping and easy accessibility.

Azure Blob Storage: Dumped raw, unstructured json data here.
![image](https://github.com/user-attachments/assets/6a19e695-f6f6-4cea-8c7d-2d45c12a221e)



Azure Data Factory: Transformed data according to the data model specifications.
![ADF Workflow](https://github.com/user-attachments/assets/88333076-687a-4b64-aa9c-7780dda3ab27)


SQL Database: Created a database to store 80+ million records in a structured manner.

PowerBI: Visualized the data, enabling users to gain valuable insights.
