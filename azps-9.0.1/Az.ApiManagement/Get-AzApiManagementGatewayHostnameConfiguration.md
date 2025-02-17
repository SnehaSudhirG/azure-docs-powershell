---
external help file: Microsoft.Azure.PowerShell.Cmdlets.ApiManagement.ServiceManagement.dll-Help.xml
Module Name: Az.ApiManagement
online version: https://learn.microsoft.com/powershell/module/az.apimanagement/get-azapimanagementgatewayhostnameconfiguration
schema: 2.0.0
content_git_url: https://github.com/Azure/azure-powershell/blob/main/src/ApiManagement/ApiManagement/help/Get-AzApiManagementGatewayHostnameConfiguration.md
original_content_git_url: https://github.com/Azure/azure-powershell/blob/main/src/ApiManagement/ApiManagement/help/Get-AzApiManagementGatewayHostnameConfiguration.md
---

# Get-AzApiManagementGatewayHostnameConfiguration

## SYNOPSIS
Gets all or specific hostname configuration for the existing Gateway.

> [!NOTE]
>This is the previous version of our documentation. Please consult [the most recent version](/powershell/module/az.apimanagement/get-azapimanagementgatewayhostnameconfiguration) for up-to-date information.

## SYNTAX

### GetByGatewayId (Default)
```
Get-AzApiManagementGatewayHostnameConfiguration -Context <PsApiManagementContext> -GatewayId <String>
 [-DefaultProfile <IAzureContextContainer>] [<CommonParameters>]
```

### GetByGatewayHostnameId
```
Get-AzApiManagementGatewayHostnameConfiguration -Context <PsApiManagementContext> -GatewayId <String>
 -GatewayHostnameConfigurationId <String> [-DefaultProfile <IAzureContextContainer>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzApiManagementGatewayHostnameConfiguration** cmdlet gets all or specific hostname configuration for the existing Gateway.

## EXAMPLES

### Example 1: Get all hostname configurations for the gateway
```powershell
$apimContext = New-AzApiManagementContext -ResourceGroupName "Api-Default-WestUS" -ServiceName "contoso"
Get-AzApiManagementGatewayHostnameConfiguration -Context $apimContext  -GatewayId "0123456789"
```

This command gets all hostname configurations for a "0123456789" gateway.

### Example 2: Get a hostname configuration for the gateway
```powershell
$apimContext = New-AzApiManagementContext -ResourceGroupName "Api-Default-WestUS" -ServiceName "contoso"
Get-AzApiManagementGatewayHostnameConfiguration -Context $apimContext -GatewayId "0123456789" -GatewayHostnameConfigurationId "123"
```

This command gets "123" hostname configuration for a "0123456789" gateway.

## PARAMETERS

### -Context
Instance of PsApiManagementContext.
This parameter is required.

```yaml
Type: Microsoft.Azure.Commands.ApiManagement.ServiceManagement.Models.PsApiManagementContext
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -DefaultProfile
The credentials, account, tenant, and subscription used for communication with Azure.

```yaml
Type: Microsoft.Azure.Commands.Common.Authentication.Abstractions.Core.IAzureContextContainer
Parameter Sets: (All)
Aliases: AzContext, AzureRmContext, AzureCredential

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -GatewayHostnameConfigurationId
Hostname Configuration identifier.
This parameter is optional.

```yaml
Type: System.String
Parameter Sets: GetByGatewayHostnameId
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -GatewayId
Gateway identifier.
This parameter is required.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Azure.Commands.ApiManagement.ServiceManagement.Models.PsApiManagementContext

### System.String

## OUTPUTS

### Microsoft.Azure.Commands.ApiManagement.ServiceManagement.Models.PsApiManagementGatewayHostnameConfiguration

## NOTES

## RELATED LINKS
