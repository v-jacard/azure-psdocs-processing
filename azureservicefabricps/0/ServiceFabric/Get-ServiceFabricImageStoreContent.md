---
external help file: Microsoft.ServiceFabric.Powershell.dll-Help.xml
ms.assetid: DD60B18E-5ED7-41B6-B9D4-38BD726DCFF2
online version:
schema: 2.0.0
updated_at: 05/19/2017 20:05 PM
ms.date: 05/19/2017
content_git_url: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/master/Service-Fabric-cmdlets/ServiceFabric/vlatest/Get-ServiceFabricImageStoreContent.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/master/Service-Fabric-cmdlets/ServiceFabric/vlatest/Get-ServiceFabricImageStoreContent.md
gitcommit: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/8d4c81aabdfff50fd2bedea27942bd6899fa7bd1
ms.topic: reference
author: oanapl
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: vipulm
open_to_public_contributors: false
---

# Get-ServiceFabricImageStoreContent

## SYNOPSIS
Gets image store content information

## SYNTAX

### Application
```
Get-ServiceFabricImageStoreContent -ApplicationTypeName <String> [-ApplicationTypeVersion <String>]
 [-ImageStoreConnectionString <String>] [-CertStoreLocation <StoreLocation>] [-TimeoutSec <Int32>]
 [<CommonParameters>]
```

### Path
```
Get-ServiceFabricImageStoreContent [-RemoteRelativePath <String>] [-ImageStoreConnectionString <String>]
 [-CertStoreLocation <StoreLocation>] [-TimeoutSec <Int32>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-ServiceFabricImageStoreContent** cmdlet gets information about image store content being organized either within the given image store relative path or belong to the specified application type/version.

## EXAMPLES

### Example 1: Get image store content by application type/version
```
PS C:\> Get-ServiceFabricImageStoreContent -Application -ApplicationTypeName "CalcServiceApp" -ApplicationTypeVersion "2.0" -ImageStoreConnectionString "fabric:ImageStore"
```

This command gets information about image store content belongs to the application CalcServiceApp, type version 2.0.

### Example 2: Get image store content by relative path
```
PS C:\> Get-ServiceFabricImageStoreContent -Path -RemoteRelativePath "Store\CalcServiceApp\apps" -ImageStoreConnectionString "fabric:ImageStore"
```

This command gets information about image store content within the specified image store relative path "Store\CalcServiceApp\apps".

## PARAMETERS

### -ApplicationTypeName
Specifies the name of a Service Fabric application type.

```yaml
Type: String
Parameter Sets: Application
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ApplicationTypeVersion
Specifies the version of a Service Fabric application type.

```yaml
Type: String
Parameter Sets: Application
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CertStoreLocation
{{Fill CertStoreLocation Description}}

```yaml
Type: StoreLocation
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ImageStoreConnectionString
Specifies the connection string for the Service Fabric image store.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RemoteRelativePath
Specifies the relative path to the image store root.

```yaml
Type: String
Parameter Sets: Path
Aliases: 

Required: False
Position: Named
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
The cmdlet **Get-ServiceFabricStoreContent** accepts string instances of a Service Fabric application type; the version of an application type; or the image store relative path.

## OUTPUTS

### None
The cmdlet **Get-ServiceFabricStoreContent** returns instances of the  **System.Fabric.Management.ImageStore.ImageStoreFile** object and/or the **System.Fabric.Management.ImageStore.ImageStoreFolder** object.

## NOTES

## RELATED LINKS

