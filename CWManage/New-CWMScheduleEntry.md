# New-CWMScheduleEntry
## SYNOPSIS
This function will create a new ticket.
## SYNTAX
```powershell
New-CWMScheduleEntry [[-id] <Int32>] [[-objectId] <Int32>] [[-name] <String>] [-member] <Object> [[-where] <Object>] [[-dateStart] <String>] [[-dateEnd] <String>] [[-reminder] <Object>] [[-status] <Object>] [-type] <Object> [[-span] <Object>] [[-doneFlag] <Boolean>] [[-acknowledgedFlag] <Boolean>] [[-ownerFlag] <Boolean>] [[-meetingFlag] <Boolean>] [[-allowScheduleConflictsFlag] <Boolean>] [[-addMemberToProjectFlag] <Boolean>] [[-projectRoleId] <Int32>] [[-mobileGuid] <Guid>] [[-closeDate] 

<String>] [[-hours] <Decimal>] [[-_info] <Object>] [<CommonParameters>]
```
## PARAMETERS
### -id &lt;Int32&gt;

```
Required                    false
Position                    1
Default value                0
Accept pipeline input       false
Accept wildcard characters  false
```
### -objectId &lt;Int32&gt;

```
Required                    false
Position                    2
Default value                0
Accept pipeline input       false
Accept wildcard characters  false
```
### -name &lt;String&gt;

```
Required                    false
Position                    3
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
### -member &lt;Object&gt;

```
Required                    true
Position                    4
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
### -where &lt;Object&gt;

```
Required                    false
Position                    5
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
### -dateStart &lt;String&gt;

```
Required                    false
Position                    6
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
### -dateEnd &lt;String&gt;

```
Required                    false
Position                    7
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
### -reminder &lt;Object&gt;

```
Required                    false
Position                    8
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
### -status &lt;Object&gt;

```
Required                    false
Position                    9
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
### -type &lt;Object&gt;

```
Required                    true
Position                    10
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
### -span &lt;Object&gt;

```
Required                    false
Position                    11
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
### -doneFlag &lt;Boolean&gt;

```
Required                    false
Position                    12
Default value                False
Accept pipeline input       false
Accept wildcard characters  false
```
### -acknowledgedFlag &lt;Boolean&gt;

```
Required                    false
Position                    13
Default value                False
Accept pipeline input       false
Accept wildcard characters  false
```
### -ownerFlag &lt;Boolean&gt;

```
Required                    false
Position                    14
Default value                False
Accept pipeline input       false
Accept wildcard characters  false
```
### -meetingFlag &lt;Boolean&gt;

```
Required                    false
Position                    15
Default value                False
Accept pipeline input       false
Accept wildcard characters  false
```
### -allowScheduleConflictsFlag &lt;Boolean&gt;

```
Required                    false
Position                    16
Default value                False
Accept pipeline input       false
Accept wildcard characters  false
```
### -addMemberToProjectFlag &lt;Boolean&gt;

```
Required                    false
Position                    17
Default value                False
Accept pipeline input       false
Accept wildcard characters  false
```
### -projectRoleId &lt;Int32&gt;

```
Required                    false
Position                    18
Default value                0
Accept pipeline input       false
Accept wildcard characters  false
```
### -mobileGuid &lt;Guid&gt;

```
Required                    false
Position                    19
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
### -closeDate &lt;String&gt;

```
Required                    false
Position                    20
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
### -hours &lt;Decimal&gt;

```
Required                    false
Position                    21
Default value                0
Accept pipeline input       false
Accept wildcard characters  false
```
### -_info &lt;Object&gt;

```
Required                    false
Position                    22
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
## EXAMPLES
### EXAMPLE 1
```powershell
PS C:\>$Ticket = @{

'identifier' = $Product.offerName
    'description' = $Product.offerName
    'subcategory' = @{id = 152}
    'type' = @{id = 47}
    'customerDescription' = $Product.offerName
    'cost' = $Product.unitPrice
    'price' = $Price
    'manufacturerPartNumber' = $Product.offerName
    'manufacturer' = $Manufacturer
    'productClass' = 'Agreement'
    'taxableFlag' = $true
}
New-CWMScheduleEntry @Ticket
```

## NOTES
Author: Chris Taylor

Date: 8/22/2018 
## LINKS
http://labtechconsulting.com

https://developer.connectwise.com/products/manage/rest?a=Schedule&e=ScheduleEntries&o=CREATE
