# SentinelGeoIP

# Project: Uploading Geo-Data to Azure Storage and Integrating with Sentinel

## Project Overview

In this project, I worked with large geo-data files, uploaded them to Azure Storage, and integrated them into Azure Sentinel for enhanced security monitoring. The project involved setting up **Log Analytics Workspace (LAW)**, configuring **Azure Sentinel**, and creating a **watchlist** from a CSV file containing geo-location information. By following this process, I learned to manage large datasets in the cloud and leverage Sentinel for data analysis.

## Steps Completed

### 1. **Download Geo-Data File**
   - Downloaded the geo-location data CSV file (`geoip-summarized.csv`) from the GitHub repository:
     - [Download File]

### 2. **Create Log Analytics Workspace**
   - Created a **Log Analytics Workspace (LAW)** named: `LAW-Cyber-Lab-0x` in Azure Portal.
   - This workspace will serve as the central hub for data aggregation and query processing.

### 3. **Set Up Azure Sentinel**
   - Set up **Azure Sentinel** and connected it to the Log Analytics Workspace created in the previous step.
   - Ensured that all configurations adhered strictly to the provided naming conventions to avoid errors and ensure a smooth setup.

### 4. **Upload Geo-IP Data to Sentinel**
   - **Created a Watchlist** in Azure Sentinel using the **geoip-summarized.csv** file:
     - **Watchlist Name/Alias**: geoip
     - **Source Type**: Local File
     - **Number of lines before row**: 0
     - **Search Key**: network
   - Uploaded the file to the **Azure Storage** and integrated it with **Azure Sentinel** via the **Log Analytics Workspace**.
   - Allowed time for the 27,000+ records to load into Sentinel, ensuring the upload was completed.

### 5. **Validate Upload and Query Watchlist**
   - Queried the watchlist in **Log Analytics Workspace** using the following query:
     ```bash
     _GetWatchlist("geoip")
     ```
   - Verified that the query returned results, indicating that the watchlist was successfully loaded and accessible.

### 6. **Final Check**
   - Ensured the **watchlist** finished uploading and was completely available for querying before proceeding with the next steps in the lab.

## Key Learnings
- **Azure Storage Integration**: Learned how to work with large datasets and store them in **Azure Storage** for easy retrieval.
- **Azure Sentinel Setup**: Gained hands-on experience in setting up **Azure Sentinel**, a cloud-native security information and event management (SIEM) solution.
- **Log Analytics Workspace**: Understood the concept of **Log Analytics Workspaces** and how they are used to store and analyze log data in Azure.
- **Watchlist Configuration**: Learned to create and manage **watchlists** in **Azure Sentinel** for efficient querying of geo-location data.
  
## Technologies Used
- **Azure Storage**
- **Azure Sentinel**
- **Log Analytics Workspace (LAW)**
- **Azure Portal**

## Screenshots (Optional)
_(Here, you can include screenshots of your setup, the Log Analytics Workspace, and the query results showing the watchlist.)_

## Conclusion
This project helped me gain practical experience in **Azure cloud services** such as **Azure Sentinel**, **Log Analytics**, and **Azure Storage**. It also reinforced my understanding of how to manage and analyze large datasets in the cloud. This project is highly applicable to roles that require expertise in **cloud security**, **SIEM** solutions, and **log data analysis**.
7fyv h 
