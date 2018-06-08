---
Description: In addition to certificates and certificate revocation lists (CRL), the CryptoAPI certificate store supports the certificate trust list (CTL).
ms.assetid: b0f7e7ce-f981-4f3f-83a0-7792224ce0e3
title: Certificate Trust List Overview
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# Certificate Trust List Overview

In addition to certificates and [*certificate revocation lists*](https://msdn.microsoft.com/db46def4-bfdc-4801-a57d-d568e94a2dbb) (CRL), the [*CryptoAPI*](https://msdn.microsoft.com/db46def4-bfdc-4801-a57d-d568e94a2dbb) [*certificate store*](https://msdn.microsoft.com/db46def4-bfdc-4801-a57d-d568e94a2dbb) supports the [*certificate trust list*](https://msdn.microsoft.com/db46def4-bfdc-4801-a57d-d568e94a2dbb) (CTL). A CTL is a predefined list of items signed by a trusted entity. A CTL is a list of [*hashes*](https://msdn.microsoft.com/4165b820-30fc-477e-a690-81109f161323) of certificates or a list of file names. All the items in the list are authenticated and approved by a trusted signing entity. A [**CTL\_CONTEXT**](/windows/desktop/api/Wincrypt/ns-wincrypt-_ctl_context) structure is similar to certificate and CRL context structures. A CTL context can be persisted to the certificate store.

A CryptoAPI CTL is a list of items that has been signed by a trusted entity. The list of items could be anything, such as a list of hashes of certificates, or a list of file names. In most cases, a CTL is a list of hashed certificate contexts. All the items in the list are authenticated and approved by the signing entity. The primary use of CTLs is to verify signed Messages, using the CTL as a source of trusted [*root certificates*](https://msdn.microsoft.com/ce589e18-02ac-42c2-b76b-776deb686bbd).

The [**CTL\_CONTEXT**](/windows/desktop/api/Wincrypt/ns-wincrypt-_ctl_context) structure is similar to the certificate and CRL context structures; however, unlike the certificate and CRL context structures, the **CTL\_CONTEXT** structure contains a **hCryptMsg** member. This handle is opened by a call to any of the functions that return a **CTL\_CONTEXT** structure, making it possible to use the message functions to verify the CTL's signature. This verification is necessary to ensure that a CTL is not a bogus CTL planted by a rogue entity.

For procedures to create a signed CTL and save it to a certificate store, see [Creating, Signing, and Storing a CTL](creating-signing-and-storing-a-ctl.md). Also see [Verifying a CTL](verifying-a-ctl.md) and [Verifying Signed Messages By Using CTLs](verifying-signed-messages-by-using-ctls.md) for step by step verification procedures.

 

 


