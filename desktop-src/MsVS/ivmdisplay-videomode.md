---
title: IVMDisplay VideoMode property
description: The VideoMode property contains the current video mode of the guest operating system (Text, VGA, SVGA, and so on).
ms.assetid: '3a42e61c-c879-4704-b5e3-ba3a599578b1'
keywords: ["VideoMode property Virtual Server", "VideoMode property Virtual Server , IVMDisplay interface", "IVMDisplay interface Virtual Server , VideoMode property", "VideoMode property Virtual Server , VMDisplay interface", "VMDisplay interface Virtual Server , VideoMode property"]
topic_type:
- apiref
api_name:
- IVMDisplay.VideoMode
- IVMDisplay.get_VideoMode
- VMDisplay.VideoMode
api_location:
- VsComInterfaces.h
api_type:
- COM
---

# IVMDisplay::VideoMode property

The **VideoMode** property contains the current video mode of the guest operating system (Text, VGA, SVGA, and so on).

This property is read-only.

## Syntax


```C++
HRESULT get_VideoMode(
  [out]�VMDisplayVideoMode *videoMode
);
```

<span codelanguage="VisualBasic"></span>

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th>VB</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><pre><code>VMDisplay.VideoMode( _
  ByRef videoMode _
)</code></pre></td>
</tr>
</tbody>
</table>



## Property value

The current video mode of the guest operating system (Text, VGA, SVGA, and so on).

This property value is read-only.

## Error codes



| Name                                                                                          | Meaning                                                                |
|-----------------------------------------------------------------------------------------------|------------------------------------------------------------------------|
| <dl> <dt>S\_OK</dt> </dl>              | The operation was successful.<br/>                               |
| <dl> <dt> E\_POINTER</dt> </dl>        | The parameter is **NULL**.<br/>                                  |
| <dl> <dt>VM\_E\_VM\_UNKNOWN</dt> </dl> | The virtual machine is invalid or is not currently running.<br/> |
| <dl> <dt>VM\_E\_NO\_DISPLAY</dt> </dl> | Unable to locate a valid display for the virtual machine.<br/>   |
| <dl> <dt>DISP\_E\_EXCEPTION</dt> </dl> | An unexpected error occurred.<br/>                               |



## Requirements



|                     |                                                                                                   |
|---------------------|---------------------------------------------------------------------------------------------------|
| Product<br/>  | Microsoft Virtual Server 2005 onWindows Server�2003<br/>                                    |
| Download<br/> | Microsoft Virtual Server 2005 R2 SP1 Update onWindows Server�2008orWindows Server�2003<br/> |
| Header<br/>   | <dl> <dt>VsComInterfaces.h</dt> </dl>      |



## See also

<dl> <dt>

[**IVMDisplay**](ivmdisplay.md)
</dt> <dt>

[**VMDisplayVideoMode**](vmdisplayvideomode.md)
</dt> </dl>

�

�




