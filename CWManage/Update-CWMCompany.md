# Update-CWMCompany
## SYNOPSIS
This will update a company.
## SYNTAX
```powershell
Update-CWMCompany [-CompanyID] <Object> [-Operation] <Object> [-Path] <String> [-Value] <String> [<CommonParameters>]
```
## PARAMETERS
### -CompanyID &lt;Object&gt;
The ID of the company that you are updating. Get-CWMCompanies
```
Required                    true
Position                    1
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
### -Operation &lt;Object&gt;
What you are doing with the value. 

replace, add, remove
```
Required                    true
Position                    2
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
### -Path &lt;String&gt;
The value that you want to perform the operation on.
```
Required                    true
Position                    3
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
### -Value &lt;String&gt;
The value of path.
```
Required                    true
Position                    4
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
## EXAMPLES
### EXAMPLE 1
```powershell
PS C:\>$UpdateParam = @{

CompanyID = $Company.id
    Operation = 'replace'
    Path = 'name'
    Value = $NewName
}
Update-CWMCompany @UpdateParam
```

## NOTES
Author: Chris Taylor

Date: 10/10/2018 
## LINKS
http://labtechconsulting.com

https://service.itnow.net/v4_6_release/services/apitools/apidocumentation/?a=Company&e=Companies&o=UPDATE
