# Get-CWMTicketConfiguration
## SYNOPSIS
This function will list configs attached to a ticket.
## SYNTAX
```powershell
Get-CWMTicketConfiguration [-TicketID] <Int32> [[-page] <Int32>] [[-pageSize] <Int32>] [-all] [<CommonParameters>]
```
## PARAMETERS
### -TicketID &lt;Int32&gt;
The id of the ticket you want to retreive configurations for.
```
Required                    true
Position                    1
Default value                0
Accept pipeline input       false
Accept wildcard characters  false
```
### -page &lt;Int32&gt;
Used in pagination to cycle through results
```
Required                    false
Position                    2
Default value                0
Accept pipeline input       false
Accept wildcard characters  false
```
### -pageSize &lt;Int32&gt;
Number of results returned per page (Defaults to 25)
```
Required                    false
Position                    3
Default value                0
Accept pipeline input       false
Accept wildcard characters  false
```
### -all &lt;SwitchParameter&gt;
Return all results
```
Required                    false
Position                    named
Default value                False
Accept pipeline input       false
Accept wildcard characters  false
```
## EXAMPLES
### EXAMPLE 1
```powershell
PS C:\>Get-CWMTicketConfiguration -TicketID 1

Will return all configurations for ticket 1
```

## NOTES
Author: Chris Taylor

Date: 10/22/2018 
## LINKS
http://labtechconsulting.com

https://developer.connectwise.com/products/manage/rest?a=Service&e=Tickets&o=CONFIGURATIONS
