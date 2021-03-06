---
external help file: Microsoft.ServiceFabric.Powershell.dll-Help.xml
ms.assetid: 2758DDB2-A3A0-48FF-B704-4BE8FD088B5D
online version:
schema: 2.0.0
updated_at: 05/19/2017 20:05 PM
ms.date: 05/19/2017
content_git_url: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/master/Service-Fabric-cmdlets/ServiceFabric/vlatest/New-ServiceFabricServiceGroupFromTemplate.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/master/Service-Fabric-cmdlets/ServiceFabric/vlatest/New-ServiceFabricServiceGroupFromTemplate.md
gitcommit: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/8d4c81aabdfff50fd2bedea27942bd6899fa7bd1
ms.topic: reference
author: oanapl
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: vipulm
open_to_public_contributors: false
---

# New-ServiceFabricServiceGroupFromTemplate

## SYNOPSIS
Creates a Service Fabric service group from a service template.

## SYNTAX

```
New-ServiceFabricServiceGroupFromTemplate [-ApplicationName] <Uri> [-ServiceName] <Uri>
 [-ServiceTypeName] <String> [-Force] [-ServicePackageActivationMode <ServicePackageActivationMode>]
 [-TimeoutSec <Int32>] [<CommonParameters>]
```

## DESCRIPTION
The **New-ServiceFabricServiceGroupFromTemplate** cmdlet creates a Service Fabric service group from the service template defined in the application manifest.

Before you perform any operation on a Service Fabric cluster, establish a connection to the cluster by using the [Connect-ServiceFabricCluster](./Connect-ServiceFabricCluster.md) cmdlet.

## EXAMPLES

### Example 1: Create a service group from a service group template
```
PS C:\> New-ServiceFabricServiceGroupFromTemplate -ApplicationName fabric:/myapp/persistenttodolist -ServiceName fabric:/myapp/persistenttodolist/svc4 -ServiceTypeName "PersistentToDoListServiceGroupType"
```

This command creates a Service Fabric service group that uses the service template for service type **PersistentToDoListServiceType**.
The type is defined in the application manifest for the fabric:/myapp/persistenttodolist Service Fabric application.

## PARAMETERS

### -ApplicationName
Specifies the Uniform Resource Identifier (URI) of a Service Fabric application.
The cmdlet creates a service group based on the application that has the URI that you specify.

```yaml
Type: Uri
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Force
Forces the command to run without asking for user confirmation.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ServiceName
Specifies the URI of a Service Fabric service group.

```yaml
Type: Uri
Parameter Sets: (All)
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ServicePackageActivationMode
Controls the [hosting model][1] to be used for the service. Valid values are **SharedProcess** and **ExclusiveProcess**. The default is **SharedProcess**. 

With **SharedProcess** activation mode, replicas (or instances) of different services of a given *ServiceType* will share same *ServiceHost*. With **ExclusiveProcess** activation mode, each replica or instance of a service will have its own dedicated *ServiceHost*. For more details, please see [Service Fabric Hosting Model][1].

```yaml
Type: ServicePackageActivationMode
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ServiceTypeName
Specifies the name of a Service Fabric service group type.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TimeoutSec
Specifies the time-out period, in seconds, for the operation.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None
You cannot pipe input to this cmdlet.

## OUTPUTS

### System.Object
This cmdlet returns the status of the operation as a string.

## NOTES

## RELATED LINKS

[Connect-ServiceFabricCluster](./Connect-ServiceFabricCluster.md)

[New-ServiceFabricServiceGroup](./New-ServiceFabricServiceGroup.md)