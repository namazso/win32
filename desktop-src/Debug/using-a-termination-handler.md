---
Description: 'The following example shows how a termination handler is used to ensure that resources are released when execution of a guarded body of code terminates.'
ms.assetid: '442af2a3-d62a-4dd8-a934-da69c1d2a738'
title: Using a Termination Handler
---

# Using a Termination Handler

The following example shows how a termination handler is used to ensure that resources are released when execution of a guarded body of code terminates. In this case, a thread uses the [**EnterCriticalSection**](base.entercriticalsection) function to wait for ownership of a critical section object. When the thread is finished executing the code that is protected by the critical section, it must call the [**LeaveCriticalSection**](base.leavecriticalsection) function to make the critical section object available to other threads. Using a termination handler guarantees that this will happen. For more information, see [critical section objects](base.critical_section_objects).


```C++
LPTSTR lpBuffer = NULL; 
CRITICAL_SECTION CriticalSection; 

// EnterCriticalSection synchronizes code with other threads. 
EnterCriticalSection(&amp;CriticalSection); 
 
__try 
{ 
    // Perform a task that may cause an exception. 
    lpBuffer = (LPTSTR) LocalAlloc(LPTR, 10); 
    StringCchCopy(lpBuffer, 10, TEXT("Hello"));

    _tprintf(TEXT("%s\n"),lpBuffer); 
    LocalFree(lpBuffer); 
} 
__finally 
{ 
    // LeaveCriticalSection is called even if an exception occurred. 
    LeaveCriticalSection(&amp;CriticalSection); 
}
```



 

 


