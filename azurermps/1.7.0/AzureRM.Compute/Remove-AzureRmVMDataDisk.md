---
external help file: Microsoft.Azure.Commands.Compute.dll-Help.xml
ms.assetid: 4538ECE1-A0B6-4439-B931-73E11B83D72A
online version:
schema: 2.0.0
updated_at: 05/01/2017 21:05 PM
ms.date: 05/01/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Compute/v1.3.4/Remove-AzureRmVMDataDisk.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Compute/v1.3.4/Remove-AzureRmVMDataDisk.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/0589fbf53d27e39e0cf445261d29c64fb0859d62
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: big-compute
---

# Remove-AzureRmVMDataDisk

## SYNOPSIS
Removes a data disk from a virtual machine.

## SYNTAX

```
Remove-AzureRmVMDataDisk [-VM] <PSVirtualMachine> [-DataDiskNames] <String[]>
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureRmVMDataDisk** cmdlet removes a data disk from a virtual machine.

## EXAMPLES

### Example 1: Remove a data disk from a virtual machine
```
PS C:\>$VirtualMachine = Get-AzureRmVM -ResourceGroupName "ResourceGroup11" -Name "VirtualMachine07" 
PS C:\> Remove-AzureRmVMDataDisk -VM $VirtualMachine -Name "Disk3"
PS C:\> Update-AzureRmVM -ResourceGroupName "ResourceGroup11" -Name "VirtualMachine07" -VM $VirtualMachine
```

The first command gets the virtual machine named VirtualMachine07 by using the **Get-AzureRmVM** cmdlet.
The command stores the virtual machine in the $VirtualMachine variable.

The second command removes the data disk named Disk3 from the virtual machine stored in $VirtualMachine.

The final command updates the state of the virtual machine stored in $VirtualMachine in ResourceGroup11.

## PARAMETERS

### -DataDiskNames
Specifies the names of one or more data disks that this cmdlet removes.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: Name

Required: True
Position: 1
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

### -VM
Specifies the local virtual machine object from which to remove a data disk.
To obtain a virtual machine object, use the Get-AzureRmVM cmdlet.

```yaml
Type: PSVirtualMachine
Parameter Sets: (All)
Aliases: VMProfile

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Add-AzureRmVMDataDisk](./Add-AzureRmVMDataDisk.md)

[Get-AzureRmVM](./Get-AzureRmVM.md)


