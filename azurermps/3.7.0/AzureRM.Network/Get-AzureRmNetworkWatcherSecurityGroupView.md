---
external help file: Microsoft.Azure.Commands.Network.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 03/11/2017 02:03 AM
ms.date: 03/11/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v3.6.0/Get-AzureRmNetworkWatcherSecurityGroupView.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v3.6.0/Get-AzureRmNetworkWatcherSecurityGroupView.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/04f63f6e685743ace2c57eb157574e34e8610b1c
ms.topic: reference
---

# Get-AzureRmNetworkWatcherSecurityGroupView

## SYNOPSIS
View the configured and effective network security group rules applied on a VM.

## SYNTAX

### SetByResource (Default)
```
Get-AzureRmNetworkWatcherSecurityGroupView -NetworkWatcher <PSNetworkWatcher> -TargetVirtualMachineId <String>
```

### SetByName
```
Get-AzureRmNetworkWatcherSecurityGroupView -NetworkWatcherName <String> -ResourceGroupName <String>
 -TargetVirtualMachineId <String>
```

## DESCRIPTION
The Get-AzureRmNetworkWatcherSecurityGroupView enables you to view the configured and effective network security group rules applied on a VM.

## EXAMPLES

### --- Example 1: Make a Security Group View call on a VM ---

```
$nw = Get-AzurermResource | Where {$_.ResourceType -eq "Microsoft.Network/networkWatchers" -and $_.Location -eq "WestCentralUS" } 
$networkWatcher = Get-AzureRmNetworkWatcher -Name $nw.Name -ResourceGroupName $nw.ResourceGroupName 
$VM = Get-AzurermVM -ResourceGroupName ContosoResourceGroup -Name VM0 
Get-AzureRmNetworkWatcherSecurityGroupView -NetworkWatcher $networkWatcher -TargetVirtualMachineId $VM.Id

```
In the above example, we first get the regional Network Watcher, then a VM in the region. 
Then we make a Security Group View call on the specified VM.

## PARAMETERS

### -NetworkWatcher
The network watcher resource.

```yaml
Type: PSNetworkWatcher
Parameter Sets: SetByResource
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -NetworkWatcherName
The name of network watcher.

```yaml
Type: String
Parameter Sets: SetByName
Aliases: Name

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ResourceGroupName
The name of the network watcher resource group.

```yaml
Type: String
Parameter Sets: SetByName
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -TargetVirtualMachineId
The target VM Id

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

## INPUTS

### Microsoft.Azure.Commands.Network.Models.PSNetworkWatcher
System.String

## OUTPUTS

### Microsoft.Azure.Commands.Network.Models.PSViewNsgRules

## NOTES
Keywords: azure, azurerm, arm, resource, management, manager, network, networking, network watcher, flow, ip 

## RELATED LINKS
[New-AzureRmNetworkWatcher]()
[Get-AzureRmNetworkWatcher]()
[Remove-AzureRmNetworkWatcher]()

[Test-AzureRmNetworkWatcherIPFlow]()
[Get-AzureRmNetworkWatcherNextHop]()
[Get-AzureRmNetworkWatcherTopology]()
[Start-AzureRmNetworkWatcherResourceTroubleshooting]()

[New-AzureRmNetworkWatcherPacketCapture]()
[New-AzureRmPacketCaptureFilterConfig]()
[Get-AzureRmNetworkWatcherPacketCapture]()
[Remove-AzureRmNetworkWatcherPacketCapture]()
[Stop-AzureRmNetworkWatcherPacketCapture]()

