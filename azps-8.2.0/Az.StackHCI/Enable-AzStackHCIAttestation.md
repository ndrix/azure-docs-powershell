---
external help file: 
Module Name: Az.StackHCI
online version: https://docs.microsoft.com/powershell/module/az.stackhci/enable-azstackhciattestation
schema: 2.0.0
content_git_url: https://github.com/Azure/azure-powershell/blob/main/src/StackHCI/help/Enable-AzStackHCIAttestation.md
original_content_git_url: https://github.com/Azure/azure-powershell/blob/main/src/StackHCI/help/Enable-AzStackHCIAttestation.md
---

# Enable-AzStackHCIAttestation

## SYNOPSIS
Enable-AzStackHCIAttestation configures the host and enables specified guests for IMDS attestation.

> [!NOTE]
>This is the previous version of our documentation. Please consult [the most recent version](/powershell/module/az.stackhci/enable-azstackhciattestation) for up-to-date information.

## SYNTAX

```
Enable-AzStackHCIAttestation [[-ComputerName] <String>] [-AddVM] [-Credential <PSCredential>] [-Force]
 [-Confirm] [-WhatIf] [<CommonParameters>]
```

## DESCRIPTION
Enable-AzStackHCIAttestation configures the host and enables specified guests for IMDS attestation.

## EXAMPLES

### Example 1: 
```powershell
Enable-AzStackHCIAttestation -AddVM
```

```output
ComputerName  Status Expiration
------------  ------ ----------
HCINODE2     Expired
```

Invoking on one of the cluster node.

## PARAMETERS

### -AddVM
After enabling each cluster node for Attestation, add all guests on each node.

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

### -ComputerName
Specifies the AzureStack HCI host to perform the operation on.
Note: this host should match the host of VMName.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases:

Required: False
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Credential
Specifies the credential for the ComputerName.
Default is the current user executing the Cmdlet.

```yaml
Type: System.Management.Automation.PSCredential
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Force
No confirmations.

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
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### System.Management.Automation.PSObject

## NOTES

ALIASES

## RELATED LINKS

