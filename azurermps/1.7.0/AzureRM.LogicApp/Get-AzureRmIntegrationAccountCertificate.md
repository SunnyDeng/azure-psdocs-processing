---
external help file: Microsoft.Azure.Commands.LogicApp.dll-Help.xml
online version:
schema: 2.0.0
updated_at: 05/02/2017 17:05 PM
ms.date: 05/02/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.LogicApp/v1.0.8/Get-AzureRmIntegrationAccountCertificate.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.LogicApp/v1.0.8/Get-AzureRmIntegrationAccountCertificate.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/fdff926f5dd35f9020f210f87b450464ba162edc
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: app-service-logic
---

# Get-AzureRmIntegrationAccountCertificate

## SYNOPSIS
Gets the specified integration account certificate from the Azure resource group.

## SYNTAX

```
Get-AzureRmIntegrationAccountCertificate [-ResourceGroupName <String>] [-Name <String>]
 [-CertificateName <String>] [-InformationAction <ActionPreference>] [-InformationVariable <String>]
 [<CommonParameters>]
```

## DESCRIPTION
This is the Description section

The Get-AzureRmIntegrationAccountCertificate cmdlet retrieves integration account certificate from the Azure resource group and returns an object that represents the integration account certificate.
Use this cmdlet to get the integration account certificate from specified resource group.
You can get the integration account certificate by specifying the integration account name, resource group name and certificate name.
To use the dynamic parameters, just type them in the command, or type a hyphen sign (-) to indicate a parameter name and then press the TAB key repeatedly to cycle through the available parameters.
If you miss a required template parameter, the cmdlet prompts you for the value.

## EXAMPLES

### --------------------------  Example 1 : Get the integration account certificate by name.  --------------------------
@{paragraph=PS C:\\\>}



```
Get-AzureRmIntegrationAccountCertificate -ResourceGroupName "ResourceGroup1" -Name "IntegrationAccount1" -CertificateName "IntegrationAccountCertificate1"
```

This command gets the integration account certificate by name.

Id                : /subscriptions/\<SusbcriptionId\>/resourceGroups/\<ResourceGroup1\>/providers/Microsoft.Logic/integrationAccounts/IntegartionAccount1/certificates/IntegrationAccountCertificate1
Name              : IntegrationAccountCertificate1
Type              : Microsoft.Logic/integrationAccounts/certificates
CreatedTime       : 3/26/2016 6:59:07 PM
ChangedTime       : 3/26/2016 6:59:07 PM
KeyName           : TestKey
KeyVersion        : 1.0
KeyVaultId        : /subscriptions/\<SusbcriptionId/resourcegroups/ResourceGroup1/providers/microsoft.keyvault/vaults/\<name\>
KeyVaultName      : testkeyvault
KeyVaultName      : testkeyvault
PublicCertificate :
MetaData          :

### --------------------------  Example 2 : Get the integration account certificates by integration account name.  --------------------------
@{paragraph=PS C:\\\>}



```
Get-AzureRmIntegrationAccountCertificate -ResourceGroupName "ResourceGroup1" -Name "IntegrationAccount1"
```

This command gets the integration account certificates by integration account name.

Id                : /subscriptions/\<SusbcriptionId\>/resourceGroups/\<ResourceGroup1\>/providers/Microsoft.Logic/integrationAccounts/IntegartionAccount1/certificates/IntegrationAccountCertificate1
Name              : IntegrationAccountCertificate1
Type              : Microsoft.Logic/integrationAccounts/certificates
CreatedTime       : 3/26/2016 6:59:07 PM
ChangedTime       : 3/26/2016 6:59:07 PM
KeyName           : TestKey
KeyVersion        : 1.0
KeyVaultId        : /subscriptions/\<SusbcriptionId/resourcegroups/ResourceGroup1/providers/microsoft.keyvault/vaults/\<name\>
KeyVaultName      : testkeyvault
KeyVaultName      : testkeyvault
PublicCertificate :
MetaData          :

## PARAMETERS

### -CertificateName
Specifies a name for the integration account certificate.
This parameter is optional.

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

### -InformationAction
@{Text=}

```yaml
Type: ActionPreference
Parameter Sets: (All)
Aliases: infa

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationVariable
@{Text=}

```yaml
Type: String
Parameter Sets: (All)
Aliases: iv

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
Specifies a name for the integration account.
This parameter is optional.

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

### -ResourceGroupName
Specifies a name for the resource group.
This parameter is required.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### Microsoft.Azure.Management.Logic.Models.IntegrationAccountCertificate

## NOTES

## RELATED LINKS

[Set-AzureRmIntegrationAccountCertificate]()

[Remove-AzureRmIntegrationAccountCertificate]()

[New-AzureRmIntegrationAccountCertificate]()

