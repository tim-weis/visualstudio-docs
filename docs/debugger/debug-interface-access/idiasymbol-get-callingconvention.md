---
description: "Returns an indicator of a methods calling convention."
title: "IDiaSymbol::get_callingConvention"
ms.date: "11/04/2016"
ms.topic: "reference"
dev_langs:
  - "C++"
helpviewer_keywords:
  - "IDiaSymbol::get_callingConvention method"
author: "mikejo5000"
ms.author: "mikejo"
manager: jmartens
ms.subservice: debug-diagnostics
---
# IDiaSymbol::get_callingConvention

Returns an indicator of a methods calling convention.

## Syntax

```C++
HRESULT get_callingConvention ( 
   DWORD* pRetVal
);
```

#### Parameters
 `pRetVal`

[out] Returns a value from the [CV_call_e Enumeration](../../debugger/debug-interface-access/cv-call-e.md) enumeration that specifies a method's calling convention.

## Return Value
 If successful, returns `S_OK`; otherwise, returns `S_FALSE` or an error code.

> [!NOTE]
> A return value of `S_FALSE` means the property is not available for the symbol.

## Requirements

|Requirement|Description|
|-----------------|-----------------|
|Header:|dia2.h|
|Version:|DIA SDK v7.0|

## See also
- [IDiaSymbol](../../debugger/debug-interface-access/idiasymbol.md)
- [CV_call_e Enumeration](../../debugger/debug-interface-access/cv-call-e.md)
