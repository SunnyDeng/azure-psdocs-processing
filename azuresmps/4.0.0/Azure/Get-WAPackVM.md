---
external help file: Microsoft.WindowsAzure.Commands.dll-Help.xml
ms.assetid: 047C5FBD-CB0D-47BF-AE03-4DF32B4FAD87
online version:
schema: 2.0.0
updated_at: 05/12/2017 22:05 PM
ms.date: 05/12/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure/v4.0.0/Get-WAPackVM.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure/v4.0.0/Get-WAPackVM.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/3b96c1e0b28fc56dfbf6de55728d5478e0d02def
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: azure-asm
---

# Get-WAPackVM

## SYNOPSIS
Gets virtual machine objects.

## SYNTAX

### Empty (Default)
```
Get-WAPackVM [-Profile <AzureSMProfile>] [<CommonParameters>]
```

### FromName
```
Get-WAPackVM [-Name <String>] [-Profile <AzureSMProfile>] [<CommonParameters>]
```

### FromId
```
Get-WAPackVM [-ID <Guid>] [-Profile <AzureSMProfile>] [<CommonParameters>]
```

## DESCRIPTION
These topics are deprecated and will be removed in the future.
For the updated topics, see [Azure WAPack Cmdlets](http://msdn.microsoft.com/library/dn776450.aspx) (http://msdn.microsoft.com/library/dn776450.aspx).
This topic describes the cmdlet in the 0.8.1 version of the Microsoft Azure PowerShell module.
To find out the version of the module you're using, from the Azure PowerShell console, type `(Get-Module -Name Azure).Version`.

The **Get-WAPackVM** cmdlet gets virtual machine objects.

## EXAMPLES

### Example 1: Get a virtual machine by using a name
```
PS C:\> Get-WAPackVM -Name "ContosoV126"
```

This command gets the virtual machine named ContosoV126.

### Example 2: Get a virtual machine by using an ID
```
PS C:\> Get-WAPackVM -Id 66242D17-189F-480D-87CF-8E1D749998C8
```

This command gets the virtual machine that has the specified ID.

### Example 3: Get all virtual machines
```
PS C:\> Get-WAPackVM
```

This command gets all virtual machines.

## PARAMETERS

### -ID
Specifies the unique ID of a virtual machine.

```yaml
Type: Guid
Parameter Sets: FromId
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Name
Specifies the name of a virtual machine.

```yaml
Type: String
Parameter Sets: FromName
Aliases: 

Required: False
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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[New-WAPackVM](./New-WAPackVM.md)

[Remove-WAPackVM](./Remove-WAPackVM.md)

[Restart-WAPackVM](./Restart-WAPackVM.md)

[Resume-WAPackVM](./Resume-WAPackVM.md)

[Set-WAPackVM](./Set-WAPackVM.md)

[Start-WAPackVM](./Start-WAPackVM.md)

[Stop-WAPackVM](./Stop-WAPackVM.md)

[Suspend-WAPackVM](./Suspend-WAPackVM.md)

[Get-WAPackVMOSDisk](./Get-WAPackVMOSDisk.md)

