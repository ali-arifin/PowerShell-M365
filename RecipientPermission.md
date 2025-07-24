# Get-RecipientPermission

Use the Get-RecipientPermission cmdlet to view information about SendAs permissions. When a user is given SendAs permission to another user or group, the user can send messages that appear to come from the other user or group.

The command below lists the recipients (user/group) for whom the user@xyz.com has SendAs permission. user@xyz.com can send messages that appear to come directly from the recipients

```powershell
Get-RecipientPermission -Trustee user@xyz.com
```

The command below lists the users who have SendAs permission on the user/group abc@xyz.com

```powershell
Get-RecipientPermission abc@xyz.com
```


# Add-RecipientPermission

This is used to give SendAs permission to user
```powershell
Add-RecipientPermission abc@xyz.com -AccessRights SendAs -Trustee user@xyz.com
```
