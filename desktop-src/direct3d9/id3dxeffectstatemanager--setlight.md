---
Description: A callback function that must be implemented by a user to set a light.
ms.assetid: 3b9b2cbd-79f5-4ea4-a47b-da23b091adfd
title: ID3DXEffectStateManager::SetLight method
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# ID3DXEffectStateManager::SetLight method

A callback function that must be implemented by a user to set a light.

## Syntax


```C++
HRESULT SetLight(
  [in]       DWORD     Index,
  [in] const D3DLight9 *pLight
);
```



## Parameters

<dl> <dt>

*Index* \[in\]
</dt> <dd>

Type: **[**DWORD**](https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46)**

The zero-based index of the light. This is the same index in [**IDirect3DDevice9::SetLight**](/windows/desktop/api/d3d9helper/nf-d3d9-idirect3ddevice9-setlight).

</dd> <dt>

*pLight* \[in\]
</dt> <dd>

Type: **const [**D3DLight9**](d3dlight9.md)\***

The light object. See [**D3DLIGHT9**](d3dlight9.md).

</dd> </dl>

## Return value

Type: **[**HRESULT**](https://msdn.microsoft.com/windows/desktop/455d07e9-52c3-4efb-a9dc-2955cbfd38cc)**

The user-implemented method should return S\_OK. If the callback fails when setting the device state, either of the following will occur:

-   The effect will fail during [**ID3DXEffect::BeginPass**](id3dxeffect--beginpass.md).
-   The dynamic effect state call (such as [**IDirect3DDevice9::SetLight**](/windows/desktop/api/d3d9helper/nf-d3d9-idirect3ddevice9-setlight)) will fail.

## Requirements



|                    |                                                                                          |
|--------------------|------------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>D3DX9Effect.h</dt> </dl> |
| Library<br/> | <dl> <dt>D3dx9.lib</dt> </dl>     |



## See also

<dl> <dt>

[ID3DXEffectStateManager](id3dxeffectstatemanager.md)
</dt> </dl>

 

 



