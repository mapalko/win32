---
title: EvalRat Object
description: EvalRat Object
ms.assetid: '6a67cdb1-9a5c-4130-a29c-05c584702fd9'
---

# EvalRat Object

This topic applies to Windows XP Service Pack 1 or later.

The **EvalRat** object evaluates program ratings and determines whether a program should be blocked under the current set of permissions. The permissions are set by the application. The rating itself is parsed from the broadcast stream using the [XDSToRat](xdstorat-object.md) object.

This object is created by third parties. It must support the **IEvalRat** interface. This object is used by the Encrypter/Tagger filter and the Decrypter/Detagger filter. Applications do not use this object directly.



|            |                              |
|------------|------------------------------|
| CLSID      | CLSID\_EvalRat               |
| Interfaces | [**IEvalRat**](ievalrat.md) |



 

## Related topics

<dl> <dt>

[TV Ratings Components](tv-ratings-components.md)
</dt> </dl>

 

 



