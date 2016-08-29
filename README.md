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

service-related
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
Copy-Item C:\ke.txt C:\ke2.txt
```
