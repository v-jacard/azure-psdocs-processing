---
Module Name: AzureRM.ServiceFabric
Module Guid: 60f3ba88-443f-46ff-88a3-318cfd11c1da
Locale: en-US
content_git_url: https://github.com/Azure/azure-powershell/blob/preview/src/ResourceManager/ServiceFabric/Commands.ServiceFabric/help/AzureRM.ServiceFabric.md
original_content_git_url: https://github.com/Azure/azure-powershell/blob/preview/src/ResourceManager/ServiceFabric/Commands.ServiceFabric/help/AzureRM.ServiceFabric.md
gitcommit: https://github.com/Azure/azure-powershell/blob/31afd32f413c3c88a30ab5322da0446efc925bf5
updated_at: 05/12/2017 03:05 AM
ms.date: 05/12/2017
ms.topic: conceptual
Add-AzureRmServiceFabricApplicationCertificate: Service Fabric
Add-AzureRmServiceFabricClientCertificate: Service Fabric
Add-AzureRmServiceFabricClusterCertificate: Service Fabric
Add-AzureRmServiceFabricNode: Service Fabric
Add-AzureRmServiceFabricNodeType: Service Fabric
Get-AzureRmServiceFabricCluster: Service Fabric
New-AzureRmServiceFabricCluster: Service Fabric
Remove-AzureRmServiceFabricClientCertificate: Service Fabric
Remove-AzureRmServiceFabricClusterCertificate: Service Fabric
Remove-AzureRmServiceFabricNode: Service Fabric
Remove-AzureRmServiceFabricNodeType: Service Fabric
Remove-AzureRmServiceFabricSetting: Service Fabric
Set-AzureRmServiceFabricSetting: Service Fabric
Set-AzureRmServiceFabricUpgradeType: Service Fabric
Update-AzureRmServiceFabricDurability: Service Fabric
Update-AzureRmServiceFabricReliability: Service Fabric
_isModulePage: true
---

# AzureRM.ServiceFabric Module
## Description
Azure Service Fabric Module that you can use to automate the end-2-end operations like creating a secure cluster, rolling over cluster certificates, adding or removed nodes from the cluster, etc. The complete list of all operations are listed below.

## AzureRM.ServiceFabric Cmdlets
### [Add-AzureRmServiceFabricApplicationCertificate](Add-AzureRmServiceFabricApplicationCertificate.md)
Add a certificate that will be used as application certificate

### [Add-AzureRmServiceFabricClientCertificate](Add-AzureRmServiceFabricClientCertificate.md)
Add common name or thumbprint to the cluster settings for client authentication

### [Add-AzureRmServiceFabricClusterCertificate](Add-AzureRmServiceFabricClusterCertificate.md)
Add a secondary cluster certificate to the cluster for rolling over the existing certificate 

### [Add-AzureRmServiceFabricNode](Add-AzureRmServiceFabricNode.md)
Add nodes/VMs to a specific node type to a cluster

### [Add-AzureRmServiceFabricNodeType](Add-AzureRmServiceFabricNodeType.md)
Add a node type/VMs to an existing cluster

### [Get-AzureRmServiceFabricCluster](Get-AzureRmServiceFabricCluster.md)
Get the details of the cluster resource 

### [New-AzureRmServiceFabricCluster](New-AzureRmServiceFabricCluster.md)
Create an new ServiceFabric cluster. This command has many overloads to cover various scenarios

### [Remove-AzureRmServiceFabricClientCertificate](Remove-AzureRmServiceFabricClientCertificate.md)
Remove client certificate from being used to access the cluster

### [Remove-AzureRmServiceFabricClusterCertificate](Remove-AzureRmServiceFabricClusterCertificate.md)
Remove cluster certificate from being used for cluster security

### [Remove-AzureRmServiceFabricNode](Remove-AzureRmServiceFabricNode.md)
Remove nodes from the specific node type from a cluster

### [Remove-AzureRmServiceFabricNodeType](Remove-AzureRmServiceFabricNodeType.md)
Remove a node type from a cluster

### [Remove-AzureRmServiceFabricSetting](Remove-AzureRmServiceFabricSetting.md)
Remove one or more ServiceFabric settings from the cluster

### [Set-AzureRmServiceFabricSetting](Set-AzureRmServiceFabricSetting.md)
Add or update one or more ServiceFabric settings to the cluster

### [Set-AzureRmServiceFabricUpgradeType](Set-AzureRmServiceFabricUpgradeType.md)
Change the ServiceFabric upgrade type of a cluster

### [Update-AzureRmServiceFabricDurability](Update-AzureRmServiceFabricDurability.md)
Change the durability tier of a cluster

### [Update-AzureRmServiceFabricReliability](Update-AzureRmServiceFabricReliability.md)
Change the reliability tier of a cluster
