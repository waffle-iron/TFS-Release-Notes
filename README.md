[![Stories in Ready](https://badge.waffle.io/vbjay/TFS-Release-Notes.png?label=ready&title=Ready)](https://waffle.io/vbjay/TFS-Release-Notes)
# TFS-Release-Notes
Generates a list of files changed from a work item.

# Use

```powershell
Import-Module '.\TFS Release Notes.dll'

$tfs=Get-Tfs <URI to TFS project collection>
$wi=$tfs.WIT.GetWorkItem(<work item id>)

Get-WorkItemFiles <URI to TFS project collection> <work item id>
Get-WorkItemFiles $tfs <work item id>
```
