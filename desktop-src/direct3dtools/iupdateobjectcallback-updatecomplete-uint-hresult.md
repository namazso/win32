---
Description: A callback used to notify the host that an object was updated.
MS-HAID: vspixengine.IUpdateObjectCallback\_UpdateComplete\_UINT\_HRESULT
MSHAttr:
- PreferredSiteName:MSDN
- PreferredLib:/library/windows/desktop
title: IUpdateObjectCallback::UpdateComplete method
ms.topic: article
ms.date: 05/31/2018
---

# <span id="vspixengine.iupdateobjectcallback_updatecomplete_uint_hresult"></span>IUpdateObjectCallback::UpdateComplete method

A callback used to notify the host that an object was updated.

## Syntax


```C++
);
```

## Parameters

*objectAddress*   
The ID of the object that was updated.

*result*   
Indicates whether or not the update succeeded.

## Return value

If this method succeeds, it returns **S\_OK**. Otherwise, it returns an **HRESULT** error code.

## Requirements

<table><colgroup><col style="width: 50%" /><col style="width: 50%" /></colgroup><tbody><tr class="odd"><td><p>Header</p></td><td>Vspixengine.h</td></tr></tbody></table>

## <span id="see_also"></span>See also

[**IUpdateObjectCallback**](https://msdn.microsoft.com/library/windows/desktop/mt432823)

 

 


