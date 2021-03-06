---
external help file: Microsoft.Azure.Commands.KeyVault.dll-Help.xml
ms.assetid: 2730C538-0318-4E98-ABC5-01D5F8C0DDCD
online version:
schema: 2.0.0
updated_at: 05/01/2017 21:05 PM
ms.date: 05/01/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.KeyVault/v1.1.11/Backup-AzureKeyVaultKey.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.KeyVault/v1.1.11/Backup-AzureKeyVaultKey.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/0589fbf53d27e39e0cf445261d29c64fb0859d62
ms.topic: reference
---

# Backup-AzureKeyVaultKey

## SYNOPSIS
Backs up a key in a key vault.

## SYNTAX

```
Backup-AzureKeyVaultKey [-VaultName] <String> [-Name] <String> [[-OutputFile] <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Backup-AzureKeyVaultKey** cmdlet backs up a specified key in a key vault by downloading it and storing it in a file.
If there are multiple versions of the key, all versions are included in the backup.
Because the downloaded content is encrypted, it cannot be used outside of azure_key_vault.
You can restore a backed-up key to any key vault in the subscription that it was backed up from.

Typical reasons to use this cmdlet are: 

- You want to escrow a copy of your key, so that you have an offline copy in case you accidentally delete your key in your key vault.
 
- You created a key using Key Vault and now want to clone the key into a different Azure region, so that you can use it from all instances of your distributed application.
Use the **Backup-AzureKeyVaultKey** cmdlet to retrieve the key in encrypted format and then use the Restore-AzureKeyVaultKey cmdlet and specify a key vault in the second region.

## EXAMPLES

### Example 1: Back up a key with an automatically generated file name
```
PS C:\>Backup-AzureKeyVaultKey -VaultName 'MyKeyVault' -Name 'MyKey'
```

This command retrieves the key named MyKey from the key vault named MyKeyVault and saves a backup of that key to a file that is automatically named for you, and displays the file name.

### Example 2: Back up a key to a specified file name
```
PS C:\>Backup-AzureKeyVaultKey -VaultName 'MyKeyVault' -Name 'MyKey' -OutputFile 'C:\Backup.blob'
```

This command retrieves the key named MyKey from the key vaultnamed MyKeyVault and saves a backup of that key to a file named Backup.blob.

## PARAMETERS

### -Name
Specifies the name of the key to back up.

```yaml
Type: String
Parameter Sets: (All)
Aliases: KeyName

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -OutputFile
Specifies the output file in which the backup blob is stored.
If you do not specify this parameter, this cmdlet generates a file name for you.
If you specify the name of an existing output file, the operation will not complete and returns an error message that the backup file already exists.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 3
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -VaultName
Specifies the name of the key vault that contains the key to back up.

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

## NOTES

## RELATED LINKS

[Add-AzureKeyVaultKey](./Add-AzureKeyVaultKey.md)

[Get-AzureKeyVaultKey](./Get-AzureKeyVaultKey.md)

[Remove-AzureKeyVaultKey](./Remove-AzureKeyVaultKey.md)

[Restore-AzureKeyVaultKey](./Restore-AzureKeyVaultKey.md)


