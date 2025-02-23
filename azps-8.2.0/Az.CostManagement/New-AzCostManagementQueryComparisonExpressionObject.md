---
external help file: 
Module Name: Az.CostManagement
online version: https://docs.microsoft.com/powershell/module/az.CostManagement/new-AzCostManagementQueryComparisonExpressionObject
schema: 2.0.0
content_git_url: https://github.com/Azure/azure-powershell/blob/main/src/CostManagement/help/New-AzCostManagementQueryComparisonExpressionObject.md
original_content_git_url: https://github.com/Azure/azure-powershell/blob/main/src/CostManagement/help/New-AzCostManagementQueryComparisonExpressionObject.md
---

# New-AzCostManagementQueryComparisonExpressionObject

## SYNOPSIS
Create a in-memory object for QueryComparisonExpression

> [!NOTE]
>This is the previous version of our documentation. Please consult [the most recent version](/powershell/module/az.costmanagement/new-azcostmanagementquerycomparisonexpressionobject) for up-to-date information.

## SYNTAX

```
New-AzCostManagementQueryComparisonExpressionObject -Name <String> -Operator <OperatorType> -Value <String[]>
 [<CommonParameters>]
```

## DESCRIPTION
Create a in-memory object for QueryComparisonExpression

## EXAMPLES

### Example 1: Create a comparison expression object of query for cost management export
```powershell
New-AzCostManagementQueryComparisonExpressionObject -Name 'ResourceLocation' -Value @('East US', 'West Europe')
```

```output
Name             Operator Value
----             -------- -----
ResourceLocation In       {East US, West Europe}
```

This command creates a comparison expression object of query for cost management export.

## PARAMETERS

### -Name
The name of the column to use in comparison.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Operator
The operator to use for comparison.

```yaml
Type: Microsoft.Azure.PowerShell.Cmdlets.CostManagement.Support.OperatorType
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Value
Array of values to use for comparison.

```yaml
Type: System.String[]
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### Microsoft.Azure.PowerShell.Cmdlets.CostManagement.Models.Api20200601.QueryComparisonExpression

## NOTES

ALIASES

## RELATED LINKS

