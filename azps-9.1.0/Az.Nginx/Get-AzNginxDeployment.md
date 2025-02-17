---
external help file: 
Module Name: Az.Nginx
online version: https://docs.microsoft.com/powershell/module/az.nginx/get-aznginxdeployment
schema: 2.0.0
content_git_url: https://github.com/Azure/azure-powershell/blob/main/src/Nginx/help/Get-AzNginxDeployment.md
original_content_git_url: https://github.com/Azure/azure-powershell/blob/main/src/Nginx/help/Get-AzNginxDeployment.md
---

# Get-AzNginxDeployment

## SYNOPSIS
Get the Nginx deployment

## SYNTAX

### List (Default)
```
Get-AzNginxDeployment [-SubscriptionId <String[]>] [-DefaultProfile <PSObject>] [<CommonParameters>]
```

### Get
```
Get-AzNginxDeployment -Name <String> -ResourceGroupName <String> [-SubscriptionId <String[]>]
 [-DefaultProfile <PSObject>] [<CommonParameters>]
```

### GetViaIdentity
```
Get-AzNginxDeployment -InputObject <INginxIdentity> [-DefaultProfile <PSObject>] [<CommonParameters>]
```

### List1
```
Get-AzNginxDeployment -ResourceGroupName <String> [-SubscriptionId <String[]>] [-DefaultProfile <PSObject>]
 [<CommonParameters>]
```

## DESCRIPTION
Get the Nginx deployment

## EXAMPLES

### Example 1: Get a NGINX deployment with name
```powershell
Get-AzNginxDeployment -Name nginx-test -ResourceGroupName nginx-test-rg
```

```output
Location      Name
--------      ----
westcentralus nginx-test
```

This command gets a NGINX deployment in a resource group.

### Example 2: List all NGINX deployments in a subscription
```powershell
Get-AzNginxDeployment
```

```output
Location      Name
--------      ----
westcentralus nginx-test
westcentralus nginx-test1
eastus2       nginx-test2

```

This command lists all NGINX deployments in a subscription.

### Example 3: List all NGINX deployments in a resource group
```powershell
Get-AzNginxDeployment -ResourceGroupName nginx-test-rg
```

```output
Location      Name
--------      ----
westcentralus nginx-test
westcentralus nginx-test1
```

This command lists all NGINX deployments in a resource group.

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
Identity Parameter
To construct, see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: Microsoft.Azure.PowerShell.Cmdlets.Nginx.Models.INginxIdentity
Parameter Sets: GetViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Name
The name of targeted Nginx deployment

```yaml
Type: System.String
Parameter Sets: Get
Aliases: DeploymentName

Required: True
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
Parameter Sets: Get, List1
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SubscriptionId
The ID of the target subscription.

```yaml
Type: System.String[]
Parameter Sets: Get, List, List1
Aliases:

Required: False
Position: Named
Default value: (Get-AzContext).Subscription.Id
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Azure.PowerShell.Cmdlets.Nginx.Models.INginxIdentity

## OUTPUTS

### Microsoft.Azure.PowerShell.Cmdlets.Nginx.Models.Api20220801.INginxDeployment

## NOTES

ALIASES

COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.


`INPUTOBJECT <INginxIdentity>`: Identity Parameter
  - `[CertificateName <String>]`: The name of certificate
  - `[ConfigurationName <String>]`: The name of configuration, only 'default' is supported value due to the singleton of Nginx conf
  - `[DeploymentName <String>]`: The name of targeted Nginx deployment
  - `[Id <String>]`: Resource identity path
  - `[ResourceGroupName <String>]`: The name of the resource group. The name is case insensitive.
  - `[SubscriptionId <String>]`: The ID of the target subscription.

## RELATED LINKS

