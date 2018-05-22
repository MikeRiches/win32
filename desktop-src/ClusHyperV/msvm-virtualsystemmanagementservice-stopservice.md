---
title: StopService method of the Msvm\_VirtualSystemManagementService class
description: Stops the virtual system management service.
audience: developer
author: REDMOND\\markl
manager: REDMOND\\markl
ms.assetid: 'c49093e4-9d07-4bf2-8406-1b1bd7323a0a'
ms.prod: 'windows-server-dev'
ms.technology:
- 'failover-cluster-hyperv'
- 'windows-management-instrumentation'
ms.tgt_platform: multiple
keywords: ["StopService method", "StopService method, Msvm_VirtualSystemManagementService class", "Msvm_VirtualSystemManagementService class, StopService method"]
topic_type:
- apiref
api_name:
- Msvm_VirtualSystemManagementService.StopService
api_location:
- VMMS.exe
api_type:
- COM
---

# StopService method of the Msvm\_VirtualSystemManagementService class

Stops the virtual system management service.

## Syntax


```mof
uint32 StopService();
```



## Parameters

This method has no parameters.

## Return value

The possible return values are:

<dl> <dt>

**Completed with No Error** (0)
</dt> <dt>

**Not supported** (1)
</dt> </dl>

## Requirements



|                                     |                                                                                                        |
|-------------------------------------|--------------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | None supported<br/>                                                                              |
| Minimum supported server<br/> | Windows Server�2016<br/>                                                                         |
| Namespace<br/>                | Root\\HyperVCluster\\v2<br/>                                                                     |
| Header<br/>                   | <dl> <dt>Sdoias.h</dt> </dl>                    |
| MOF<br/>                      | <dl> <dt>WindowsHyperVCluster.V2.mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>VMMS.exe</dt> </dl>                    |



## See also

<dl> <dt>

[**Msvm\_VirtualSystemManagementService**](msvm-virtualsystemmanagementservice.md)
</dt> </dl>

�

�




