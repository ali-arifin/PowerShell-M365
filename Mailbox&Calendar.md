# MailboxPermission

For getting information about who has access to a user mailbox or shared mailbox:

```powershell
Get-MailboxPermission "abc@xyz.com"
```
The output also provides information about the level of access

# MailboxFolderPermission

For getting information about who has access to a specific folder inside the mailbox (like who has access to the Calendar):
```powershell
Get-MailboxFolderPermission "abc@xyz.com:\Calendar"
```

Grant Reviewer access of someone's calendar to a user "user@xyz.com"
```powershell
Set-MailboxFolderPermission -Identity abc@xyz.com:\Calendar -User user@xyz.com -AccessRights Reviewer
```

# CalendarProcessing

This command is useful for viewing calendar properties:
```powershell
Get-CalendarProcessing -Identity abc@xyz.com | Format-List
```
The output gives valuable information like AddOrganizerToSubject, DeleteComments, DeleteSubject
