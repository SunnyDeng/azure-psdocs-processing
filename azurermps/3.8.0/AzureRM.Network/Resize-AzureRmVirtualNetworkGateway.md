---
external help file: Microsoft.Azure.Commands.Network.dll-Help.xml
ms.assetid: DE2441FC-9504-4F3F-AEAF-37EDCD9B7275
online version:
schema: 2.0.0
content_git_url: https://github.com/Azure/azure-powershell/blob/preview/src/ResourceManager/Network/Commands.Network/help/Resize-AzureRmVirtualNetworkGateway.md
original_content_git_url: https://github.com/Azure/azure-powershell/blob/preview/src/ResourceManager/Network/Commands.Network/help/Resize-AzureRmVirtualNetworkGateway.md
gitcommit: https://github.com/Azure/azure-powershell/blob/898dcc79a9e3bf9563d390c9a7c04f5ea5b5a269
updated_at: 04/28/2017 07:04 AM
ms.date: 04/28/2017
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: virtual-network
---

# Resize-AzureRmVirtualNetworkGateway

## SYNOPSIS
Resizes an existing virtual network gateway.

## SYNTAX

```
Resize-AzureRmVirtualNetworkGateway -VirtualNetworkGateway <PSVirtualNetworkGateway> -GatewaySku <String>
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Resize-AzureRmVirtualNetworkGateway** cmdlet enables you to change the stock-keeping unit (SKU) for a virtual network gateway.
SKUs determine the capabilities of a gateway, including such things as throughput and the maximum number of IP tunnels that are allowed.
Azure supports Basic, Standard, and High-Performance SKUs (sometimes referred to as Small, Medium, and Large SKUs).
For detailed information about the capabilities of each SKU type, see https://azure.microsoft.com/en-us/documentation/articles/vpn-gateway-about-vpngateways/.https://azure.microsoft.com/en-us/documentation/articles/vpn-gateway-about-vpngateways/.

Keep in mind that SKUs differ in pricing as well as capabilities.
For more information, see https://azure.microsoft.com/en-us/pricing/details/vpn-gateway/https://azure.microsoft.com/en-us/pricing/details/vpn-gateway/.

## EXAMPLES

### Example 1: Change the size of a virtual network gateway
```
PS C:\>$Gateway = Get-AzureRmVirtualNetworkGateway -Name "ContosoVirtualGateway"
PS C:\> Resize-AzureRmVirtualNetworkGateway -VirtualNetworkGateway $Gateway -GatewaySku "Basic"
```

This example changes the size of a virtual network gateway named ContosoVirtualGateway.

The first command creates an object reference to ContosoVirtualGateway; this object reference is stored in a variable named $Gateway.

The second command then uses the **Resize-AzureRmVirtualNetworkGateway** cmdlet to set the *GatewaySku* property to Basic.

## PARAMETERS

### -GatewaySku
Specifies the new type of gateway SKU.
The acceptable values for this parameter are:

- Basic
- Standard
- High Performance

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

### -VirtualNetworkGateway
Specifies an object reference to the virtual network gateway to be resized.
You can create this object reference by using the Get-AzureRmVirtualNetworkGateway and specifying the name of the gateway.

```yaml
Type: PSVirtualNetworkGateway
Parameter Sets: (All)
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

###  
This cmdlet accepts pipelined instances of the **Microsoft.Azure.Commands.Network.Models.PSVirtualNetworkGateway** object.

## OUTPUTS

###  
This cmdlet modifies existing instances of the **Microsoft.Azure.Commands.Network.Models.PSVirtualNetworkGateway** object.

## NOTES

## RELATED LINKS

[Get-AzureRmVpnClientPackage](./Get-AzureRmVpnClientPackage.md)

[Get-AzureRmVirtualNetworkGateway](./Get-AzureRmVirtualNetworkGateway.md)

[Set-AzureRmVirtualNetworkGatewayVpnClientConfig](./Set-AzureRmVirtualNetworkGatewayVpnClientConfig.md)


