# Curriculum - Data Engineering Training (Azure) | Basic

## Foundations

### Setup

#### Create Azure Account

#### Install Azure Powershell

Install Azure PowerShell on your machine; instructions for installing it can be found at [https://docs.microsoft.com/en-us/powershell/azure/install-az-ps?view=azps-6.6.00](https://docs.microsoft.com/en-us/powershell/azure/install-az-ps?view=azps-6.6.00).

Run these commands to install and connect to azure:

```powershell
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
Install-Module -Name Az -Scope CurrentUser -Repository PSGallery -Force
Import-Module Az
Connect-AzAccount
```

## Azure Data Lake

### Creating and Managing Data in Azure Data Lake

[Source code](../02-data-storages/data-lakes/azure-data-lakes/lab-create-manage-data)

This lab focuses on provisioning, uploading, and managing the data life cycle in Azure Data Lake accounts.

- Recipe 1a - Provisioning an Azure storage account using the Azure portal
- Recipe 1b - Provisioning an Azure storage account using PowerShell
- Recipe 2 - Creating containers and uploading files to Azure Blob storage using PowerShell
- Recipe 3 - Managing blobs in Azure Storage using PowerShell
  - Recipe 3a - Copying blobs between containers
  - Recipe 3b - Listing blobs in an Azure storage container
  - Recipe 3c - Modifying a blob access tier
  - Recipe 3d - Downloading a blob
  - Recipe 3e - Deleting a blob
- Recipe 4 - Configuring blob lifecycle management for blob objects using the Azure portal

### Securing and Monitoring Data in Azure Data Lake

Covers securing an Azure Data Lake account using firewall and private links, accessing data lake accounts using managed identities, and monitoring an Azure Data Lake account using Azure Monitor.

## Building Data Ingestion Pipelines Using Azure Data Factory

Covers ingesting data using Azure Data Factory and copying data between Azure SQL Database and Azure Data Lake.

## Azure Data Factory Integration Runtime

Focuses on configuring and managing self-hosted integration runtimes and running SSIS packages in Azure using Azure-SSIS integration runtimes.

## Configuring and Securing Azure SQL Database

Covers configuring a Serverless SQL database, Hyperscale SQL database, and securing Azure SQL Database using virtual networks and private links.

## Implementing High Availability and Monitoring in Azure SQL Database

Explains configuring high availability to Azure SQL Database using auto-failover groups and read replicas, monitoring Azure SQL Database, and the automated scaling of Azure SQL Database during utilization spikes.

## Processing Data Using Azure Databricks

Covers integrating Azure Databricks with Azure Data Lake and Azure Key Vault, processing data using Databricks notebooks, working with Delta tables, and visualizing Delta tables using Power BI.

## Processing Data Using Azure Synapse Analytics

Covers exploring data using Synapse Serverless SQL pool, processing data using Synapse Spark Pools, Working with Synapse Lake database, and integrating Synapse Analytics with Power BI.

## Transforming Data Using Azure Synapse Dataflows

Focuses on performing transformations using Synapse Dataflows, optimizing data flows using partitioning, and managing dynamic source schema changes using schema drifting.

## Building the Serving Layer in Azure Synapse SQL Pools

Covers loading processed data into Synapse dedicated SQL pools, performing data archival using partitioning, managing table distributions, and optimizing performance using statistics and workload management.

## Monitoring Synapse SQL and Spark Pools

Covers monitoring Synapse dedicated SQL and Spark pools using Azure Log Analytics workbooks, Kusto scripts, and Azure Monitor, and monitoring Synapse dedicated SQL pools using Dynamic Management Views (DMVs).

## Optimizing and Maintaining Synapse SQL and Spark Pools

Offers techniques for tuning query performance by optimizing query plans, rebuilding replication caches and maintenance scripts to optimize Delta tables, and automatically pausing SQL pools during inactivity, among other things.

## Monitoring and Maintaining Azure Data Engineering Pipelines

Covers monitoring and managing end-to-end data engineering pipelines, which includes tracking data lineage using Microsoft Purview and improving the observability of pipeline executions using log analytics and query labeling.