---
external help file: Az.ServiceBus-help.xml
Module Name: Az.ServiceBus
online version: https://docs.microsoft.com/powershell/module/az.servicebus/new-azservicebusvirtualnetworkruleconfig
schema: 2.0.0
content_git_url: https://github.com/Azure/azure-powershell/blob/main/src/ServiceBus/ServiceBus/help/New-AzServiceBusVirtualNetworkRuleConfig.md
original_content_git_url: https://github.com/Azure/azure-powershell/blob/main/src/ServiceBus/ServiceBus/help/New-AzServiceBusVirtualNetworkRuleConfig.md
---

# New-AzServiceBusVirtualNetworkRuleConfig

## SYNOPSIS
Constructs an INwRuleSetIPRules object that can be fed as input to Set-AzServiceBusNetworkRuleSet

## SYNTAX

```
New-AzServiceBusVirtualNetworkRuleConfig -SubnetId <String> [-IgnoreMissingVnetServiceEndpoint]
 [<CommonParameters>]
```

## DESCRIPTION
Constructs an INwRuleSetIPRules object that can be fed as input to Set-AzServiceBusNetworkRuleSet

## EXAMPLES

### Example 1: Constructs an INwRuleSetVirtualNetworkRules object
```powershell
New-AzServiceBusVirtualNetworkRuleConfig -SubnetId /subscriptions/subscriptionId/resourcegroups/myResourceGroup/providers/Microsoft.Network/virtualNetworks/myVirtualNetwork/subnets/default
```

```output
IgnoreMissingVnetServiceEndpoint SubnetId
-------------------------------- --------
                                 /subscriptions/subscriptionId/resourcegroups/myResourceGroup/providers/Microsoft.Network/virtualNetworks/myVirtualNetwork/subnets/default
```

Please refer examples for Set-AzServiceBusNetworkRuleSet to know more.

## PARAMETERS

### -IgnoreMissingVnetServiceEndpoint
Resource ID of Virtual Network Subnet

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SubnetId
Resource ID of Virtual Network Subnet

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### Microsoft.Azure.PowerShell.Cmdlets.ServiceBus.Models.Api202201Preview.INwRuleSetVirtualNetworkRules

## NOTES

ALIASES

## RELATED LINKS
