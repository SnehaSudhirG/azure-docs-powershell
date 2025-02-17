---
external help file: 
Module Name: Az.SecurityInsights
online version: https://docs.microsoft.com/powershell/module/az.securityinsights/invoke-azsentinelthreatintelligenceindicatorquery
schema: 2.0.0
content_git_url: https://github.com/Azure/azure-powershell/blob/main/src/SecurityInsights/help/Invoke-AzSentinelThreatIntelligenceIndicatorQuery.md
original_content_git_url: https://github.com/Azure/azure-powershell/blob/main/src/SecurityInsights/help/Invoke-AzSentinelThreatIntelligenceIndicatorQuery.md
---

# Invoke-AzSentinelThreatIntelligenceIndicatorQuery

## SYNOPSIS
Query threat intelligence indicators as per filtering criteria.

## SYNTAX

```
Invoke-AzSentinelThreatIntelligenceIndicatorQuery -ResourceGroupName <String> -WorkspaceName <String>
 [-SubscriptionId <String>] [-Id <String[]>] [-IncludeDisabled] [-Keyword <String[]>] [-MaxConfidence <Int32>]
 [-MaxValidUntil <String>] [-MinConfidence <Int32>] [-MinValidUntil <String>] [-PageSize <Int32>]
 [-PatternType <String[]>] [-SkipToken <String>] [-SortBy <IThreatIntelligenceSortingCriteria[]>]
 [-Source <String[]>] [-ThreatType <String[]>] [-DefaultProfile <PSObject>] [-Confirm] [-WhatIf]
 [<CommonParameters>]
```

## DESCRIPTION
Query threat intelligence indicators as per filtering criteria.

## EXAMPLES

### Example 1: Query all Threat Intelligence Indicators
```powershell
Invoke-AzSentinelThreatIntelligenceIndicatorQuery -ResourceGroupName "myResourceGroupName" -WorkspaceName "myWorkspaceName"
```

```output
Etag                                    Kind        Name                                    SystemDataCreatedAt SystemDataCreatedBy
----                                    ----        ----                                    ------------------- -------
"b603878e-0000-0100-0000-62d1d0010000"  indicator   f4dd9aa3-081b-2f0b-a5d7-3805954e8a39
```

This command queries TI indicators.

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

### -Id
Ids of threat intelligence indicators

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -IncludeDisabled
Parameter to include/exclude disabled indicators.

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

### -Keyword
Keywords for searching threat intelligence indicators

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MaxConfidence
Maximum confidence.

```yaml
Type: System.Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MaxValidUntil
End time for ValidUntil filter.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MinConfidence
Minimum confidence.

```yaml
Type: System.Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MinValidUntil
Start time for ValidUntil filter.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PageSize
Page size

```yaml
Type: System.Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PatternType
Pattern types

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResourceGroupName
The name of the resource group.
The name is case insensitive.

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

### -SkipToken
Skip token.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SortBy
Columns to sort by and sorting order
To construct, see NOTES section for SORTBY properties and create a hash table.

```yaml
Type: Microsoft.Azure.PowerShell.Cmdlets.SecurityInsights.Models.Api20210901Preview.IThreatIntelligenceSortingCriteria[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Source
Sources of threat intelligence indicators

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SubscriptionId
The ID of the target subscription.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: (Get-AzContext).Subscription.Id
Accept pipeline input: False
Accept wildcard characters: False
```

### -ThreatType
Threat types of threat intelligence indicators

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WorkspaceName
The name of the workspace.

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

## OUTPUTS

### Microsoft.Azure.PowerShell.Cmdlets.SecurityInsights.Models.Api20210901Preview.IThreatIntelligenceInformation

## NOTES

ALIASES

COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.


`SORTBY <IThreatIntelligenceSortingCriteria[]>`: Columns to sort by and sorting order
  - `[ItemKey <String>]`: Column name
  - `[SortOrder <ThreatIntelligenceSortingCriteriaEnum?>]`: Sorting order (ascending/descending/unsorted).

## RELATED LINKS

