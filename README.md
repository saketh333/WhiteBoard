# WhiteBoard

## PowerBi
 
Drill down - to go down a hierarchy if available

Slicer - Is an Interactive visualization for selecting data

Filter - Visual, Page, Report, Advanced Filters (relative time, text based filtering)

DrillThrough Filters allows to focus on specific information per record

Grouping data

__Sharing Reports__

Embed in a Sharepoint Site

Share Public to anyone on internet - no pro account needed (delete it to remove it from web)

Share using PowerBi - does need pro account

Power point - static

## Churning

To understand why customers churn, it's important to understand churn drivers

https://docs.microsoft.com/en-us/azure/machine-learning/studio/sample-experiments Azure | sample churn model
https://gallery.azure.ai/Collection/Retail-Customer-Churn-Prediction-Template-1 | sample template

https://jungleworks.com/predictive-analytics-reduce-churn/
https://datascienceplus.com/predict-customer-churn-logistic-regression-decision-tree-and-random-forest/
https://www.datascience.com/blog/feature-engineering-for-churn-modeling


## Azure Data Factory

For building data pipelines that pull data from source transform and store

lift and shift ssis packages using adf Integration runtime

monitoring execution, triggers!

## Logic App

06/26/2018 - creating a logic app for processing email attachments and storing it on a Azure blob storage. 

https://docs.microsoft.com/en-us/azure/logic-apps/tutorial-process-email-attachments-workflow#create-blobs-for-attachments

Functions
https://docs.microsoft.com/en-us/azure/logic-apps/workflow-definition-language-functions-reference

## SSIS

Jun 11 2018

* Created a package that would download data from azure blob storage to local file storage
* These files are processed locally using Foreach loop container and a derived column for processing time
* This cleaned data is loaded into Azure Sql database

Create a Console app from Project Pane - this app is configured to run the package on virtual machine

A configuration file is used to configure account name | passwords for database connection manager and locations for file
connection manager

# Installation Order

June 16 2018

1. Sql Server Express

2. Sql Server Management Studio

3. Visual Studio Professional

4. SQl Server Data Tools

5. Azure Storage Explorer

6. SSIS Azure Feature Pack

*Updates can brick ssdt tools


## .Net

.Net is a platform that allows various languages to write code and integrate into a common place

.NET Framework is a software framework developed by Microsoft that runs primarily on Microsoft Windows. It includes a large class library named Framework Class Library and provides language interoperability across several programming languages. Source: __Wikipedia

__Powershell__

Using Powershell script to delete all files in the container matching a naming pattern

__Script__
$context = New-AzureStorageContext -StorageAccountName "account name" -StorageAccountKey "account key"

Get-AzureStorageBlob -Container "containername" -blob *test.zip -Context $context | ForEach-Object {Remove-AzureStorageBlob -Blob $_.Name -Container "containername" -Context $context}


https://blogs.msdn.microsoft.com/ssis/2017/01/26/run-powershell-scripts-in-ssis/

## Visual Studio

__Version Control with Visual Studio__

2 source control options
Team Foundation version control (TFVC)
GIT

https://docs.microsoft.com/en-us/vsts/user-guide/work-team-explorer?view=vsts


## Python
Different Functions used

pd.to_csv()

pd.merge()

pd.DataFrame()

df.value_counts()

df.groupby()

df.groupby().agg()

df.groupby().count()

df.reset_index(drop = True)

df.loc[row_indexer,column_indexer]=value

os.listdir()

os.chdir()

string.strip()


## Congnitive Engineering

While Making Reports in Power Bi will be using these 

Gestalt Principles
Encoding
Patterns

#August

## Runbooks
Running powershell scripts inside runbooks

A script that takes in date and goes back three weeks and gets files from the web using wget and writes the file to azure blob storage

blobstorage -force and also set blob for uploading data

## Logic apps
using recurrence trigger
for downloading files from ftp and sftp extracting, creating blob, organizing and running data factory pipelines from logic apps
