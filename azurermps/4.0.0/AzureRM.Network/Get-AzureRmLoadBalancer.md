---
external help file: Microsoft.Azure.Commands.Network.dll-Help.xml
ms.assetid: 78F356F6-A621-4C27-B9CC-D103E74B3A33
online version:
schema: 2.0.0
content_git_url: https://github.com/Azure/azure-powershell/blob/preview/src/ResourceManager/Network/Commands.Network/help/Get-AzureRmLoadBalancer.md
original_content_git_url: https://github.com/Azure/azure-powershell/blob/preview/src/ResourceManager/Network/Commands.Network/help/Get-AzureRmLoadBalancer.md
gitcommit: https://github.com/Azure/azure-powershell/blob/8810c0614b76be8d014616888a4ae7733a452af9
updated_at: 05/12/2017 03:05 AM
ms.date: 05/12/2017
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: virtual-network
---

# Get-AzureRmLoadBalancer

## SYNOPSIS
Gets a load balancer.

## SYNTAX

### NoExpand
```
Get-AzureRmLoadBalancer [-Name <String>] [-ResourceGroupName <String>] [<CommonParameters>]
```

### Expand
```
Get-AzureRmLoadBalancer -Name <String> -ResourceGroupName <String> -ExpandResource <String>
 [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmLoadBalancer** cmdlet gets one or more Azure load balancers that are contained in a resource group.

## EXAMPLES

### Example 1: Get a load balancer
```
PS C:\>Get-AzureRmLoadBalancer -Name "MyLoadBalancer" -ResourceGroupName "MyResourceGroup"
```

This command gets the load balancer named MyLoadBalancer.
A load balancer must exist before you can run this cmdlet.

## PARAMETERS

### -ExpandResource
```yaml
Type: String
Parameter Sets: Expand
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Name
```yaml
Type: String
Parameter Sets: NoExpand
Aliases: ResourceName

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

```yaml
Type: String
Parameter Sets: Expand
Aliases: ResourceName

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
```yaml
Type: String
Parameter Sets: NoExpand
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

```yaml
Type: String
Parameter Sets: Expand
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

## NOTES

## RELATED LINKS

[New-AzureRmLoadBalancer](./New-AzureRmLoadBalancer.md)

[Remove-AzureRmLoadBalancer](./Remove-AzureRmLoadBalancer.md)

[Set-AzureRmLoadBalancer](./Set-AzureRmLoadBalancer.md)


