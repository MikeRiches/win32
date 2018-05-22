---
Description: 'The CopyPalette method copies the palette from any VIDEOINFO structure to any palettized VIDEOINFO structure.'
ms.assetid: 'ea06b40b-3f96-4c11-921c-52f3a44e0a30'
title: 'CImagePalette.CopyPalette method'
---

# CImagePalette.CopyPalette method

The `CopyPalette` method copies the palette from any [**VIDEOINFO**](videoinfo.md) structure to any palettized **VIDEOINFO** structure.

## Syntax


```C++
HRESULT CopyPalette(
  �const CMediaType *pSrc,
  �const CMediaType *pDest
);
```



## Parameters

<dl> <dt>

*pSrc* 
</dt> <dd>

Pointer to the source media type.

</dd> <dt>

*pDest* 
</dt> <dd>

Pointer to the destination media type.

</dd> </dl>

## Return value

Returns S\_OK if the palette was copied. Returns S\_FALSE if either the source or destination media type does not have a palette.

## Remarks

The *pDest* media type must be a palettized format with a color depth of 8 bits or less. The *pSrc* media type can be any [**VIDEOINFOHEADER**](videoinfoheader.md) type with a palette, including YUV and true-color formats with palette entries. The method copies the palette entries from *pSrc* into a new palette, and attaches the new palette to *pDest*.

## Requirements



|                    |                                                                                                                                                                                            |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>Winutil.h (include Streams.h)</dt> </dl>                                                                                   |
| Library<br/> | <dl> <dt>Strmbase.lib (retail builds); </dt> <dt>Strmbasd.lib (debug builds)</dt> </dl> |



## See also

<dl> <dt>

[**CImagePalette Class**](cimagepalette.md)
</dt> </dl>

�

�



