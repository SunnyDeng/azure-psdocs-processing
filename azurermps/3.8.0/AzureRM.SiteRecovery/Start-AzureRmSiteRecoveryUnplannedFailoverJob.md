---
external help file: Microsoft.Azure.Commands.SiteRecovery.dll-Help.xml
ms.assetid: 48494D81-A138-4D20-9286-D6A989AE70C9
online version:
schema: 2.0.0
updated_at: 04/07/2017 09:04 AM
ms.date: 04/07/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.SiteRecovery/v3.7.0/Start-AzureRmSiteRecoveryUnplannedFailoverJob.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.SiteRecovery/v3.7.0/Start-AzureRmSiteRecoveryUnplannedFailoverJob.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/195dcb690a30a5f2c0ecd5606483862547ef544a
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: site-recovery
---

# Start-AzureRmSiteRecoveryUnplannedFailoverJob

## SYNOPSIS
Starts the unplanned failover for a Site Recovery protection entity or recovery plan.

## SYNTAX

### ByPEObject (Default)
```
Start-AzureRmSiteRecoveryUnplannedFailoverJob -ProtectionEntity <ASRProtectionEntity> -Direction <String>
 [-PerformSourceSideActions] [-DataEncryptionPrimaryCertFile <String>]
 [-DataEncryptionSecondaryCertFile <String>] [<CommonParameters>]
```

### ByRPObject
```
Start-AzureRmSiteRecoveryUnplannedFailoverJob -RecoveryPlan <ASRRecoveryPlan> -Direction <String>
 [-PerformSourceSideActions] [-DataEncryptionPrimaryCertFile <String>]
 [-DataEncryptionSecondaryCertFile <String>] [<CommonParameters>]
```

### ByRPIObject
```
Start-AzureRmSiteRecoveryUnplannedFailoverJob -ReplicationProtectedItem <ASRReplicationProtectedItem>
 -Direction <String> [-PerformSourceSideActions] [-DataEncryptionPrimaryCertFile <String>]
 [-DataEncryptionSecondaryCertFile <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Start-AzureRmSiteRecoveryUnplannedFailoverJob** cmdlet starts the unplanned failover of an Azure Site Recovery protection entity or recovery plan.
You can check whether the job succeeds by using the Get-AzureRmSiteRecoveryJob cmdlet.

## EXAMPLES

### 1:
```

```

## PARAMETERS

### -ProtectionEntity
Specifies the Site Recovery protection entity object.

```yaml
Type: ASRProtectionEntity
Parameter Sets: ByPEObject
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Direction
Specifies the direction of the failover.
The acceptable values for this parameter are:

- PrimaryToRecovery
- RecoveryToPrimary

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PerformSourceSideActions
Indicates that the action can perform source site operations.

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

### -DataEncryptionPrimaryCertFile
Specifies the primary certificate file.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DataEncryptionSecondaryCertFile
Specifies the secondary certificate file.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RecoveryPlan
Specifies a recovery plan object.

```yaml
Type: ASRRecoveryPlan
Parameter Sets: ByRPObject
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ReplicationProtectedItem
```yaml
Type: ASRReplicationProtectedItem
Parameter Sets: ByRPIObject
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

[Get-AzureRmSiteRecoveryJob](./Get-AzureRmSiteRecoveryJob.md)

