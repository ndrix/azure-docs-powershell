---
external help file: 
Module Name: Az.Cdn
online version: https://docs.microsoft.com/powershell/module/az.Cdn/new-AzCdnHealthProbeParametersObject
schema: 2.0.0
content_git_url: https://github.com/Azure/azure-powershell/blob/main/src/Cdn/help/New-AzCdnHealthProbeParametersObject.md
original_content_git_url: https://github.com/Azure/azure-powershell/blob/main/src/Cdn/help/New-AzCdnHealthProbeParametersObject.md
---

# New-AzCdnHealthProbeParametersObject

## SYNOPSIS
Create an in-memory object for HealthProbeParameters.

> [!NOTE]
>This is the previous version of our documentation. Please consult [the most recent version](/powershell/module/az.cdn/new-azcdnhealthprobeparametersobject) for up-to-date information.

## SYNTAX

```
New-AzCdnHealthProbeParametersObject [-ProbeIntervalInSecond <Int32>] [-ProbePath <String>]
 [-ProbeProtocol <ProbeProtocol>] [-ProbeRequestType <HealthProbeRequestType>] [<CommonParameters>]
```

## DESCRIPTION
Create an in-memory object for HealthProbeParameters.

## EXAMPLES

### Example 1: Create an in-memory object for AzureCDN HealthProbeParameters
```powershell
New-AzCdnHealthProbeParametersObject -ProbeIntervalInSecond 120 -ProbePath "/check-health.aspx" -ProbeProtocol "Http" -ProbeRequestType "HEAD"
```

```output
ProbeIntervalInSecond ProbePath          ProbeProtocol ProbeRequestType
--------------------- ---------          ------------- ----------------
120                   /check-health.aspx Http          HEAD
```

Create an in-memory object for AzureCDN HealthProbeParameters

## PARAMETERS

### -ProbeIntervalInSecond
The number of seconds between health probes.Default is 240sec.

```yaml
Type: System.Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ProbePath
The path relative to the origin that is used to determine the health of the origin.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ProbeProtocol
Protocol to use for health probe.

```yaml
Type: Microsoft.Azure.PowerShell.Cmdlets.Cdn.Support.ProbeProtocol
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ProbeRequestType
The type of health probe request that is made.

```yaml
Type: Microsoft.Azure.PowerShell.Cmdlets.Cdn.Support.HealthProbeRequestType
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### Microsoft.Azure.PowerShell.Cmdlets.Cdn.Models.Api20210601.HealthProbeParameters

## NOTES

ALIASES

## RELATED LINKS

