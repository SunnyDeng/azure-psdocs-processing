---
external help file: Microsoft.Azure.Commands.OperationalInsights.dll-Help.xml
ms.assetid: 26B1921E-6052-471B-B5B6-F2853536A425
online version:
schema: 2.0.0
updated_at: 03/11/2017 23:03 PM
ms.date: 03/11/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.OperationalInsights/v2.6.0/Enable-AzureRmOperationalInsightsIISLogCollection.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.OperationalInsights/v2.6.0/Enable-AzureRmOperationalInsightsIISLogCollection.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/bc71000aa3c7f754b95442dcc415a7324626a15c
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
---

# Enable-AzureRmOperationalInsightsIISLogCollection

## SYNOPSIS
Starts collection of IIS logs from computers in a workspace.

## SYNTAX

### ByWorkspaceName (Default)
```
Enable-AzureRmOperationalInsightsIISLogCollection [-ResourceGroupName] <String> [-WorkspaceName] <String>
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### ByWorkspaceObject
```
Enable-AzureRmOperationalInsightsIISLogCollection [-Workspace] <PSWorkspace>
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

## DESCRIPTION
The **Enable-AzureRmOperationalInsightsIISLogCollection** cmdlet starts collection of Internet Information Services (IIS) logs from connected computers in a workspace.

## EXAMPLES

### 1:
```

```

## PARAMETERS

### -ResourceGroupName
Specifies the name of a resource group that contains computers.

```yaml
Type: String
Parameter Sets: ByWorkspaceName
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -WorkspaceName
Specifies the name of a workspace in which this cmdlet operates.

```yaml
Type: String
Parameter Sets: ByWorkspaceName
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -InformationAction
Specifies how this cmdlet responds to an information event.

The acceptable values for this parameter are:

- Continue
- Ignore
- Inquire
- SilentlyContinue
- Stop
- Suspend

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
Specifies an information variable.

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

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -Workspace
Specifies a workspace in which this cmdlet operates.

```yaml
Type: PSWorkspace
Parameter Sets: ByWorkspaceObject
Aliases: 

Required: True
Position: 0
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

[Disable-AzureRmOperationalInsightsIISLogCollection](./Disable-AzureRmOperationalInsightsIISLogCollection.md)

