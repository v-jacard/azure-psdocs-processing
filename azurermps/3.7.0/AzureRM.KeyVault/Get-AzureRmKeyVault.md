---
external help file: Microsoft.Azure.Commands.KeyVault.dll-Help.xml
ms.assetid: A7C287C4-E9FD-407A-91BD-EFA17C33FC8B
online version: http://go.microsoft.com/fwlink/?LinkID=690161
schema: 2.0.0
updated_at: 03/11/2017 02:03 AM
ms.date: 03/11/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.KeyVault/v2.7.0/Get-AzureRmKeyVault.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.KeyVault/v2.7.0/Get-AzureRmKeyVault.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/04f63f6e685743ace2c57eb157574e34e8610b1c
ms.topic: reference
---

# Get-AzureRmKeyVault

## SYNOPSIS
Gets key vaults.

## SYNTAX

### GetVaultByName
```
Get-AzureRmKeyVault [-VaultName] <String> [[-ResourceGroupName] <String>] [<CommonParameters>]
```

### ListVaultsByResourceGroup
```
Get-AzureRmKeyVault [-ResourceGroupName] <String> [<CommonParameters>]
```

### ListAllVaultsInSubscription
```
Get-AzureRmKeyVault [-Tag <Hashtable>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmKeyVault** cmdlet gets information about the key vaults in a subscription.
You can view all key vaults instances in a subscription, or filter your results by a resource group or a particular key vault.

Note that although specifying the resource group is optional for this cmdlet when you get a single key vault, you should do so for better performance.

## EXAMPLES

### Example 1: Get all key vaults in your current subscription
```
PS C:\>Get-AzureRMKeyVault
```

This command gets all the key vaults in your current subscription.

### Example 2: Get a specific key vault
```
PS C:\>$MyVault = Get-AzureRMKeyVault -VaultName 'Contoso03Vault'
```

This command gets the key vault named Contoso03Vault in your current subscription, and then stores it in the $MyVault variable.
You can inspect the properties of $MyVault to get details about the key vault.

### Example 3: Get key vaults in a resource group
```
PS C:\>Get-AzureRMKeyVault -ResourceGroupName 'ContosoPayRollResourceGroup'
```

This command gets all the key vaults in the resource group named ContosoPayRollResourceGroup.

## PARAMETERS

### -ResourceGroupName
Specifies the name of the resource group associated with the key vault or key vaults being queried.

```yaml
Type: String
Parameter Sets: GetVaultByName
Aliases: 

Required: False
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

```yaml
Type: String
Parameter Sets: ListVaultsByResourceGroup
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Tag
Specifies the key and value of the specified tag to filter the list of key vaults by hash table.

```yaml
Type: Hashtable
Parameter Sets: ListAllVaultsInSubscription
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -VaultName
Specifies the name of the key vault.

```yaml
Type: String
Parameter Sets: GetVaultByName
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

## NOTES

## RELATED LINKS

[New-AzureRmKeyVault](./New-AzureRmKeyVault.md)

[Remove-AzureRmKeyVault](./Remove-AzureRmKeyVault.md)

