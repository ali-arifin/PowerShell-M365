# MailboxStatistics

This command provides a lot of metrics like ItemCount, DeletedItemCount, TotalDeletedItemSize, TotalItemSize, LastUserAccessTime etc.

```powershell
Get-MailboxStatistics abc@xyz.com | fl *
```

This command provides metrics starting from the word 'Total':
```powershell
Get-MailboxStatistics abc@xyz.com | fl total*
```

This command provides some metrics for each mailbox folder:
```powershell
Get-MailboxFolderStatistics abc@xyz.com | select identity, itemsinfolder, deleteditemsinfolder, foldersize, itemsinfolderandsubfolders
```
