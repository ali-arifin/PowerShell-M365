# :white_check_mark: Get-DistributionGroup

The command below returns a summary list of all distribution groups and mail-enabled security groups in the organization.

```powershell
Get-DistributionGroup
```
The command below returns detailed information about the distribution group abc@xyz.com

```powershell
Get-DistributionGroup -Identity abc@xyz.com | Format-List
```


# :white_check_mark: Get-DistributionGroupMember

Use the Get-DistributionGroupMember cmdlet to view the members of distribution groups and mail-enabled security groups

```powershell
Get-DistributionGroupMember -Identity abc@xyz.com | Select PrimarySMTPAddress
```

# :white_check_mark: Get-DynamicDistributionGroup

The command below returns a summary list of all dynamic distribution groups in the organization

```powershell
Get-DynamicDistributionGroup
```
The command below returns detailed information about the dynamic distribution group abc@xyz.com


```powershell
Get-DynamicDistributionGroup -Identity abc@xyz.com | Format-List
```

# :white_check_mark: Get-DynamicDistributionGroupMember

The command below returns the existing members for the dynamic distribution group abc@xyz.com

```powershell
Get-DynamicDistributionGroupMember -Identity abc@xyz.com
```




