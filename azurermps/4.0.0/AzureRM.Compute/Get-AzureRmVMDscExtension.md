---
external help file: Microsoft.Azure.Commands.Compute.dll-Help.xml
ms.assetid: 5B7A1BE6-F5F5-4968-BE32-7743D0E25FE3
online version:
schema: 2.0.0
content_git_url: https://github.com/Azure/azure-powershell/blob/preview/src/ResourceManager/Compute/Commands.Compute/help/Get-AzureRmVMDscExtension.md
original_content_git_url: https://github.com/Azure/azure-powershell/blob/preview/src/ResourceManager/Compute/Commands.Compute/help/Get-AzureRmVMDscExtension.md
gitcommit: https://github.com/Azure/azure-powershell/blob/8810c0614b76be8d014616888a4ae7733a452af9
updated_at: 05/12/2017 03:05 AM
ms.date: 05/12/2017
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: big-compute
---

# Get-AzureRmVMDscExtension

## SYNOPSIS
Gets the settings of the DSC extension on a particular virtual machine.

## SYNTAX

```
Get-AzureRmVMDscExtension [-ResourceGroupName] <String> [-VMName] <String> [[-Name] <String>] [-Status]
 [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmVMDscExtension** cmdlet gets the settings of the Desired State Configuration (DSC) extension on a particular virtual machine.

## EXAMPLES

### Example 1: Get the settings of a DSC extension
```
PS C:\>Get-AzureRmVMDscExtension -ResourceGroupName "ResourceGroup002" -VMName "VM07" -Name "DSC"
```

This command gets the settings of extension named DSC on the virtual machine named VM07.

## PARAMETERS

### -Name
Specifies the name of the Azure Resource Manager resource that represents the extension.
The Set-AzureRmVMDscExtension cmdlet sets this name to Microsoft.Powershell.DSC, which is the same value that is used by **Get-AzureRmVMDscExtension**.
Specify this parameter only if you changed the default name in the **Set-AzureRmVMDscExtension** cmdlet or used a different resource name in a Resource Manager template.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of the resource group of the virtual machine.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Status
Indicates that this cmdlet gets the instance view of the DSC extension.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -VMName
Specifies the name of a virtual machine for which this cmdlet gets the DSC extension.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### Microsoft.Azure.Commands.Compute.Extension.DSC.VirtualMachineDscExtensionContext

## NOTES

## RELATED LINKS

[Remove-AzureRmVMDscExtension](./Remove-AzureRmVMDscExtension.md)

[Set-AzureRmVMDscExtension](./Set-AzureRmVMDscExtension.md)

