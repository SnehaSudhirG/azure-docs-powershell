---
external help file:
Module Name: Az.Quota
online version: https://learn.microsoft.com/powershell/module/az.Quota/New-AzQuotaLimitObject
schema: 2.0.0
content_git_url: https://github.com/Azure/azure-powershell/blob/main/src/Quota/help/New-AzQuotaLimitObject.md
original_content_git_url: https://github.com/Azure/azure-powershell/blob/main/src/Quota/help/New-AzQuotaLimitObject.md
---

# New-AzQuotaLimitObject

## SYNOPSIS
Create an in-memory object for LimitObject.

> [!NOTE]
>This is the previous version of our documentation. Please consult [the most recent version](/powershell/module/az.quota/new-azquotalimitobject) for up-to-date information.

## SYNTAX

```
New-AzQuotaLimitObject -Value <Int32> [-LimitType <QuotaLimitTypes>] [<CommonParameters>]
```

## DESCRIPTION
Create an in-memory object for LimitObject.

## EXAMPLES

### Example 1: Create an in-memory object for LimitValue
```powershell
New-AzQuotaLimitObject -Value 1003
```

```output
LimitObjectType LimitType Value
--------------- --------- -----
LimitValue                1003
```

This command create an in-memory object for LimitValue as value of the parameter Limit in the New/Update-AzQuota cmdlet.

## PARAMETERS

### -LimitType
The quota or usages limit types.

```yaml
Type: Microsoft.Azure.PowerShell.Cmdlets.Quota.Support.QuotaLimitTypes
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Value
The quota/limit value.

```yaml
Type: System.Int32
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

### Microsoft.Azure.PowerShell.Cmdlets.Quota.Models.Api20210315Preview.LimitObject

## NOTES

ALIASES

## RELATED LINKS

