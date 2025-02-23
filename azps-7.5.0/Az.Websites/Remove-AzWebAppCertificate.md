---
external help file: Microsoft.Azure.PowerShell.Cmdlets.Websites.dll-Help.xml
Module Name: Az.Websites
online version: https://docs.microsoft.com/powershell/module/az.websites/remove-AzWebAppCertificate
schema: 2.0.0
content_git_url: https://github.com/Azure/azure-powershell/blob/main/src/Websites/Websites/help/Remove-AzWebAppCertificate.md
original_content_git_url: https://github.com/Azure/azure-powershell/blob/main/src/Websites/Websites/help/Remove-AzWebAppCertificate.md
---

# Remove-AzWebAppCertificate

## SYNOPSIS
Removes an App service managed certificate for an Azure Web App. 

> [!NOTE]
>This is the previous version of our documentation. Please consult [the most recent version](/powershell/module/az.websites/remove-azwebappcertificate) for up-to-date information.

## SYNTAX

```
Remove-AzWebAppCertificate [-ResourceGroupName] <String> [-ThumbPrint] <String>
 [-DefaultProfile <IAzureContextContainer>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzWebAppCertificate** cmdlet Removes an Azure App Service Managed Certificate

## EXAMPLES

### Example 1
```powershell
Remove-AzWebAppCertificate -ResourceGroupName Default-Web-WestUS -Thumbprint "E3A38EBA60CAA1C162785A2E1C44A15AD450199C3"
```

This command removes App Service Managed certificate for the given web app.

## PARAMETERS

### -DefaultProfile
The credentials, account, tenant, and subscription used for communication with Azure.

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

### -ResourceGroupName
The name of the resource group.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ThumbPrint
Thumbprint of the certificate that already exists in web space.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: 3
Default value: None
Accept pipeline input: False
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
Shows what would happen if the cmdlet runs. The cmdlet is not run.

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
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None

## OUTPUTS

### System.Void

## NOTES

## RELATED LINKS

[New-AzWebAppCertificate](./New-AzWebAppCertificate.md)
