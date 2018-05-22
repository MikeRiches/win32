---
Description: 'Associates the Msvm\_ReferencePointCollection to the contained Msvm\_VirtualSystemReferencePoint objects.'
ms.assetid: '826125c3-0a89-4573-ac28-88588eac248d'
title: 'Msvm\_CollectedReferencePoints class'
---

# Msvm\_CollectedReferencePoints class

Associates the [**Msvm\_ReferencePointCollection**](msvm-referencepointcollection.md) to the contained [**Msvm\_VirtualSystemReferencePoint**](msvm-virtualsystemreferencepoint.md) objects.

The following syntax is simplified from Managed Object Format (MOF) code and includes all of the inherited properties.

## Syntax

``` syntax
[Association, Dynamic, Provider("VmmsWmiInstanceAndMethodProvider"), AMENDMENT]
class Msvm_CollectedReferencePoints : CIM_CollectedMSEs
{
  Msvm_ReferencePointCollection��� REF Collection;
  Msvm_VirtualSystemReferencePoint REF Member;
};
```

## Members

The **Msvm\_CollectedReferencePoints** class has these types of members:

-   [Properties](#properties)

### Properties

The **Msvm\_CollectedReferencePoints** class has these properties.

<dl> <dt>

**Collection**
</dt> <dd> <dl> <dt>

Data type: **Msvm\_ReferencePointCollection**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: [**Aggregate**](https://msdn.microsoft.com/library/aa393650), [**Override**](https://msdn.microsoft.com/library/aa393650) ("Collection")
</dt> </dl>

An [**Msvm\_ReferencePointCollection**](msvm-referencepointcollection.md) grouping or 'bag' object that represents the collection.

</dd> <dt>

**Member**
</dt> <dd> <dl> <dt>

Data type: **Msvm\_VirtualSystemReferencePoint**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: [**Override**](https://msdn.microsoft.com/library/aa393650) ("Member")
</dt> </dl>

An [**Msvm\_VirtualSystemReferencePoint**](msvm-virtualsystemreferencepoint.md) containing the members of the collection.

</dd> </dl>

## Requirements



|                                     |                                                                                                         |
|-------------------------------------|---------------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows�10 \[desktop apps only\]<br/>                                                             |
| Minimum supported server<br/> | Windows Server�2016<br/>                                                                          |
| Namespace<br/>                | Root\\virtualization\\v2<br/>                                                                     |
| MOF<br/>                      | <dl> <dt>WindowsVirtualization.V2.mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Vmms.exe</dt> </dl>                     |



## See also

<dl> <dt>

[**CIM\_CollectedMSEs**](cim-collectedmses.md)
</dt> </dl>

�

�



