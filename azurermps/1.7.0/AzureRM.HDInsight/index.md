---
Module Name: AzureRM.HDInsight
Module Guid: XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
Locale: en-US
ms.assetid: 14AE1A77-6013-4A31-8105-778DA9CCF66F
updated_at: 11/11/2016 23:11 PM
ms.date: 11/11/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.HDInsight/v1.1.4/AzureRM.HDInsight.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.HDInsight/v1.1.4/AzureRM.HDInsight.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/79eeb985ea480979357fb4695832a0c3d29a48bf
ms.topic: conceptual
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: false
Add-AzureRmHDInsightClusterIdentity: HD Monitoring
Add-AzureRmHDInsightComponentVersion: HD Monitoring
Add-AzureRmHDInsightConfigValues: HD Monitoring
Add-AzureRmHDInsightMetastore: HD Monitoring
Add-AzureRmHDInsightScriptAction: HD Monitoring
Add-AzureRmHDInsightSecurityProfile: HD Monitoring
Add-AzureRmHDInsightStorage: HD Monitoring
Get-AzureRmHDInsightCluster: HD Monitoring
Get-AzureRmHDInsightJob: HD Monitoring
Get-AzureRmHDInsightJobOutput: HD Monitoring
Get-AzureRmHDInsightPersistedScriptAction: HD Monitoring
Get-AzureRmHDInsightProperties: HD Monitoring
Get-AzureRmHDInsightScriptActionHistory: HD Monitoring
Grant-AzureRmHDInsightHttpServicesAccess: HD Monitoring
Grant-AzureRmHDInsightRdpServicesAccess: HD Monitoring
Invoke-AzureRmHDInsightHiveJob: HD Monitoring
New-AzureRmHDInsightCluster: HD Monitoring
New-AzureRmHDInsightClusterConfig: HD Monitoring
New-AzureRmHDInsightHiveJobDefinition: HD Monitoring
New-AzureRmHDInsightMapReduceJobDefinition: HD Monitoring
New-AzureRmHDInsightPigJobDefinition: HD Monitoring
New-AzureRmHDInsightSqoopJobDefinition: HD Monitoring
New-AzureRmHDInsightStreamingMapReduceJobDefinition: HD Monitoring
Remove-AzureRmHDInsightCluster: HD Monitoring
Remove-AzureRmHDInsightPersistedScriptAction: HD Monitoring
Revoke-AzureRmHDInsightHttpServicesAccess: HD Monitoring
Revoke-AzureRmHDInsightRdpServicesAccess: HD Monitoring
Set-AzureRmHDInsightClusterSize: HD Monitoring
Set-AzureRmHDInsightDefaultStorage: HD Monitoring
Set-AzureRmHDInsightPersistedScriptAction: HD Monitoring
Start-AzureRmHDInsightJob: HD Monitoring
Stop-AzureRmHDInsightJob: HD Monitoring
Submit-AzureRmHDInsightScriptAction: HD Monitoring
Use-AzureRmHDInsightCluster: HD Monitoring
Wait-AzureRmHDInsightJob: HD Monitoring
New-AzureHDInsightClusterIdentity: HD Monitoring
_isModulePage: true
---

# AzureRM.HDInsight Module
## Description
The topics in this section document the Azure PowerShell cmdlets for Microsoft Azure HDInsight in the Azure Resource Manager (ARM) framework. These cmdlets are used to manage HDInsight clusters and the jobs that run on them. The cmdlets exist in the Microsoft.Azure.Commands.HDInsight namespace.

## AzureRM.HDInsight Cmdlets
### [Add-AzureRmHDInsightClusterIdentity](./Add-AzureRmHDInsightClusterIdentity.md)
Adds a cluster identity to a cluster configuration object.


### [Add-AzureRmHDInsightConfigValues](./Add-AzureRmHDInsightConfigValues.md)
Adds a Hadoop configuration value customization and/or a Hive shared library customization to a cluster configuration object.


### [Add-AzureRmHDInsightMetastore](./Add-AzureRmHDInsightMetastore.md)
Adds a SQL Database to serve as a Hive or Oozie metastore to a cluster configuration object.


### [Add-AzureRmHDInsightScriptAction](./Add-AzureRmHDInsightScriptAction.md)
Adds a script action to a cluster configuration object.


### [Add-AzureRmHDInsightStorage](./Add-AzureRmHDInsightStorage.md)
Adds an Azure Storage key to a cluster configuration object.


### [Get-AzureRmHDInsightCluster](./Get-AzureRmHDInsightCluster.md)
Gets and lists all of the Azure HDInsight clusters associated with the current subscription or a specified resource group, or retrieves a specific cluster.


### [Get-AzureRmHDInsightJobOutput](./Get-AzureRmHDInsightJobOutput.md)
Gets the log output for a job from the storage account associated with a specified cluster.


### [Get-AzureRmHDInsightJob](./Get-AzureRmHDInsightJob.md)
Gets the list of jobs from a cluster and lists them in reverse chronological order, or retrieves a specific job.


### [Get-AzureRmHDInsightPersistedScriptAction](./Get-AzureRmHDInsightPersistedScriptAction.md)
Gets the persisted script actions for a cluster and lists them in chronological order, or gets details for a specified persisted script action.


### [Get-AzureRmHDInsightProperties](./Get-AzureRmHDInsightProperties.md)
Gets properties about the HDInsight service, such as available locations and capacity.


### [Get-AzureRmHDInsightScriptActionHistory](./Get-AzureRmHDInsightScriptActionHistory.md)
Gets the script action history for a cluster and lists it in reverse chronological order, or gets details of a previously executed script action.


### [Grant-AzureRmHDInsightHttpServicesAccess](./Grant-AzureRmHDInsightHttpServicesAccess.md)
Grants HTTP access to the cluster.


### [Grant-AzureRmHDInsightRdpServicesAccess](./Grant-AzureRmHDInsightRdpServicesAccess.md)
Grants RDP access to the Windows cluster.


### [Invoke-AzureRmHDInsightHiveJob](./Invoke-AzureRmHDInsightHiveJob.md)
Submits a Hive query to an HDInsight cluster and retrieves query results in one operation.


### [New-AzureRmHDInsightClusterConfig](./New-AzureRmHDInsightClusterConfig.md)
Creates a non-persisted cluster configuration object that describes an Azure HDInsight cluster configuration.


### [New-AzureRmHDInsightHiveJobDefinition](./New-AzureRmHDInsightHiveJobDefinition.md)
Creates a Hive job object.


### [New-AzureRmHDInsightMapReduceJobDefinition](./New-AzureRmHDInsightMapReduceJobDefinition.md)
Creates a MapReduce job object.


### [New-AzureRmHDInsightPigJobDefinition](./New-AzureRmHDInsightPigJobDefinition.md)
Creates a Pig job object.


### [New-AzureRmHDInsightSqoopJobDefinition](./New-AzureRmHDInsightSqoopJobDefinition.md)
Creates a Sqoop job object.


### [New-AzureRmHDInsightStreamingMapReduceJobDefinition](./New-AzureRmHDInsightStreamingMapReduceJobDefinition.md)
Creates a Streaming MapReduce job object.


### [Remove-AzureRmHDInsightCluster](./Remove-AzureRmHDInsightCluster.md)
Removes the specified HDInsight cluster from the current subscription.


### [Remove-AzureRmHDInsightPersistedScriptAction](./Remove-AzureRmHDInsightPersistedScriptAction.md)
Removes an persisted script action from an HDInsight cluster.


### [Revoke-AzureRmHDInsightHttpServicesAccess](./Revoke-AzureRmHDInsightHttpServicesAccess.md)
Disables HTTP access to the cluster.


### [Revoke-AzureRmHDInsightRdpServicesAccess](./Revoke-AzureRmHDInsightRdpServicesAccess.md)
Disables RDP access to a Windows cluster.


### [Set-AzureRmHDInsightClusterSize](./Set-AzureRmHDInsightClusterSize.md)
Sets the number of Worker nodes in a specified cluster.


### [Set-AzureRmHDInsightDefaultStorage](./Set-AzureRmHDInsightDefaultStorage.md)
Sets the default Storage account setting in a cluster configuration object.


### [Set-AzureRmHDInsightPersistedScriptAction](./Set-AzureRmHDInsightPersistedScriptAction.md)
Sets a previously executed script action to be a persisted script action.


### [Start-AzureRmHDInsightJob](./Start-AzureRmHDInsightJob.md)
Starts a defined Azure HDInsight job on a specified cluster.


### [Stop-AzureRmHDInsightJob](./Stop-AzureRmHDInsightJob.md)
Stops a specified running job on a cluster.


### [Submit-AzureRmHDInsightScriptAction](./Submit-AzureRmHDInsightScriptAction.md)
Submits a new script action to an Azure HDInsight cluster.


### [Use-AzureRmHDInsightCluster](./Use-AzureRmHDInsightCluster.md)
Selects a cluster to be used with the Invoke-RmAzureHDInsightHiveJob cmdlet.


### [Wait-AzureRmHDInsightJob](./Wait-AzureRmHDInsightJob.md)
Waits for the completion or failure of a specified job.


