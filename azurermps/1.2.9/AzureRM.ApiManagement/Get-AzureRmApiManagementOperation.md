---
external help file: Microsoft.Azure.Commands.ApiManagement.ServiceManagement.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 05/01/2017 21:05 PM
ms.date: 05/01/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.ApiManagement/v1.0.4.3/Get-AzureRmApiManagementOperation.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.ApiManagement/v1.0.4.3/Get-AzureRmApiManagementOperation.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/0589fbf53d27e39e0cf445261d29c64fb0859d62
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: api-Management
---

# Get-AzureRmApiManagementOperation

## SYNOPSIS
Gets a list or a particular API Operation.

## SYNTAX

### All API Operations (Default)
```
Get-AzureRmApiManagementOperation -Context <PsApiManagementContext> -ApiId <String> [<CommonParameters>]
```

### Find by ID
```
Get-AzureRmApiManagementOperation -Context <PsApiManagementContext> -ApiId <String> -OperationId <String>
 [<CommonParameters>]
```

## DESCRIPTION
Gets a list or a particular API Operation.

## EXAMPLES

### --------------------------  Example 1  --------------------------
@{paragraph=PS C:\\\>}





```
Get-AzureRmApiManagementOperation -Context $apimContext -ApiId $apiId
```

Get all API Operations.

### --------------------------  Example 2  --------------------------
@{paragraph=PS C:\\\>}





```
Get-AzureRmApiManagementOperation -Context $apimContext -ApiId $apiId -OperationId 0123456789
```

Get Operation by id.

## PARAMETERS

### -Context
Instance of PsApiManagementContext.
This parameter is required.

```yaml
Type: PsApiManagementContext
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ApiId
Identifier of API Operation belongs to.
This parameter is required.

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

### -OperationId
Identifier operation to look for.
This parameter is optional.

```yaml
Type: String
Parameter Sets: Find by ID
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### IList<Microsoft.Azure.Commands.ApiManagement.ServiceManagement.Models.PsApiManagementOperation>

### Microsoft.Azure.Commands.ApiManagement.ServiceManagement.Models.PsApiManagementOperation

## NOTES
Keywords: azure, azurerm, arm, resource, management, manager, api, apimanagement, apimgmt, apism

## RELATED LINKS

