---
external help file: Microsoft.Azure.Commands.ServiceFabric.dll-Help.xml
online version:
schema: 2.0.0
content_git_url: https://github.com/Azure/azure-powershell/blob/preview/src/ResourceManager/ServiceFabric/Commands.ServiceFabric/help/Get-AzureRmServiceFabricCluster.md
original_content_git_url: https://github.com/Azure/azure-powershell/blob/preview/src/ResourceManager/ServiceFabric/Commands.ServiceFabric/help/Get-AzureRmServiceFabricCluster.md
gitcommit: https://github.com/Azure/azure-powershell/blob/18f30b6ac812908643ec13e91c827df3fc1840a3
updated_at: 05/12/2017 03:05 AM
ms.date: 05/12/2017
ms.topic: reference
---

# Get-AzureRmServiceFabricCluster

## SYNOPSIS
Get the cluster resource details.

## SYNTAX

```
Get-AzureRmServiceFabricCluster [[-ResourceGroupName] <String>] [[-Name] <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Add-AzureRmServiceFabricCluster** will get the cluster resource details.

## EXAMPLES

### Example 1
```
PS C:\> Get-AzureRmServiceFabricCluster -ResourceGroupName 'Group1' -ClusterName 'Contoso01SFCluster'
```

This command will get the cluster resource details for cluster 'myCluster'.

## PARAMETERS

### -Name
Specify the name of the cluster.

```yaml
Type: String
Parameter Sets: (All)
Aliases: ClusterName

Required: False
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of the resource group.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.String

## OUTPUTS

### System.Collections.Generic.IList`1[[Microsoft.Azure.Commands.ServiceFabric.Models.PsCluster, Microsoft.Azure.Commands.ServiceFabric, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null]]

## NOTES

## RELATED LINKS

