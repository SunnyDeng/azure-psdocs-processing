---
external help file: Microsoft.Azure.Commands.SiteRecovery.dll-Help.xml
ms.assetid: 133668A0-0D11-4034-A743-4C0D3CE0FAF1
online version:
schema: 2.0.0
content_git_url: https://github.com/Azure/azure-powershell/blob/preview/src/ResourceManager/SiteRecovery/Commands.SiteRecovery/help/Set-AzureRmSiteRecoveryVaultSettings.md
original_content_git_url: https://github.com/Azure/azure-powershell/blob/preview/src/ResourceManager/SiteRecovery/Commands.SiteRecovery/help/Set-AzureRmSiteRecoveryVaultSettings.md
gitcommit: https://github.com/Azure/azure-powershell/blob/94e42834e29c78cafba9e3f1e99e14af92561036
updated_at: 04/28/2017 07:04 AM
ms.date: 04/28/2017
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: site-recovery
---

# Set-AzureRmSiteRecoveryVaultSettings

## SYNOPSIS
Sets the Site Recovery vault context for further operations.

## SYNTAX

### AzureSiteRecoveryVault
```
Set-AzureRmSiteRecoveryVaultSettings -ASRVault <ASRVault> [<CommonParameters>]
```

### AzureRecoveryServicesVault
```
Set-AzureRmSiteRecoveryVaultSettings -ARSVault <ARSVault> [<CommonParameters>]
```

## DESCRIPTION
The **Set-AzureRmSiteRecoveryVaultSettings** cmdlet sets the Azure Site Recovery vault context for further operations.
This does not apply to recovery services vaults.

## EXAMPLES

## PARAMETERS

### -ASRVault
Specifies an **ASRVault** object.

```yaml
Type: ASRVault
Parameter Sets: AzureSiteRecoveryVault
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ARSVault
Specifies an **ARSVault** object.

```yaml
Type: ARSVault
Parameter Sets: AzureRecoveryServicesVault
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureRmSiteRecoveryVaultSettings](./Get-AzureRmSiteRecoveryVaultSettings.md)
