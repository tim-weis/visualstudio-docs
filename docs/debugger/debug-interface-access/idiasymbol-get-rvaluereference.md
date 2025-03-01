---
description: "Retrieves a flag that specifies whether a pointer type is an rvalue reference."
title: "IDiaSymbol::get_RValueReference"
ms.date: "11/04/2016"
ms.topic: "reference"
dev_langs:
  - "C++"
helpviewer_keywords:
  - "IDiaSymbol::get_RValueReference method"
author: "mikejo5000"
ms.author: "mikejo"
manager: jmartens
ms.subservice: debug-diagnostics
---
# IDiaSymbol::get_RValueReference

Retrieves a flag that specifies whether a pointer type is an rvalue reference. Use when the [SymTagEnum Enumeration](../../debugger/debug-interface-access/symtagenum.md) is set to a pointer type.

## Syntax

```C++
HRESULT get_RValueReference (
   BOOL* pRetVal
);
```

#### Parameters
 `pRetVal`

[out] Returns `TRUE` if the pointer is an rvalue reference; otherwise, returns `FALSE`.

## Return Value
 If successful, returns `S_OK`; otherwise, returns `S_FALSE` or an error code.

> [!NOTE]
> A return value of `S_FALSE` means the property is not available for the symbol.

## Remarks

## Requirements
 Header: Dia2.h

 Library: diaguids.lib

 DLL: msdia100.dll

## See also
- [IDiaSymbol](../../debugger/debug-interface-access/idiasymbol.md)
