---
Description: 'All fax service providers (FSPs) must use a private heap for memory allocations.'
ms.assetid: 'e1ef250a-407d-4d96-a9be-0ae60c748dc0'
title: Allocating Memory
---

# Allocating Memory

All fax service providers (FSPs) must use a private heap for memory allocations. The fax service creates a private heap for each FSP when it loads the FSP's DLL, and it passes the heap handle on a call to the [**FaxDevInitialize**](-mfax-faxdevinitialize.md) function. The fax service deallocates the heap when it unloads the DLL.

The FSP should wrap all memory allocations and deallocations inside the DLL with private functions. The private functions should call the [HeapAlloc](http://msdn.microsoft.com/library/en-us/memory/base/heapalloc.asp) and [HeapFree](http://msdn.microsoft.com/library/en-us/memory/base/heapfree.asp) functions with the heap handle passed to [**FaxDevInitialize**](-mfax-faxdevinitialize.md).

This method achieves a robust server with the extensibility of the service provider model, and it isolates memory problems specific to the FSP. For more information about allocating memory, see [Operating in a Multithreaded Environment](-mfax-operating-in-a-multithreaded-environment.md).

 

 


