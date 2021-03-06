---
title: LogonCommands
description: LogonCommands
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: f5e2b20d-1931-4811-86df-854aa2ffdf25
ms.mktglfcycl: deploy
ms.sitesec: msdn
ms.author: alhopper
ms.date: 05/02/2017
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-oem
---

# LogonCommands


`LogonCommands` specifies one or more commands to run the first time a user logs on to the computer.

**Note**  
This setting cannot be used to launch applications that require administrative privileges to run.

 

## Child Elements


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p>[AsynchronousCommand](microsoft-windows-shell-setup-logoncommands-asynchronouscommand.md)</p></td>
<td><p>Specifies a single command to run the first time a user logs on to the computer.</p></td>
</tr>
</tbody>
</table>

 

## Valid Configuration Passes


oobeSystem

## Parent Hierarchy


[Microsoft-Windows-Shell-Setup](microsoft-windows-shell-setup.md) | **LogonCommands**

## Applies To


For a list of the supported Windows editions and architectures that this component supports, see [Microsoft-Windows-Shell-Setup](microsoft-windows-shell-setup.md).

## XML Example


The following XML output shows how to set logon commands.

```
<LogonCommands>
   <AsynchronousCommand wcm:action="add">
      <CommandLine>c:\asynccommands\command1.exe</CommandLine>
      <Description>Description_of_command1</Description>
      <Order>1</Order>
   </AsynchronousCommand>
   <AsynchronousCommand wcm:action="add">
      <CommandLine>c:\asynccommands\command2.exe</CommandLine>
      <Description>Description_of_command2</Description>
      <Order>2</Order>
   </AsynchronousCommand>
</LogonCommands>
```

## Related topics


[Microsoft-Windows-Shell-Setup](microsoft-windows-shell-setup.md)

 

 







