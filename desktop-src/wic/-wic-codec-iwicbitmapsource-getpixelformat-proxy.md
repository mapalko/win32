---
Description: 'Proxy function for the GetPixelFormat method.'
ms.assetid: '0879bfb7-0175-4275-a093-a69b39c66a41'
title: 'IWICBitmapSource\_GetPixelFormat\_Proxy function'
---

# IWICBitmapSource\_GetPixelFormat\_Proxy function

Proxy function for the [**GetPixelFormat**](-wic-codec-iwicbitmapsource-getpixelformat.md) method.

## Syntax


```C++
HRESULT IWICBitmapSource_GetPixelFormat_Proxy(
  _In_��IWICBitmapSource ��*THIS_PTR,
  _Out_�WICPixelFormatGUID *pPixelFormat
);
```



## Parameters

<dl> <dt>

*THIS\_PTR* \[in\]
</dt> <dd>

Type: **[**IWICBitmapSource**](-wic-codec-iwicbitmapsource.md)\***

Pointer to this [**IWICBitmapSource**](-wic-codec-iwicbitmapsource.md) object.

</dd> <dt>

*pPixelFormat* \[out\]
</dt> <dd>

Type: **WICPixelFormatGUID\***

A pointer that receives the pixel format GUID the bitmap is stored in.

</dd> </dl>

## Return value

Type: **HRESULT**

If this function succeeds, it returns **S\_OK**. Otherwise, it returns an **HRESULT** error code.

## Remarks

## Requirements



|                                     |                                                                                                                                                                  |
|-------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows�XP with SP2, Windows�Vista \[desktop apps only\]<br/>                                                                                              |
| Minimum supported server<br/> | Windows Server�2008 \[desktop apps only\]<br/>                                                                                                             |
| DLL<br/>                      | <dl> <dt>Windowscodecs.dll; </dt> <dt>Wincodec.lib</dt> </dl> |



�

�



