---
external help file: 
Module Name: Az.Cdn
online version: https://docs.microsoft.com/powershell/module/az.Cdn/new-AzCdnResponseBasedOriginErrorDetectionParametersObject
schema: 2.0.0
content_git_url: https://github.com/Azure/azure-powershell/blob/main/src/Cdn/help/New-AzCdnResponseBasedOriginErrorDetectionParametersObject.md
original_content_git_url: https://github.com/Azure/azure-powershell/blob/main/src/Cdn/help/New-AzCdnResponseBasedOriginErrorDetectionParametersObject.md
---

# New-AzCdnResponseBasedOriginErrorDetectionParametersObject

## SYNOPSIS
Create an in-memory object for ResponseBasedOriginErrorDetectionParameters.

> [!NOTE]
>This is the previous version of our documentation. Please consult [the most recent version](/powershell/module/az.cdn/new-azcdnresponsebasedoriginerrordetectionparametersobject) for up-to-date information.

## SYNTAX

```
New-AzCdnResponseBasedOriginErrorDetectionParametersObject [-HttpErrorRange <IHttpErrorRangeParameters[]>]
 [-ResponseBasedDetectedErrorType <ResponseBasedDetectedErrorTypes>]
 [-ResponseBasedFailoverThresholdPercentage <Int32>] [<CommonParameters>]
```

## DESCRIPTION
Create an in-memory object for ResponseBasedOriginErrorDetectionParameters.

## EXAMPLES

### Example 1: {{ Add title here }}
```powershell
{{ Add code here }}
```

```output
{{ Add output here }}
```

{{ Add description here }}

### Example 2: {{ Add title here }}
```powershell
{{ Add code here }}
```

```output
{{ Add output here }}
```

{{ Add description here }}

## PARAMETERS

### -HttpErrorRange
The list of Http status code ranges that are considered as server errors for origin and it is marked as unhealthy.
To construct, see NOTES section for HTTPERRORRANGE properties and create a hash table.

```yaml
Type: Microsoft.Azure.PowerShell.Cmdlets.Cdn.Models.Api20210601.IHttpErrorRangeParameters[]
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResponseBasedDetectedErrorType
Type of response errors for real user requests for which origin will be deemed unhealthy.

```yaml
Type: Microsoft.Azure.PowerShell.Cmdlets.Cdn.Support.ResponseBasedDetectedErrorTypes
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResponseBasedFailoverThresholdPercentage
The percentage of failed requests in the sample where failover should trigger.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### Microsoft.Azure.PowerShell.Cmdlets.Cdn.Models.Api20210601.ResponseBasedOriginErrorDetectionParameters

## NOTES

ALIASES

COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.


HTTPERRORRANGE <IHttpErrorRangeParameters[]>: The list of Http status code ranges that are considered as server errors for origin and it is marked as unhealthy.
  - `[Begin <Int32?>]`: The inclusive start of the http status code range.
  - `[End <Int32?>]`: The inclusive end of the http status code range.

## RELATED LINKS

