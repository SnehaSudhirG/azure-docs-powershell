---
external help file:
Module Name: Az.VMware
online version: https://learn.microsoft.com/powershell/module/az.VMware/new-AzVMwareAddonSrmPropertiesObject
schema: 2.0.0
content_git_url: https://github.com/Azure/azure-powershell/blob/main/src/VMware/help/New-AzVMwareAddonSrmPropertiesObject.md
original_content_git_url: https://github.com/Azure/azure-powershell/blob/main/src/VMware/help/New-AzVMwareAddonSrmPropertiesObject.md
---

# New-AzVMwareAddonSrmPropertiesObject

## SYNOPSIS
Create a in-memory object for AddonSrmProperties

> [!NOTE]
>This is the previous version of our documentation. Please consult [the most recent version](/powershell/module/az.vmware/new-azvmwareaddonsrmpropertiesobject) for up-to-date information.

## SYNTAX

```
New-AzVMwareAddonSrmPropertiesObject -LicenseKey <String> [<CommonParameters>]
```

## DESCRIPTION
Create a in-memory object for AddonSrmProperties

## EXAMPLES

### Example 1: Create a local SRM object for the Addon Property parameter
```powershell
New-AzVMwareAddonSrmPropertiesObject -LicenseKey "YourLicenseKeyValue"
```
```output
AddonType ProvisioningState LicenseKey
--------- ----------------- ----------
SRM                         YourLicenseKeyValue
```

Create a local SRM object for the Addon Property parameter

## PARAMETERS

### -LicenseKey
The Site Recovery Manager (SRM) license.

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

### Microsoft.Azure.PowerShell.Cmdlets.VMware.Models.Api20211201.AddonSrmProperties

## NOTES

ALIASES

## RELATED LINKS

