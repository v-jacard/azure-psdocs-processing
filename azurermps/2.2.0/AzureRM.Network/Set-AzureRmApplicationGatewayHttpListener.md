---
external help file: Microsoft.Azure.Commands.Network.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 05/01/2017 21:05 PM
ms.date: 05/01/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/sdw-version-test/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v2.2.0/Set-AzureRmApplicationGatewayHttpListener.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/sdw-version-test/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v2.2.0/Set-AzureRmApplicationGatewayHttpListener.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/0589fbf53d27e39e0cf445261d29c64fb0859d62
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: virtual-network
---

# Set-AzureRmApplicationGatewayHttpListener

## SYNOPSIS
Modifies an HTTP listener for an application gateway.

## SYNTAX

### SetByResourceId
```
Set-AzureRmApplicationGatewayHttpListener -ApplicationGateway <PSApplicationGateway> -Name <String>
 [-FrontendIPConfigurationId <String>] [-FrontendPortId <String>] [-SslCertificateId <String>]
 [-HostName <String>] [-RequireServerNameIndication <String>] -Protocol <String> [<CommonParameters>]
```

### SetByResource
```
Set-AzureRmApplicationGatewayHttpListener -ApplicationGateway <PSApplicationGateway> -Name <String>
 [-FrontendIPConfiguration <PSApplicationGatewayFrontendIPConfiguration>]
 [-FrontendPort <PSApplicationGatewayFrontendPort>] [-SslCertificate <PSApplicationGatewaySslCertificate>]
 [-HostName <String>] [-RequireServerNameIndication <String>] -Protocol <String> [<CommonParameters>]
```

## DESCRIPTION
The Set-AzureRmApplicationGatewayHttpListener cmdlet modifies an HTTP listener for an Azure application gateway.

## EXAMPLES

### --------------------------  Example 1: Set an HTTP listener  --------------------------
@{paragraph=PS C:\\\>}



```
PS C:\>$AppGw = Get-AzureRmApplicationGateway -Name "ApplicationGateway01" -ResourceGroupName "ResourceGroup01"
PS C:\> $AppGw = Set-AzureRmApplicationGatewayHttpListener -ApplicationGateway $AppGw -Name "Listener01" -Protocol Http -FrontendIpConfiguration $FIP01 -FrontendPort 80
```

The first command gets the application gateway named ApplicationGateway01 that belongs to the resource group named ResourceGroup01 and stores it in the $AppGw variable.

## PARAMETERS

### -ApplicationGateway
Specifies the application gateway with which this cmdlet associates the HTTP listener.

```yaml
Type: PSApplicationGateway
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Name
Specifies the name of the HTTP listener.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FrontendIPConfigurationId
Specifies the ID of the front-end IP address of the application gateway.

```yaml
Type: String
Parameter Sets: SetByResourceId
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FrontendPortId
Specifies the application gateway front-end port ID.

```yaml
Type: String
Parameter Sets: SetByResourceId
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SslCertificateId
Specifies the SSL certificate ID of the HTTP listener.

```yaml
Type: String
Parameter Sets: SetByResourceId
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Protocol
Specifies the protocol that the HTTP listener uses.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FrontendIPConfiguration
Specifies the front-end IP address of the application gateway.

```yaml
Type: PSApplicationGatewayFrontendIPConfiguration
Parameter Sets: SetByResource
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FrontendPort
Specifies the application gateway front-end port.

```yaml
Type: PSApplicationGatewayFrontendPort
Parameter Sets: SetByResource
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SslCertificate
Specifies the SSL certificate of the HTTP listener.

```yaml
Type: PSApplicationGatewaySslCertificate
Parameter Sets: SetByResource
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -HostName
@{Text=}

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

### -RequireServerNameIndication
@{Text=}

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.String

### Microsoft.Azure.Commands.Network.Models.PSApplicationGatewayFrontendIPConfiguration

### Microsoft.Azure.Commands.Network.Models.PSApplicationGatewayFrontendPort

### Microsoft.Azure.Commands.Network.Models.PSApplicationGatewaySslCertificate

## OUTPUTS

### Microsoft.Azure.Commands.Network.Models.PSApplicationGateway

## NOTES
Keywords: azure, azurerm, arm, resource, management, manager, network, networking

## RELATED LINKS

[Add-AzureRmApplicationGatewayHttpListener]()

[Get-AzureRmApplicationGatewayHttpListener]()

[New-AzureRmApplicationGatewayHttpListener]()

[Remove-AzureRmApplicationGatewayHttpListener]()
