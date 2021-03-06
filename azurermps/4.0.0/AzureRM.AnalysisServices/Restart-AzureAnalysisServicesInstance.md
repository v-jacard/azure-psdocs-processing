---
external help file: Microsoft.Azure.Commands.AnalysisServices.Dataplane.dll-Help.xml
online version:
schema: 2.0.0
content_git_url: https://github.com/Azure/azure-powershell/blob/preview/src/ResourceManager/AnalysisServices/Commands.AnalysisServices.Dataplane/help/Restart-AzureAnalysisServicesInstance.md
original_content_git_url: https://github.com/Azure/azure-powershell/blob/preview/src/ResourceManager/AnalysisServices/Commands.AnalysisServices.Dataplane/help/Restart-AzureAnalysisServicesInstance.md
gitcommit: https://github.com/Azure/azure-powershell/blob/2526f281fe0af40ef67662068fdbfa4ba9e7db43
updated_at: 05/10/2017 19:05 PM
ms.date: 05/10/2017
ms.topic: reference
---

# Restart-AzureAnalysisServicesInstance

## SYNOPSIS
Restarts an instance of Analysis Services server in the currently logged in Environment as specified in Add-AzureAnalysisServicesAccount command

## SYNTAX

```
Restart-AzureAnalysisServicesInstance [-Instance] <String> [-PassThru] [-WhatIf] [-Confirm]
```

## DESCRIPTION
The Restart-AzureAnalysisServicesInstance cmdlet restarts an instance of Azure Analysis Services server

## EXAMPLES

### Example 1
```
PS C:\>Restart-AzureAnalysisServicesInstance
Instance: testserver
```

This command will restart the server 'testserver' in the environment specified in the Add-AzureAnalysisServicesAccount command

## PARAMETERS

### -Instance
Name of the Analysis Services server instance to restart

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PassThru
Specifying this will return true if the command was successful.

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

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

## NOTES
Alias: Restart-AzureAsInstance

## RELATED LINKS

