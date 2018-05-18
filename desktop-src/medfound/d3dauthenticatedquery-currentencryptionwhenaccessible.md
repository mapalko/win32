﻿---
Description: 'Returns the encryption type that is applied before content becomes accessible to the CPU or bus.'
ms.assetid: '89526bb2-1316-4730-b599-3690b1838c3e'
title: 'D3DAUTHENTICATEDQUERY\_CURRENTENCRYPTIONWHENACCESSIBLE'
---

# D3DAUTHENTICATEDQUERY\_CURRENTENCRYPTIONWHENACCESSIBLE

Returns the encryption type that is applied before content becomes accessible to the CPU or bus.



|             |                                                                                                                                              |
|-------------|----------------------------------------------------------------------------------------------------------------------------------------------|
| Query GUID  | **D3DAUTHENTICATEDQUERY\_CURRENTENCRYPTIONWHENACCESSIBLE**                                                                                   |
| Input data  | [**D3DAUTHENTICATEDCHANNEL\_QUERY\_INPUT**](d3dauthenticatedchannel-query-input.md)                                                         |
| Return data | [**D3DAUTHENTICATEDCHANNEL\_QUERYUNCOMPRESSEDENCRYPTIONLEVEL\_OUTPUT**](d3dauthenticatedchannel-queryuncompressedencryptionlevel-output.md) |



 

## Remarks

The following channel types support this query:

-   **D3DAUTHENTICATEDCHANNEL\_DRIVER\_HARDWARE**
-   **D3DAUTHENTICATEDCHANNEL\_DRIVER\_SOFTWARE**

## Requirements



|                                     |                                                                                        |
|-------------------------------------|----------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows 7 \[desktop apps only\]<br/>                                             |
| Minimum supported server<br/> | Windows Server 2008 R2 \[desktop apps only\]<br/>                                |
| Header<br/>                   | <dl> <dt>D3d9types.h</dt> </dl> |



## See also

<dl> <dt>

[Content Protection Queries](content-protection-queries.md)
</dt> <dt>

[GPU-Based Content Protection](gpu-based-content-protection.md)
</dt> <dt>

[**IDirect3DAuthenticatedChannel9::Query**](idirect3dauthenticatedchannel9-query.md)
</dt> </dl>

 

 



