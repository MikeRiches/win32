---
title: IVMVirtualNetwork PacketsDropped property
description: The PacketsDropped property contains the current number of packets dropped per second by this virtual network.
ms.assetid: '49a9d4e9-8fb9-42d3-9211-00c3b18eb546'
keywords: ["PacketsDropped property Virtual Server", "PacketsDropped property Virtual Server , IVMVirtualNetwork interface", "IVMVirtualNetwork interface Virtual Server , PacketsDropped property", "PacketsDropped property Virtual Server , VMVirtualNetwork class", "VMVirtualNetwork class Virtual Server , PacketsDropped property"]
topic_type:
- apiref
api_name:
- IVMVirtualNetwork.PacketsDropped
- IVMVirtualNetwork.get_PacketsDropped
- VMVirtualNetwork.PacketsDropped
api_location:
- VsComInterfaces.h
api_type:
- COM
---

# IVMVirtualNetwork::PacketsDropped property

The **PacketsDropped** property contains the current number of packets dropped per second by this virtual network.

This property is read-only.

## Syntax


```C++
HRESULT get_PacketsDropped(
  [out]�long *packetsDropped
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
<td><pre><code>VMVirtualNetwork.PacketsDropped( _
  ByRef packetsDropped _
)</code></pre></td>
</tr>
</tbody>
</table>



## Property value

The current number of packets dropped per second by this virtual network.

This property value is read-only.

## Error codes



| Name                                                                                          | Meaning                                                |
|-----------------------------------------------------------------------------------------------|--------------------------------------------------------|
| <dl> <dt>S\_OK</dt> </dl>              | The operation was successful.<br/>               |
| <dl> <dt>E\_POINTER</dt> </dl>         | The *packetsDropped* parameter is **NULL**.<br/> |
| <dl> <dt>DISP\_E\_EXCEPTION</dt> </dl> | An unexpected error occurred.<br/>               |



## Requirements



|                     |                                                                                                   |
|---------------------|---------------------------------------------------------------------------------------------------|
| Product<br/>  | Microsoft Virtual Server 2005 onWindows Server�2003<br/>                                    |
| Download<br/> | Microsoft Virtual Server 2005 R2 SP1 Update onWindows Server�2008orWindows Server�2003<br/> |
| Header<br/>   | <dl> <dt>VsComInterfaces.h</dt> </dl>      |



## See also

<dl> <dt>

[**IVMVirtualNetwork**](ivmvirtualnetwork.md)
</dt> </dl>

�

�




