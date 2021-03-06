# Remove-CWMMarketingGroupCompany
## SYNOPSIS
This function will remove a company from a marketing group.
## SYNTAX
```powershell
Remove-CWMMarketingGroupCompany [-ID] <Int32> [-CompanyId] <Int32> [<CommonParameters>]
```
## PARAMETERS
### -ID &lt;Int32&gt;
The ID of the group you want to delete from.
```
Required                    true
Position                    1
Default value                0
Accept pipeline input       false
Accept wildcard characters  false
```
### -CompanyId &lt;Int32&gt;
The ID if the company you want to remove from the group.
```
Required                    true
Position                    2
Default value                0
Accept pipeline input       false
Accept wildcard characters  false
```
## EXAMPLES
### EXAMPLE 1
```powershell
PS C:\>Remove-CWMMarketingGroupCompany -id 1 -CompanyId 1

Will remove company 1 from marketing group 1
```

## NOTES
Author: Chris Taylor

Date: 1/9/2019 
## LINKS
http://labtechconsulting.com

https://developer.connectwise.com/products/manage/rest?a=Marketing&e=GroupCompanies&o=DELETE
