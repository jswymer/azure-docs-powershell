---
external help file: Microsoft.Azure.Commands.ApiManagement.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: 3B62AE64-D540-4D3D-BCB1-F3C4CD57E7E7
---

# Restore-AzureRmApiManagement

## SYNOPSIS
Restores an API Management Service from the specified Azure storage blob.

## SYNTAX

```
Restore-AzureRmApiManagement -ResourceGroupName <String> -Name <String> [-StorageContext] <AzureStorageContext>
 -SourceContainerName <String> -SourceBlobName <String> [-PassThru] [<CommonParameters>]
```

## DESCRIPTION
The **Restore-AzureRmApiManagement** cmdlet restores an API Management Service from the specified backup residing in an Azurestorage blob.

## EXAMPLES

### Example 1: Restore an API Management service
```
PS C:\> Restore-AzureRmApiManagement -ResourceGroupName "ContosoGroup" -Name "RestoredContosoApi" -StorageContext $StorageContext -SourceContainerName "ContosoBackups" -SourceBlobName "ContosoBackup.apimbackup"
```

This command restores an API Management service from Azure storage blob.

## PARAMETERS

### -ResourceGroupName
Specifies the name of resource group under which API Management exists.

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

### -Name
Specifies the name of the API Management instance that this cmdlet restores.

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

### -StorageContext
Specifies the storage connection context.

```yaml
Type: AzureStorageContext
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SourceContainerName
Specifies the name of the Azure storage backup source container.

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

### -SourceBlobName
Specifies the name of the Azure storage backup source blob.

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

### -PassThru
Returns an object representing the item with which you are working.
By default, this cmdlet does not generate any output.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Backup-AzureRmApiManagement](./Backup-AzureRmApiManagement.md)

[Get-AzureRmApiManagement](./Get-AzureRmApiManagement.md)

[New-AzureRmApiManagement](./New-AzureRmApiManagement.md)

[Remove-AzureRmApiManagement](./Remove-AzureRmApiManagement.md)


