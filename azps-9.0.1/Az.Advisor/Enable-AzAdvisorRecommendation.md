---
external help file:
Module Name: Az.Advisor
online version: https://learn.microsoft.com/powershell/module/az.advisor/Enable-AzAdvisorRecommendation
schema: 2.0.0
content_git_url: https://github.com/Azure/azure-powershell/blob/main/src/Advisor/help/Enable-AzAdvisorRecommendation.md
original_content_git_url: https://github.com/Azure/azure-powershell/blob/main/src/Advisor/help/Enable-AzAdvisorRecommendation.md
---

# Enable-AzAdvisorRecommendation

## SYNOPSIS
Enables Azure Advisor recommendation(s).

> [!NOTE]
>This is the previous version of our documentation. Please consult [the most recent version](/powershell/module/az.advisor/enable-azadvisorrecommendation) for up-to-date information.

## SYNTAX

### IdParameterSet (Default)
```
Enable-AzAdvisorRecommendation -ResourceId <String> [-SubscriptionId <String[]>] [-DefaultProfile <PSObject>]
 [-Confirm] [-WhatIf] [<CommonParameters>]
```

### InputObjectParameterSet
```
Enable-AzAdvisorRecommendation -InputObject <IAdvisorIdentity> [-SubscriptionId <String[]>]
 [-DefaultProfile <PSObject>] [-Confirm] [-WhatIf] [<CommonParameters>]
```

### NameParameterSet
```
Enable-AzAdvisorRecommendation -RecommendationName <String> [-SubscriptionId <String[]>]
 [-DefaultProfile <PSObject>] [-Confirm] [-WhatIf] [<CommonParameters>]
```

## DESCRIPTION
Enables Azure Advisor recommendation(s).

## EXAMPLES

### Example 1: Enable recommendation by resource Id
```powershell
Enable-AzAdvisorRecommendation -ResourceId /subscriptions/9e223dbe-3399-4e19-88eb-0975f02ac87f/resourcegroups/automanagehcrprg/providers/microsoft.compute/virtualmachines/arcbox-capi-mgmt/providers/Microsoft.Advisor/recommendations/42963553-61de-5334-2d2e-47f3a0099d41
```

```output
Name                                 Category Resource Group   Impact ImpactedField
----                                 -------- --------------   ------ -------------
42963553-61de-5334-2d2e-47f3a0099d41 Security automanagehcrprg High   Microsoft.Compute/virtualMachines
```

Enable recommendation by resource Id

### Example 2: Enable recommendation byrecommendation name
```powershell
Enable-AzAdvisorRecommendation -RecommendationName 42963553-61de-5334-2d2e-47f3a0099d41
```

```output
Name                                 Category Resource Group   Impact ImpactedField
----                                 -------- --------------   ------ -------------
42963553-61de-5334-2d2e-47f3a0099d41 Security automanagehcrprg High   Microsoft.Compute/virtualMachines
```

Enable recommendation byrecommendation name

## PARAMETERS

### -DefaultProfile
The credentials, account, tenant, and subscription used for communication with Azure.

```yaml
Type: System.Management.Automation.PSObject
Parameter Sets: (All)
Aliases: AzureRMContext, AzureCredential

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InputObject
The powershell object type PsAzureAdvisorResourceRecommendationBase returned by Get-AzAdvisorRecommendation call.
To construct, see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: Microsoft.Azure.PowerShell.Cmdlets.Advisor.Models.IAdvisorIdentity
Parameter Sets: InputObjectParameterSet
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -RecommendationName
ResourceName of the recommendation.

```yaml
Type: System.String
Parameter Sets: NameParameterSet
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResourceId
Id of the recommendation to be suppressed.

```yaml
Type: System.String
Parameter Sets: IdParameterSet
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SubscriptionId
The Azure subscription ID.

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: (Get-AzContext).Subscription.Id
Accept pipeline input: False
Accept wildcard characters: False
```

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: System.Management.Automation.SwitchParameter
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
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Azure.PowerShell.Cmdlets.Advisor.Models.IAdvisorIdentity

## OUTPUTS

### Microsoft.Azure.PowerShell.Cmdlets.Advisor.Models.Api202001.IResourceRecommendationBase

## NOTES

ALIASES

COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.


`INPUTOBJECT <IAdvisorIdentity>`: The powershell object type PsAzureAdvisorResourceRecommendationBase returned by Get-AzAdvisorRecommendation call.
  - `[ConfigurationName <ConfigurationName?>]`: Advisor configuration name. Value must be 'default'
  - `[Id <String>]`: Resource identity path
  - `[Name <String>]`: Name of metadata entity.
  - `[OperationId <String>]`: The operation ID, which can be found from the Location field in the generate recommendation response header.
  - `[RecommendationId <String>]`: The recommendation ID.
  - `[ResourceGroup <String>]`: The name of the Azure resource group.
  - `[ResourceUri <String>]`: The fully qualified Azure Resource Manager identifier of the resource to which the recommendation applies.
  - `[SubscriptionId <String>]`: The Azure subscription ID.

## RELATED LINKS

