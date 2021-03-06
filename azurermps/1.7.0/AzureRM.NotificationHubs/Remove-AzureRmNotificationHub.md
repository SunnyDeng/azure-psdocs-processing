---
external help file: Microsoft.Azure.Commands.NotificationHubs.dll-Help.xml
ms.assetid: FEBB2EBF-3525-4D89-BB76-A38FAF40FCB7
online version:
schema: 2.0.0
updated_at: 05/01/2017 21:05 PM
ms.date: 05/01/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.NotificationHubs/v1.0.12/Remove-AzureRmNotificationHub.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.NotificationHubs/v1.0.12/Remove-AzureRmNotificationHub.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/0589fbf53d27e39e0cf445261d29c64fb0859d62
ms.topic: reference
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: true
ms.service: notification-hubs
---

# Remove-AzureRmNotificationHub

## SYNOPSIS
Removes an existing notification hub.

## SYNTAX

```
Remove-AzureRmNotificationHub [-ResourceGroup] <String> [-Namespace] <String> [-NotificationHub] <String>
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureRmNotificationHub** cmdlet removes an existing notification hub.
Notification hubs are used to send push notifications to multiple clients regardless of the platform used by those clients.
Platforms include, but are not limited to: iOS, Android, Windows Phone 8, and Windows Store.
Notification hubs are roughly equivalent to individual apps: each of your apps will typically have its own notification hub.

You can remove an existing notification hub by using the **Remove-AzureRmNotificationHub** cmdlet.
After a hub has been removed you can no longer use that hub to send push notifications to users.

## EXAMPLES

### Example 1: Remove a notification hub
```
PS C:\>Remove-AzureRmNotificationHub -Namespace "ContosoNamespace" -ResourceGroup "ContosoNotificationsGroup" -NotificationHub "ContosoInternalHub"
```

This command removes the notification hub named ContosoInternalHub.
In order to remove the hub, you must specify the namespace where the hub is located as well as the resource group the hub is assigned to.

## PARAMETERS

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

### -Namespace
Specifies the namespace to which the notification hub is assigned.

Namespaces provide a way to group and categorize notification hubs.

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

### -NotificationHub
Specifies the notification hub to be removed.

Notification hubs are used to send push notifications to multiple clients regardless of the platform used by those clients.

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

### -ResourceGroup
Specifies the resource group to which the notification hub is assigned.

Resource groups organize items such as namespaces, notification hubs, and authorization rules in ways that help simply inventory management and Azure administration.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
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

[Get-AzureRmNotificationHub](./Get-AzureRmNotificationHub.md)

[New-AzureRmNotificationHub](./New-AzureRmNotificationHub.md)

[Set-AzureRmNotificationHub](./Set-AzureRmNotificationHub.md)


