---
external help file: Az.KeyVault-help.xml
Module Name: Az.KeyVault
online version: https://docs.microsoft.com/en-us/powershell/module/az.keyvault/invoke-azkeyvaultsignkey
schema: 2.0.0
---

# Invoke-AzKeyVaultSignKey

## SYNOPSIS
The SIGN operation is applicable to asymmetric and symmetric keys stored in Azure Key Vault since this operation uses the private portion of the key.
This operation requires the keys/sign permission.

## SYNTAX

### Sign (Default)
```
Invoke-AzKeyVaultSignKey -KeyName <String> -KeyVersion <String> [-Parameter <IKeySignParameters>]
 [-DefaultProfile <PSObject>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### SignExpanded
```
Invoke-AzKeyVaultSignKey -KeyName <String> -KeyVersion <String> -Algorithm <JsonWebKeySignatureAlgorithm>
 -Value <Byte[]> [-DefaultProfile <PSObject>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### SignViaIdentityExpanded
```
Invoke-AzKeyVaultSignKey -InputObject <IKeyVaultIdentity> -Algorithm <JsonWebKeySignatureAlgorithm>
 -Value <Byte[]> [-DefaultProfile <PSObject>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### SignViaIdentity
```
Invoke-AzKeyVaultSignKey -InputObject <IKeyVaultIdentity> [-Parameter <IKeySignParameters>]
 [-DefaultProfile <PSObject>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The SIGN operation is applicable to asymmetric and symmetric keys stored in Azure Key Vault since this operation uses the private portion of the key.
This operation requires the keys/sign permission.

## EXAMPLES

### Example 1
```powershell
PS C:\> {{ Add example code here }}
```

{{ Add example description here }}

## PARAMETERS

### -Algorithm
The signing/verification algorithm identifier.
For more information on possible algorithm types, see JsonWebKeySignatureAlgorithm.

```yaml
Type: Microsoft.Azure.PowerShell.Cmdlets.KeyVault.Support.JsonWebKeySignatureAlgorithm
Parameter Sets: SignExpanded, SignViaIdentityExpanded
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DefaultProfile
The credentials, account, tenant, and subscription used for communication with Azure.

```yaml
Type: System.Management.Automation.PSObject
Parameter Sets: (All)
Aliases: AzureRMContext, AzureCredential

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InputObject
Identity Parameter

```yaml
Type: Microsoft.Azure.PowerShell.Cmdlets.KeyVault.Models.IKeyVaultIdentity
Parameter Sets: SignViaIdentityExpanded, SignViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -KeyName
The name of the key.

```yaml
Type: System.String
Parameter Sets: Sign, SignExpanded
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -KeyVersion
The version of the key.

```yaml
Type: System.String
Parameter Sets: Sign, SignExpanded
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Parameter
The key operations parameters.

```yaml
Type: Microsoft.Azure.PowerShell.Cmdlets.KeyVault.Models.Api20161001.IKeySignParameters
Parameter Sets: Sign, SignViaIdentity
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Value
HELP MESSAGE MISSING

```yaml
Type: System.Byte[]
Parameter Sets: SignExpanded, SignViaIdentityExpanded
Aliases:

Required: True
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

### Microsoft.Azure.PowerShell.Cmdlets.KeyVault.Models.Api20161001.IKeyOperationResult
## NOTES

## RELATED LINKS

[https://docs.microsoft.com/en-us/powershell/module/az.keyvault/invoke-azkeyvaultsignkey](https://docs.microsoft.com/en-us/powershell/module/az.keyvault/invoke-azkeyvaultsignkey)
