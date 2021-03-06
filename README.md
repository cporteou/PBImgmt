# PBImgmt
Manage your PBI env VIA Powershell Script

Based on the following project: 
https://github.com/Azure-Samples/powerbi-powershell/

Please make sure that you fill in the $clientId pramater within the script.



## Prerequisites

1. Install PowerShell (https://msdn.microsoft.com/en-us/powershell/scripting/setup/installing-windows-powershell) and the Azure PowerShell cmdlets (https://docs.microsoft.com/en-us/powershell/azure/install-azurerm-ps?view=azurermps-4.4.1)

2. Fill in the parameters below

3. Run the PowerShell script



## Parameters

Please make sure that you fill in the $clientId pramater.

To set it up, go to the following page and follow the steps to provision an app https://dev.powerbi.com/apps


To get the sample to work, ensure that you have the following fields:

App Type: Native app

Redirect URL: urn:ietf:wg:oauth:2.0:oob

Level of access: all dataset APIs


## Current supported actions

**List Groups -** Lists all groups (App Workspaces)

**List Reports -** List all reports or per specifc group   

**List Datasets -** List all datasets or per specifc group    

**Clone Single Report -** Clones a selected report   

**Clone All App Reports -** Clones all the reports in an app workspace for a selected dataset

**Delete Report -** Deletes a report

**Rebind Report -** Rebinds a report to a different datasource

**Rebind Dataset -** Changes a dataset's connection string

**Get Dashboards -** Lists dashboards

**Get Tiles -** Lists dashboard tiles

## Output functionality supported

User will be presented by the following output options:

1. Output to Screen
2. Output to file location.

File location provided must be a folder. Trailing slash is handled in code.