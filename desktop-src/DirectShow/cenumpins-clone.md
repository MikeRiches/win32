---
Description: 'The Clone method makes a copy of the enumerator with the same enumeration state. This method implements the IEnumPins::Clone method.'
ms.assetid: '6e44c970-b90a-4bdb-8c60-dd8f31516249'
title: 'CEnumPins.Clone method'
---

# CEnumPins.Clone method

The `Clone` method makes a copy of the enumerator with the same enumeration state. This method implements the [**IEnumPins::Clone**](ienumpins-clone.md) method.

## Syntax


```C++
HRESULT Clone(
  �IEnumPins **ppEnum
);
```



## Parameters

<dl> <dt>

*ppEnum* 
</dt> <dd>

Address of a variable that receives a pointer to the [**IEnumPins**](ienumpins.md) interface of the new enumerator.

</dd> </dl>

## Return value

Returns one of the **HRESULT** values shown in the following table.



| Return code                                                                                                | Description                                                                            |
|------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------|
| <dl> <dt>**S\_OK**</dt> </dl>                       | Success.<br/>                                                                    |
| <dl> <dt>**E\_OUTOFMEMORY**</dt> </dl>              | Insufficient memory.<br/>                                                        |
| <dl> <dt>**E\_POINTER**</dt> </dl>                  | **NULL** pointer argument.<br/>                                                  |
| <dl> <dt>**VFW\_E\_ENUM\_OUT\_OF\_SYNC**</dt> </dl> | The filter's state has changed and is now inconsistent with the enumerator.<br/> |



�

## Requirements



|                    |                                                                                                                                                                                            |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>Amfilter.h (include Streams.h)</dt> </dl>                                                                                  |
| Library<br/> | <dl> <dt>Strmbase.lib (retail builds); </dt> <dt>Strmbasd.lib (debug builds)</dt> </dl> |



## See also

<dl> <dt>

[**CEnumPins Class**](cenumpins.md)
</dt> </dl>

�

�



