---
external help file: Microsoft.Azure.Commands.Resources.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 05/02/2017 17:05 PM
ms.date: 05/02/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Resources/v2.0.3/New-AzureRmADServicePrincipal.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Resources/v2.0.3/New-AzureRmADServicePrincipal.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/fdff926f5dd35f9020f210f87b450464ba162edc
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: azure-resource-manager
---

# New-AzureRmADServicePrincipal

## SYNOPSIS
Creates a new azure active directory service principal.

## SYNTAX

```
New-AzureRmADServicePrincipal -ApplicationId <Guid> [-DisableAccount] [<CommonParameters>]
```

## DESCRIPTION
Creates a new azure active directory service principal.

## EXAMPLES

### --------------------------  Create new AAD service principal.  --------------------------
@{paragraph=PS C:\\\>}



```
New-AzureRmADServicePrincipal -ApplicationId a3dad041-8119-4182-b500-f8f959bf31db
```

Creates a new azure active directory service principal.

DisplayName                    Type                           ObjectId
-----------                    ----                           --------
NewApplication                                                61b5d8ea-fdc6-40a2-8d5b-ad447c678d45

## PARAMETERS

### -ApplicationId
@{Text=}

```yaml
Type: Guid
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -DisableAccount
@{Text=}

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

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

## NOTES
Keywords: azure, azurerm, arm, resource, management, manager, resource, group, template, deployment

## RELATED LINKS

[Remove-AzureRmADServicePrincipal]()

[Get-AzureRmADServicePrincipal]()

[New-AzureRmADApplication]()

[Remove-AzureRmADApplication]()

