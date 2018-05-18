﻿---
Description: 'Retrieves a child object in this file data object.'
ms.assetid: '0c4f1efa-f096-443d-a482-a3c5a9138c3d'
title: 'ID3DXFileData::GetChild method'
---

# ID3DXFileData::GetChild method

Retrieves a child object in this file data object.

## Syntax


```C++
HRESULT GetChild(
  [in] SIZE_T        uiChild,
  [in] ID3DXFileData **ppChild
);
```



## Parameters

<dl> <dt>

*uiChild* \[in\]
</dt> <dd>

Type: **[**SIZE\_T**](winprog.windows_data_types)**

ID of the child object to retrieve.

</dd> <dt>

*ppChild* \[in\]
</dt> <dd>

Type: **[**ID3DXFileData**](id3dxfiledata.md)\*\***

Address of a pointer to receive the child object's interface pointer.

</dd> </dl>

## Return value

Type: **[**HRESULT**](455d07e9-52c3-4efb-a9dc-2955cbfd38cc)**

If the method succeeds, the return value is S\_OK. If the method fails, the return value can be one of the following values: D3DXFERR\_BADVALUE, D3DXFERR\_NOMOREOBJECTS.

## Requirements



|                    |                                                                                       |
|--------------------|---------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>D3DX9Xof.h</dt> </dl> |
| Library<br/> | <dl> <dt>D3dx9.lib</dt> </dl>  |



## See also

<dl> <dt>

[ID3DXFileData](id3dxfiledata.md)
</dt> </dl>

 

 



