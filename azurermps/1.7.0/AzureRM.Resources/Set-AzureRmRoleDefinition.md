---
external help file: Microsoft.Azure.Commands.Resources.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 05/02/2017 17:05 PM
ms.date: 05/02/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Resources/v2.0.3/Set-AzureRmRoleDefinition.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Resources/v2.0.3/Set-AzureRmRoleDefinition.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/fdff926f5dd35f9020f210f87b450464ba162edc
ms.topic: reference
---

# Set-AzureRmRoleDefinition

## SYNOPSIS
Modifies a custom role in Azure RBAC.
Provide the modified role definition either as a JSON file or as a PSRoleDefinition.
First, use the Get-AzureRmRoleDefinition command to retrieve the custom role that you wish to modify.
Then, modify the properties that you wish to change.
Finally, save the role definition using this command.

## SYNTAX

### InputFileParameterSet
```
Set-AzureRmRoleDefinition -InputFile <String> [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [<CommonParameters>]
```

### RoleDefinitionParameterSet
```
Set-AzureRmRoleDefinition -Role <PSRoleDefinition> [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The Set-AzureRmRoleDefinition cmdlet updates an existing custom role in Azure Role-Based Access Control.
Provide the updated role definition as an input to the command as a JSON file or a PSRoleDefinition object.
The role definition for the updated custom role MUST contain the Id and all other required properties of the role even if they are not updated: DisplayName, Description, Actions, AssignableScopes.
NotActions is optional.

Following is a sample updated role definition json for Set-AzureRmRoleDefinition

{
        "Id": "52a6cc13-ff92-47a8-a39b-2a8205c3087e",
        "Name": "Updated Role",
        "Description": "Can monitor all resources and start and restart virtual machines",
        "Actions":
        \[
            "*/read",
            "Microsoft.ClassicCompute/virtualmachines/restart/action",
            "Microsoft.ClassicCompute/virtualmachines/start/action"
        \]
        "AssignableScopes": \["/subscriptions/4004a9fd-d58e-48dc-aeb2-4a4aec58606f"\]
    }

## EXAMPLES

### --------------------------  Update using PSRoleDefinitionObject  --------------------------
@{paragraph=PS C:\\\>}



```
PS C:\> $roleDef = Get-AzureRmRoleDefinition "Contoso On-Call"
          PS C:\> $roleDef.Actions.Add("Microsoft.ClassicCompute/virtualmachines/start/action")
          PS C:\> $roleDef.Description = "Can monitor all resources and start and restart virtual machines"
          PS C:\> $roleDef.AssignableScopes = @("/subscriptions/eb910d4f-edbf-429b-94F6-d76bae7ff401", "/subscriptions/a846d197-5eac-45c7-b885-a6227fe6d388")

          PS C:\> New-AzureRmRoleDefinition -Role $roleDef
```

### --------------------------  Create using JSON file  --------------------------
@{paragraph=PS C:\\\>}



```
PS C:\> Set-AzureRmRoleDefinition -InputFile C:\Temp\roleDefinition.json
```

## PARAMETERS

### -InformationAction
@{Text=}

```yaml
Type: ActionPreference
Parameter Sets: (All)
Aliases: infa

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationVariable
@{Text=}

```yaml
Type: String
Parameter Sets: (All)
Aliases: iv

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InputFile
File name containing a single json role definition to be updated.
Only include the properties that are to be updated in the JSON.
Id property is Required.

```yaml
Type: String
Parameter Sets: InputFileParameterSet
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Role
Role definition object to be updated

```yaml
Type: PSRoleDefinition
Parameter Sets: RoleDefinitionParameterSet
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES
Keywords: azure, azurerm, arm, resource, management, manager, resource, group, template, deployment

## RELATED LINKS

[Get-AzureRmProviderOperation]()

[Get-AzureRmRoleDefinition]()

[New-AzureRmRoleDefinition]()

[Remove-AzureRmRoleDefinition]()

