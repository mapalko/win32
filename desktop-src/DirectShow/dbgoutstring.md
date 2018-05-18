---
Description: 'The DbgOutString function sends a string to the debug output location. Ignored in retail builds.'
ms.assetid: '644bf4f7-ec2d-466e-85c6-690dd44da702'
title: DbgOutString function
---

# DbgOutString function

The **DbgOutString** function sends a string to the debug output location. Ignored in retail builds.

## Syntax


```C++
void DbgOutString(
  �LPCTSTR psz
);
```



## Parameters

<dl> <dt>

*psz* 
</dt> <dd>

String to output.

</dd> </dl>

## Return value

This function does not return a value.

## Remarks

In debug builds, this function always outputs the string, regardless of the current debug output levels. For finer control over the output, use the [**DbgLog**](dbglog.md) macro.

## Examples


```C++
DbgOutString("Creating the filter graph...\n"); 
```



## Requirements



|                    |                                                                                                                                                                                            |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>Wxdebug.h (include Streams.h)</dt> </dl>                                                                                   |
| Library<br/> | <dl> <dt>Strmbase.lib (retail builds); </dt> <dt>Strmbasd.lib (debug builds)</dt> </dl> |



## See also

<dl> <dt>

[Debug Output Functions](debug-output-functions.md)
</dt> </dl>

�

�



