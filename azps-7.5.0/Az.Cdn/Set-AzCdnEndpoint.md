---
external help file: Microsoft.Azure.PowerShell.Cmdlets.Cdn.dll-Help.xml
Module Name: Az.Cdn
ms.assetid: 1A84AF77-1AEF-4FD0-9FAA-D195B361FCEB
online version: https://docs.microsoft.com/powershell/module/az.cdn/set-azcdnendpoint
schema: 2.0.0
content_git_url: https://github.com/Azure/azure-powershell/blob/main/src/Cdn/Cdn/help/Set-AzCdnEndpoint.md
original_content_git_url: https://github.com/Azure/azure-powershell/blob/main/src/Cdn/Cdn/help/Set-AzCdnEndpoint.md
---

# Set-AzCdnEndpoint

## SYNOPSIS
Updates a CDN endpoint.

> [!NOTE]
>This is the previous version of our documentation. Please consult [the most recent version](/powershell/module/az.cdn/set-azcdnendpoint) for up-to-date information.

## SYNTAX

```
Set-AzCdnEndpoint -CdnEndpoint <PSEndpoint> [-DefaultProfile <IAzureContextContainer>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

## DESCRIPTION
The **Set-AzCdnEndpoint** cmdlet updates an Azure Content Delivery Network (CDN) endpoint.

## EXAMPLES

### Example 1: Set allowed protocols to HTTPS only
```powershell
$endpointObject = Get-AzCdnEndpoint -ResourceGroupName myresourcegroup -ProfileName mycdnprofile -EndpointName myendpoint
$endpointObject.IsHttpAllowed = $false
Set-AzCdnEndpoint -CdnEndpoint $endpointObject
```

```Output
HostName                   : myendpoint.azureedge.net
OriginHostHeader           :
OriginPath                 :
ContentTypesToCompress     : {}
IsCompressionEnabled       : False
IsHttpAllowed              : False
IsHttpsAllowed             : True
QueryStringCachingBehavior : IgnoreQueryString
Origins                    : {mystorage}
OptimizationType           :
ProbePath                  :
GeoFilters                 : {}
DeliveryPolicy             :
ResourceState              : Running
DefaultOriginGroup         :
ResourceGroupName          : myresourcegroup
ProfileName                : mycdnprofile
Location                   : WestUs
Tags                       : {}
Id                         : /subscriptions/11111111-1111-1111-1111-111111111111/resourcegroups/myresourcegroup/providers/Micr
                             osoft.Cdn/profiles/mycdnprofile/endpoints/myendpoint
Name                       : myendpoint
Type                       : Microsoft.Cdn/profiles/endpoints
ProvisioningState          : Succeeded
```

Properties that are allowed to change are: `ContentTypesToCompress`, `IsCompressionEnabled`, `IsHttpAllowed`, `IsHttpsAllowed`, `QueryStringCachingBehavior`, `GeoFilters` and `Tags`.

## PARAMETERS

### -CdnEndpoint
Specifies the endpoint that this cmdlet updates.

```yaml
Type: Microsoft.Azure.Commands.Cdn.Models.Endpoint.PSEndpoint
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
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

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: False
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
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Azure.Commands.Cdn.Models.Endpoint.PSEndpoint

## OUTPUTS

### Microsoft.Azure.Commands.Cdn.Models.Endpoint.PSEndpoint

## NOTES

## RELATED LINKS

[Get-AzCdnEndpoint](./Get-AzCdnEndpoint.md)

[New-AzCdnEndpoint](./New-AzCdnEndpoint.md)

[Remove-AzCdnEndpoint](./Remove-AzCdnEndpoint.md)

[Start-AzCdnEndpoint](./Start-AzCdnEndpoint.md)

[Stop-AzCdnEndpoint](./Stop-AzCdnEndpoint.md)


