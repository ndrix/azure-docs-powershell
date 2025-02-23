---
external help file: Microsoft.Azure.PowerShell.Cmdlets.NotificationHubs.dll-Help.xml
Module Name: Az.NotificationHubs
ms.assetid: 1EC19069-B64C-4F0F-99A3-07C16E46C0A0
online version: https://docs.microsoft.com/powershell/module/az.notificationhubs/new-aznotificationhubsnamespacekey
schema: 2.0.0
content_git_url: https://github.com/Azure/azure-powershell/blob/main/src/NotificationHubs/NotificationHubs/help/New-AzNotificationHubsNamespaceKey.md
original_content_git_url: https://github.com/Azure/azure-powershell/blob/main/src/NotificationHubs/NotificationHubs/help/New-AzNotificationHubsNamespaceKey.md
---

# New-AzNotificationHubsNamespaceKey

## SYNOPSIS
Regenerate the Authorization Rule Key for a Namespace.

> [!NOTE]
>This is the previous version of our documentation. Please consult [the most recent version](/powershell/module/az.notificationhubs/new-aznotificationhubsnamespacekey) for up-to-date information.

## SYNTAX

```
New-AzNotificationHubsNamespaceKey [-ResourceGroup] <String> [-Namespace] <String>
 [[-AuthorizationRule] <String>] [-PolicyKey] <String> [-Force] [-DefaultProfile <IAzureContextContainer>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
New-AzNotificationHubsNamespaceKey cmdlet regenerates the Primary Key/Secondary Key for the Namespace Authorization Rule.

## EXAMPLES

### Example 1
```powershell
New-AzNotificationHubsNamespaceKey -ResourceGroup "ContosoNotificationsGroup" -Namespace "ContosoNamespace" -AuthorizationRule "RootManageSharedAccessKey" -PolicyKey "PrimaryKey"
```

```Output
PrimaryConnectionString   : Endpoint=sb://contosonamespace.servicebus.windows.net/;SharedAccessKeyName=RootManageSharedAc
                            cessKey;SharedAccessKey=VUhKcGJXRnllVU52Ym01bFkzUnBiMjVUZEhKcGJtYz0=
SecondaryConnectionString : Endpoint=sb://contosonamespace.servicebus.windows.net/;SharedAccessKeyName=RootManageSharedAc
                            cessKey;SharedAccessKey=VTJWamIyNWtZWEo1UTI5dWJtVmpkR2x2YmxOMGNtbHV=
PrimaryKey                : VUhKcGJXRnllVU52Ym01bFkzUnBiMjVUZEhKcGJtYz0=
SecondaryKey              : VTJWamIyNWtZWEo1UTI5dWJtVmpkR2x2YmxOMGNtbHV=
KeyName                   : RootManageSharedAccessKey
```

## PARAMETERS

### -AuthorizationRule
```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -DefaultProfile
The credentials, account, tenant, and subscription used for communication with azure

```yaml
Type: Microsoft.Azure.Commands.Common.Authentication.Abstractions.Core.IAzureContextContainer
Parameter Sets: (All)
Aliases: AzContext, AzureRmContext, AzureCredential

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Force
Do not ask for confirmation.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Namespace
```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -PolicyKey
```yaml
Type: System.String
Parameter Sets: (All)
Aliases:
Accepted values: PrimaryKey, SecondaryKey

Required: True
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResourceGroup
```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: cf

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
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.String

## OUTPUTS

### Microsoft.Azure.Management.NotificationHubs.Models.ResourceListKeys

## NOTES

## RELATED LINKS
