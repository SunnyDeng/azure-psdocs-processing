---
external help file: Microsoft.Azure.Commands.ResourceManager.Automation.dll-Help.xml
online version:
schema: 2.0.0
ms.assetid: 9E03B502-062A-4B67-B17C-810E3E2CEEBA
updated_at: 11/11/2016 23:11 PM
ms.date: 11/11/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Automation/v2.1.0/Get-AzureRmAutomationRegistrationInfo.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Automation/v2.1.0/Get-AzureRmAutomationRegistrationInfo.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/79eeb985ea480979357fb4695832a0c3d29a48bf
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: automation
---

# Get-AzureRmAutomationRegistrationInfo

## SYNOPSIS
Gets registration information for onboarding a DSC node or hybrid worker to Automation.

## SYNTAX

```
Get-AzureRmAutomationRegistrationInfo [-ResourceGroupName] <String> [-AutomationAccountName] <String>
 [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmAutomationRegistrationInfo** cmdlet gets the endpoint and keys required to onboard a Desired State Configuration (DSC) node or hybrid worker into an Azure Automation account.

## EXAMPLES

### Example 1: Get registration information
```
PS C:\>Get-AzureRmAutomationRegistrationInfo -ResourceGroup "ResourceGroup01" -AutomationAccountName "AutomationAccount01"
```

This command gets the registration information for the Automation account named AutomationAccount01 in the Resource Group named ResourceGroup01.

## PARAMETERS

### -AutomationAccountName
Specifies the name of Automation account for which this cmdlet gets registration information.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of a resource group.
This cmdlet gets registration information for the resource group that this parameter specifies.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureRmAutomationAccount](./Get-AzureRmAutomationAccount.md)

[Get-AzureRmAutomationDscNode](./Get-AzureRmAutomationDscNode.md)

[New-AzureRmAutomationKey](./New-AzureRmAutomationKey.md)


