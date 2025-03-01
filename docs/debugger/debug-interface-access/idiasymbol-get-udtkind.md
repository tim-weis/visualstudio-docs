---
description: "Retrieves the variety of a user-defined type (UDT)."
title: "IDiaSymbol::get_udtKind"
ms.date: "11/04/2016"
ms.topic: "reference"
dev_langs:
  - "C++"
helpviewer_keywords:
  - "IDiaSymbol::get_udtKind method"
author: "mikejo5000"
ms.author: "mikejo"
manager: jmartens
ms.subservice: debug-diagnostics
---
# IDiaSymbol::get_udtKind

Retrieves the variety of a user-defined type (UDT).

## Syntax

```C++
HRESULT get_udtKind ( 
   DWORD* pRetVal
);
```

#### Parameters
 `pRetVal`

[out] Returns a value from the [UdtKind Enumeration](../../debugger/debug-interface-access/udtkind.md) enumeration that specifies the kind of a UDT: structure, class, or union.

## Return Value
 If successful, returns `S_OK`; otherwise, returns `S_FALSE` or error code.

> [!NOTE]
> A return value of `S_FALSE` means the property is not available for the symbol.

## See also
- [IDiaSymbol](../../debugger/debug-interface-access/idiasymbol.md)
- [UdtKind Enumeration](../../debugger/debug-interface-access/udtkind.md)
