---
external help file: Microsoft.Azure.Commands.TrafficManager.dll-Help.xml
online version:
schema: 2.0.0
ms.assetid: 2BA0AB11-0490-42F2-A852-A8D8AE4C2E7A
updated_at: 11/01/2016 22:11 PM
ms.date: 11/01/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.TrafficManager/v2.1.0/New-AzureRmTrafficManagerProfile.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.TrafficManager/v2.1.0/New-AzureRmTrafficManagerProfile.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/f59f3ef60bc592383812213e69fd77ba950759ed
ms.topic: reference
---

# New-AzureRmTrafficManagerProfile

## SYNOPSIS
Creates a Traffic Manager profile.

## SYNTAX

```
New-AzureRmTrafficManagerProfile -Name <String> -ResourceGroupName <String> [-ProfileStatus <String>]
 -RelativeDnsName <String> -Ttl <UInt32> -TrafficRoutingMethod <String> -MonitorProtocol <String>
 -MonitorPort <UInt32> -MonitorPath <String> [-Tag <Hashtable>] [<CommonParameters>]
```

## DESCRIPTION
The **New-AzureRmTrafficManagerProfile** cmdlet creates an Azure Traffic Manager profile.
Specify the *Name* parameter and required settings.
This cmdlet returns a local object that represents the new profile.

This cmdlet does not configure Traffic Manager endpoints.
You can update the local profile object by using the Add-AzureRmTrafficManagerEndpointConfig cmdlet.
Then upload changes to Traffic Manager by using the Set-AzureRmTrafficManagerProfile cmdlet.
Alternatively, you can add endpoints by using the New-AzureRmTrafficManagerEndpoint cmdlet.

## EXAMPLES

### Example 1: Create a profile
```
PS C:\>New-AzureRmTrafficManagerProfile -Name "ContosoProfile" -ResourceGroupName "ResourceGroup11" -ProfileStatus Enabled -TrafficRoutingMethod Performance -RelativeDnsName "contosoapp" -TTL 30 -MonitorProtocol HTTP -MonitorPort 80 -MonitorPath "/default.aspx"
```

This command creates an Azure Traffic Manager profile named ContosoProfile in resource group ResourceGroup11.
The DNS FQDN is contosoapp.trafficmanager.net.

## PARAMETERS

### -MonitorPath
Specifies the path that is used to monitor endpoint health.
Specify a value relative to the endpoint domain name.
This value must begin with a slash (/).

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

### -MonitorPort
Specifies the TCP port that is used to monitor endpoint health.
Valid values are integers from 1 through 65535.

```yaml
Type: UInt32
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MonitorProtocol
Specifies the protocol to use to monitor endpoint health.
Valid values are: 

- HTTP
- HTTPS

```yaml
Type: String
Parameter Sets: (All)
Aliases: 
Accepted values: HTTP, HTTPS

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
Specifies a name for the Traffic Manager profile that this cmdlet creates.

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

### -RelativeDnsName
Specifies the relative DNS name that this Traffic Manager profile provides.
Traffic Manager combines this value and the DNS domain name that Azure Traffic Manager uses to form the fully qualified domain name (FQDN) of the profile.

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

### -ResourceGroupName
Specifies the name of a resource group.
This cmdlet creates a Traffic Manager profile in the group that this parameter specifies.

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

### -TrafficRoutingMethod
Specifies the traffic routing method.
This method determines which endpoint Traffic Manager returns in response to incoming DNS queries.
Valid values are: 

- Performance 
- Weighted 
- Priority

```yaml
Type: String
Parameter Sets: (All)
Aliases: 
Accepted values: Performance, Weighted, Priority

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Ttl
Specifies the DNS Time to Live (TTL) value.

```yaml
Type: UInt32
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ProfileStatus
Specifies the status of the profile.
Valid values are: Enabled and Disabled.

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

### -Tag
Specifies tags as an array of hash tables.

```yaml
Type: Hashtable
Parameter Sets: (All)
Aliases: Tags

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

### Microsoft.Azure.Commands.Network.TrafficManagerProfile
This cmdlet returns a new TrafficManagerProfile object.

## NOTES

## RELATED LINKS

[Add-AzureRmTrafficManagerEndpointConfig](./Add-AzureRmTrafficManagerEndpointConfig.md)

[Disable-AzureRmTrafficManagerProfile](./Disable-AzureRmTrafficManagerProfile.md)

[Enable-AzureRmTrafficManagerProfile](./Enable-AzureRmTrafficManagerProfile.md)

[Get-AzureRmTrafficManagerProfile](./Get-AzureRmTrafficManagerProfile.md)

[Remove-AzureRmTrafficManagerProfile](./Remove-AzureRmTrafficManagerProfile.md)

[Set-AzureRmTrafficManagerProfile](./Set-AzureRmTrafficManagerProfile.md)


