---
Description: Requests to get information about what columns (fields) this object table request type supports.
MS-HAID: vspixengine.IObjectTableRequest\_RequestSupportedColumnsAsync\_IObjectTableCallback\_ptr\_DWORD
MSHAttr:
- PreferredSiteName:MSDN
- PreferredLib:/library/windows/desktop
title: IObjectTableRequest::RequestSupportedColumnsAsync method
ms.topic: article
ms.date: 05/31/2018
---

# <span id="vspixengine.iobjecttablerequest_requestsupportedcolumnsasync_iobjecttablecallback_ptr_dword"></span>IObjectTableRequest::RequestSupportedColumnsAsync method

Requests to get information about what columns (fields) this object table request type supports.

## Syntax


```C++
);
```

## Parameters

*requestCallback*   
The address of callback used to notify the host of results.

*progressIntervalMsecs*   
Not used.

## Return value

If this method succeeds, it returns **S\_OK**. Otherwise, it returns an **HRESULT** error code.

## Requirements

<table><colgroup><col style="width: 50%" /><col style="width: 50%" /></colgroup><tbody><tr class="odd"><td><p>Header</p></td><td>Vspixengine.h</td></tr></tbody></table>

## <span id="see_also"></span>See also

[**IObjectTableRequest**](https://msdn.microsoft.com/library/windows/desktop/mt422699)

 

 


