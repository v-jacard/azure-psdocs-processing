---
external help file: Microsoft.Azure.Commands.RecoveryServices.Backup.dll-Help.xml
ms.assetid: A10DC2A2-A732-416F-9C68-6533C143AE8F
online version:
schema: 2.0.0
content_git_url: https://github.com/Azure/azure-powershell/blob/preview/src/ResourceManager/RecoveryServices.Backup/Commands.RecoveryServices.Backup/help/Unregister-AzureRmRecoveryServicesBackupContainer.md
original_content_git_url: https://github.com/Azure/azure-powershell/blob/preview/src/ResourceManager/RecoveryServices.Backup/Commands.RecoveryServices.Backup/help/Unregister-AzureRmRecoveryServicesBackupContainer.md
gitcommit: https://github.com/Azure/azure-powershell/blob/8810c0614b76be8d014616888a4ae7733a452af9
updated_at: 05/12/2017 03:05 AM
ms.date: 05/12/2017
ms.topic: reference
---

# Unregister-AzureRmRecoveryServicesBackupContainer

## SYNOPSIS
Unregisters a Windows Server or other container from the vault.

## SYNTAX

```
Unregister-AzureRmRecoveryServicesBackupContainer [-Container] <ContainerBase> [<CommonParameters>]
```

## DESCRIPTION
The **Unregister-AzureRmRecoveryServicesBackupContainer** cmdlet unregisters a Windows Server or other Backup container from the vault.
This cmdlet removes references to a container from the vault.
Before you can unregister a container, you must delete any protected data associated with that container.

Set the vault context by using the Set-AzureRmRecoveryServicesVaultContext cmdlet before you use the current cmdlet.

## EXAMPLES

### Example 1: Unregister a Windows Server from the vault
```
PS C:\>$Cont = Get-AzureRmRecoveryServicesContainer -ContainerType "Windows" -BackupManagementType MARS -Name "server01.contoso.com"
PS C:\> Unregister-AzureRmRecoveryServiceBackupContainer -Container $Cont
```

The first command gets the Windows container named server01.contoso.com that is registered in the vault, and then stores it in the $Cont variable.

The second command unregisters the specified Windows Server from the Azure Backup vault.

## PARAMETERS

### -Container
Specifies a Backup container object to unregister.
To obtain a **BackupContainer** object, use the Get-AzureRmRecoveryServicesBackupContainer cmdlet.

```yaml
Type: ContainerBase
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
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

[Get-AzureRmRecoveryServicesBackupContainer](./Get-AzureRmRecoveryServicesBackupContainer.md)


