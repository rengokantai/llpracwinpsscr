#### llpracwinpsscr
######2.1 Commonly Used Cmdlets
WS = workingset memory
```
Get-Process | Select-Object Name,WS
```
sort by memory usage
```
Get-Process | Sort-Object WS
```
Descending
```
Get-Process | Sort-Object WS -Descending | Select-Object Name,WS
```
show last 5
```
Get-Process | Sort-Object WS -Descending | Select-Object Name,WS -Last 5
```

service-related (default=Format-Table)
```
Get-Service VSS |Select-Object Name |Format-List
```
Type = cat in linux
```
Type C:\ke.txt
Get-Content C:\ke.txt
```
clear screen
```
CLS
Clear-Host
```
copy
```
Copy-Item C:\ke.txt D:\
```
Get-ChildItem=dir
```
Get-ChildItem C:\
```
get history
```
Get-History
```
######2.3 Working with Var
```
[int]$x+[int]$y
```
array type
```
$arr = "a","b"
```
printout
```
$arr  //onebyone
Write-Host $arr
Write-Host $arr[2] //0 based
```
assign a command to var, do not use quote
```
$GC = Get-Command
$GC
$GC.count
```
######2.4 An Introduction to Module
```
Get-Module
Import-Module mn
```
```
Get-Command -Module Hyper-V
```
