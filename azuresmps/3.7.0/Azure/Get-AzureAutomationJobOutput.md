---
external help file: Microsoft.Azure.Commands.Automation.dll-Help.xml
ms.assetid: 1C18EE5D-A916-4776-ABAE-A7B24FA74108
online version:
schema: 2.0.0
updated_at: 03/29/2017 02:03 AM
ms.date: 03/29/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure/v3.7.0/Get-AzureAutomationJobOutput.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure/v3.7.0/Get-AzureAutomationJobOutput.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/828e5b8648af6bdf3119ffe0cd409647f00de183
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: azure-asm
---

# Get-AzureAutomationJobOutput

## SYNOPSIS
Gets the output of an Azure Automation job.

## SYNTAX

```
Get-AzureAutomationJobOutput -Id <Guid> [-Stream <StreamType>] [-StartTime <DateTimeOffset>]
 -AutomationAccountName <String> [-Profile <AzureSMProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureAutomationJobOutput** cmdlet gets the output of a Microsoft Azure Automation job.

## EXAMPLES

### Example 1: Get the output of an Azure Automation job
```
PS C:\> Get-AzureAutomationJobOutput -AutomationAccountName "Contoso17" -Id 2989b069-24fe-40b9-b3bd-cb7e5eac4b64 -Stream "Any"
```

This command gets all of the output of the job that has the specified ID.

## PARAMETERS

### -AutomationAccountName
Specifies the name of an Azure Automation account.

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

### -Id
Specifies the ID of a job.

```yaml
Type: Guid
Parameter Sets: (All)
Aliases: JobId

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Profile
Specifies the Azure profile from which this cmdlet reads.
If you do not specify a profile, this cmdlet reads from the local default profile.

```yaml
Type: AzureSMProfile
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -StartTime
Specifies a start time.

```yaml
Type: DateTimeOffset
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Stream
Specifies the type of output.
Valid values are: 

- Any
- Debug
- Error
- Output
- Progress
- Verbose
- Warning

```yaml
Type: StreamType
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

## NOTES

## RELATED LINKS

[Get-AzureAutomationJob](./Get-AzureAutomationJob.md)

[Resume-AzureAutomationJob](./Resume-AzureAutomationJob.md)

[Stop-AzureAutomationJob](./Stop-AzureAutomationJob.md)

[Suspend-AzureAutomationJob](./Suspend-AzureAutomationJob.md)


