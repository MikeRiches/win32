---
Description: Access the mesh's vertex buffer after it has been committed to the device with ID3DX10Mesh::CommitToDevice. This is different from ID3DX10Mesh::GetVertexBuffer, which returns the vertex buffer before it has been committed to the device.
ms.assetid: 621d9105-e55d-47b8-8557-8adb7db19d66
title: ID3DX10Mesh::GetDeviceVertexBuffer method
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# ID3DX10Mesh::GetDeviceVertexBuffer method

Access the mesh's vertex buffer after it has been committed to the device with [**ID3DX10Mesh::CommitToDevice**](id3dx10mesh-committodevice.md). This is different from [**ID3DX10Mesh::GetVertexBuffer**](id3dx10mesh-getvertexbuffer.md), which returns the vertex buffer before it has been committed to the device.

## Syntax


```C++
HRESULT GetDeviceVertexBuffer(
  [in]  UINT         iBuffer,
  [out] ID3D10Buffer **ppVertexBuffer
);
```



## Parameters

<dl> <dt>

*iBuffer* \[in\]
</dt> <dd>

Type: **[**UINT**](https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46)**

An index identifying which vertex buffer to access.

</dd> <dt>

*ppVertexBuffer* \[out\]
</dt> <dd>

Type: **[**ID3D10Buffer**](/windows/desktop/api/D3D10/nn-d3d10-id3d10buffer)\*\***

The vertex buffer after it has been committed to the device.

</dd> </dl>

## Return value

Type: **[**HRESULT**](https://msdn.microsoft.com/windows/desktop/455d07e9-52c3-4efb-a9dc-2955cbfd38cc)**

The return value is one of the values listed in [Direct3D 10 Return Codes](d3d10-graphics-reference-returnvalues.md).

## Requirements



|                    |                                                                                       |
|--------------------|---------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>D3DX10.h</dt> </dl>   |
| Library<br/> | <dl> <dt>D3DX10.lib</dt> </dl> |



## See also

<dl> <dt>

[ID3DX10Mesh](id3dx10mesh.md)
</dt> <dt>

[D3DX Interfaces](d3d10-graphics-reference-d3dx10-interfaces.md)
</dt> </dl>

 

 



