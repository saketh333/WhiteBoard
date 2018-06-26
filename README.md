 # WhiteBoard


## PowerBi
 
Drill down - to go down a hierarchy if available

Slicer - Is just like the filter in tableau

## Churning

To understand why customers churn, it's important to understand churn drivers

https://docs.microsoft.com/en-us/azure/machine-learning/studio/sample-experiments Azure | sample churn model
https://gallery.azure.ai/Collection/Retail-Customer-Churn-Prediction-Template-1 | sample template

## Azure Data Factory

## Logic App

06/26/2018 - creating a logic app for processing email attachments and storing it on a blob. 

https://docs.microsoft.com/en-us/azure/logic-apps/tutorial-process-email-attachments-workflow#create-blobs-for-attachments

## SSIS

Jun 11 2018

* Created a package that would download data from azure blob storage to local file storage
* These files are processed locally using Foreach loop container and a derived column for processing time
* This cleaned data is loaded into Azure Sql database

Create a Console app from Project Pane - this app is configured to run the package on virtual machine

A configuration file is used to configure account name | passwords for database connection manager and locations for file
connection manager


# Installation Order

1. Sql Server Express

2. Sql Server Management Studio

3. Visual Studio Professional

4. SQl Server Data Tools

5. Azure Storage Explorer

6. SSIS Azure Feature Pack

*Updates can brick ssdt tools
