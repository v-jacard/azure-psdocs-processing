---
external help file: Microsoft.RightsManagementServices.Online.Admin.PowerShell.dll-Help.xml
online version: http://go.microsoft.com/fwlink/?LinkId=400606
schema: 2.0.0
ms.assetid: DF116EAD-6AC1-44CF-89E6-5E63D72FF58C
updated_at: 04/11/2017 21:04 PM
ms.date: 04/11/2017
content_git_url: https://github.com/Azure/azure-docs-powershell-aip/blob/master/Azure%20Information%20Protection/AADRM/vlatest/Get-Aadrm.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-aip/blob/master/Azure%20Information%20Protection/AADRM/vlatest/Get-Aadrm.md
gitcommit: https://github.com/Azure/azure-docs-powershell-aip/blob/5c9a32d3338744ea1dfb2e9f3a06cf42d59847a0
ms.topic: reference
author: cabailey
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: cabailey
open_to_public_contributors: false
---

# Get-Aadrm

## SYNOPSIS
Gets the activation status of Rights Management for your organization.

## SYNTAX

```
Get-Aadrm [<CommonParameters>]
```

## DESCRIPTION
The **Get-Aadrm** cmdlet gets the activation status of Azure Rights Management for your organization. The status of Rights Management is enabled (activated) or disabled (deactivated).

You can also view this information in a management portal. For more information, see [Activating Azure Rights Management](https://docs.microsoft.com/information-protection/deploy-use/decommission-deactivate).

## EXAMPLES

### Example 1: Get the status of Rights Management
```
PS C:\>Get-Aadrm
```

This command gets the activation status of your Rights Management service for your organization.

## PARAMETERS

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Disable-Aadrm](./Disable-Aadrm.md)

[Enable-Aadrm](./Enable-Aadrm.md)


