---
external help file: Microsoft.Azure.Commands.ApiManagement.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 05/01/2017 21:05 PM
ms.date: 05/01/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.ApiManagement/v1.0.4.3/Set-AzureRmApiManagementVirtualNetworks.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.ApiManagement/v1.0.4.3/Set-AzureRmApiManagementVirtualNetworks.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/0589fbf53d27e39e0cf445261d29c64fb0859d62
ms.topic: reference
---

# Set-AzureRmApiManagementVirtualNetworks

## SYNOPSIS
Sets the VPN configuration for an API Management Service.

## SYNTAX

```
Set-AzureRmApiManagementVirtualNetworks -ResourceGroupName <String> -Name <String>
 [-VirtualNetworks <PsApiManagementVirtualNetwork[]>] [-PassThru] [<CommonParameters>]
```

## DESCRIPTION
The Set-AzureRmApiManagementVirtualNetworks cmdlet sets Virtual Network configuration for an API Management service.

## EXAMPLES

### Example 1: Set virtual networks for an API Management service
```
PS C:\>Set-AzureRmApiManagementVirtualNetworks -ResourceGroupName "ContosoGroup" -Name "ContosoApi" -VirtualNetworks $VirtualNetworks
```

This command sets virtual networks for an API Management service.

## PARAMETERS

### -Name
Specifies the name of an API Management service.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -PassThru
Returns an object representing the item with which you are working.
By default, this cmdlet does not generate any output.

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

### -ResourceGroupName
Specifies the name of the resource group under which the API Management service exists.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -VirtualNetworks
Specifies an array of virtual networks configurations.
Passing $null will remove the virtual network configuration.

```yaml
Type: PsApiManagementVirtualNetwork[]
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

## OUTPUTS

## NOTES

## RELATED LINKS

[New-AzureRmApiManagementVirtualNetwork]()

