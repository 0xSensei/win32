﻿---
Description: 'Is used as a handle to a CryptoAPI cryptographic service provider (CSP) or CNG CSP.'
ms.assetid: '1ad77adb-5960-4965-bddb-5967b982b034'
title: 'HCRYPTPROV\_OR\_NCRYPT\_KEY\_HANDLE'
---

# HCRYPTPROV\_OR\_NCRYPT\_KEY\_HANDLE

The **HCRYPTPROV\_OR\_NCRYPT\_KEY\_HANDLE** data type is used as a handle to a CryptoAPI [*cryptographic service provider*](security.c_gly#-security-cryptographic-service-provider-gly) (CSP) or CNG CSP. This handle must be an [**HCRYPTPROV**](hcryptprov.md) handle that has been created by using the [**CryptAcquireContext**](cryptacquirecontext.md) function or an **NCRYPT\_KEY\_HANDLE** handle that has been created by using the [**NCryptOpenKey**](security.ncryptopenkey_func) function. New applications should always pass in the **NCRYPT\_KEY\_HANDLE** handle to a CNG CSP.


```C++
typedef ULONG_PTR HCRYPTPROV_OR_NCRYPT_KEY_HANDLE;
```



## Requirements



|                                     |                                                                                       |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows Vista \[desktop apps only\]<br/>                                        |
| Minimum supported server<br/> | Windows Server 2008 \[desktop apps only\]<br/>                                  |
| Header<br/>                   | <dl> <dt>Wincrypt.h</dt> </dl> |



 

 



