# Azure Project

This project demonstrates various methods to access Azure Data Lake Storage (ADLS) and perform data ingestion, presentation, and analysis tasks using **Databricks**, **Key Vaults**, **Entra ID**, **Storage Accounts**, **Data Factory**, **Cost Management**, **Python**, **PySpark**, and **SQL**.

---

## Technologies Used

- **Databricks**: For data processing and analysis.
- **Key Vaults**: For securely storing and managing secrets.
- **Entra ID**: For authentication and access management.
- **Storage Account**: For storing data in ADLS.
- **Data Factory**: For orchestrating data pipelines.
- **Cost Management**: For monitoring and optimizing costs.
- **Python**: For scripting and data processing.
- **PySpark**: For distributed data processing in Databricks.
- **SQL**: For querying and analyzing structured data.

## Project Structure

### Folder Set-Up

1. **1_access_adls_using_access_keys**
<img src="adls/Images/1.png" alt="imagelalalaa" width="50%" />

2. **2_access_adls_using_sas_token**
<img src="adls/Images/2.png" alt="imagelalalaa" width="75%" />

3. **3_access_adls_using_service_principal** 
<img src="adls/Images/3.png" alt="imagelalalaa" width="75%" />
<img src="adls/Images/4.png" alt="imagelalalaa" width="75%" /> 

4. **4_access_adls_using_cluster_scoped_credentials**  
5. **5_explore_dbutils_secrets_utility**  
6. **6_access_adls_using_secrets**  
7. **7_access_adls_using_secret_sas_token**  
8. **8_explore_dbfs_root**  
9. **9_mount_adls_using_service_principal**  
10. **10_mount_adls_containers_for_project**
<img src="adls/Images/5.png" alt="imagelalalaa" width="75%" />
<img src="adls/Images/6.png" alt="imagelalalaa" width="75%" /> 
<img src="adls/Images/7.png" alt="imagelalalaa" width="75%" />
<img src="adls/Images/8.png" alt="imagelalalaa" width="75%" />  

### Folder Ingestion
The Ingestion Folder focuses on the process of extracting, transforming, and loading (ETL) data from various file formats—such as CSV, JSON, and bulk files—into Azure Data Lake Storage (ADLS). Using PySpark within Databricks, the data was efficiently read from ADLS, transformed to meet project requirements, and then written back to ADLS in a structured format for further analysis. The ingestion process handled a variety of file types, including single CSV and JSON files, as well as multiple CSV and JSON files for bulk ingestion. Authentication and secure access to ADLS were managed through Azure Key Vault, ensuring that sensitive credentials were securely stored and retrieved. This was a simple project with relatively small datasets, and the main objective was to work with the Azure environment, leveraging tools like Databricks, ADLS, and Key Vault to build a streamlined ETL workflow. All files used in this process are located in the adls folder within this GitHub repository.
0. **0_ingest_all_files**  
1. **1_ingest_circuits_file**  
2. **2_ingest_races_file**  
3. **3_ingest_construct_file**  
4. **4_ingest_drivers_file**  
5. **5_ingest_results_file**  
6. **6_ingest_pitstop_file**  
7. **7_ingest_laptimes_file**  
8. **8_ingest_qualifying_file**
<img src="adls/Images/9.png" alt="imagelalalaa" width="75%" />
<img src="adls/Images/10.png" alt="imagelalalaa" width="75%" /> 

### Folder Presentation
The Presentation Folder combines diverse datasets to perform minor analyses, such as identifying the best drivers in the 2020 Abu Dhabi Grand Prix, the best driver and team by year, and standardizing points calculations across different seasons
1. **1_race_results**  
2. **2_driver_standings**  
3. **3_constructors_standing**  
4. **4_calculated_race_results_py**  
5. **5_calculated_race_results_sql**  

### Folder Includes

- **common_functions**: Contains shared utility functions used across the project. These functions are accessed in notebooks using the %run command to avoid code duplication and ensure consistency.
- **configuration**: Stores configuration files that centralize settings and parameters, making it easier to manage and update project-wide configurations.
<img src="adls/Images/11.png" alt="imagelalalaa" width="75%" /> 
### Folder Analysis
This folder contains two notebooks with visualizations created in Databricks. The analyses focus on identifying dominant drivers and teams based on historical data. Visualizations are included in the notebooks for better insights, and I’ve added them to the files for you to review.

1. **1_find_dominant_drivers**  
2. **2_find_dominant_teams**

### Folder ADLS

1. **demo**  
2. **images**
3. **raw**
4. **process1**
5. **presentation**

## Databricks Insights

### Cluster Creation
<img src="adls/Images/12.png" alt="Cluster Creation" width="30%" />

### Job Configuration
<img src="adls/Images/13.png" alt="Job Configuration" width="75%" />

### Catalog Management
<img src="adls/Images/14.png" alt="Catalog Management" width="75%" />

## Data Factory Insights

### Association of the Cluster Created in Databricks
<img src="adls/Images/21.png" alt="Cluster Association" width="75%" />
<img src="adls/Images/15.png" alt="Cluster Association" width="75%" />

### Association of ADLS
<img src="adls/Images/17.png" alt="ADLS Association" width="50%" />

### Creation and Execution of a Pipeline with All Ingestion Notebooks
<img src="adls/Images/16.png" alt="Pipeline Execution" width="50%" />

### Verification of the Raw Folder in ADLS and Execution of Ingestion Notebooks
<img src="adls/Images/18.png" alt="Raw Folder Verification" width="50%" />

## Cost of This Small Project
<img src="adls/Images/19.png" alt="Project Cost" width="50%" />

## My Azure Portal Dashboard for This Project
<img src="adls/Images/20.png" alt="Azure Portal Dashboard" width="75%" />

