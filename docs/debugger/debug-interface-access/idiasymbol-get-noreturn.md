---
description: "Retrieves a flag that specifies whether the function has been marked as never returning with the noreturn) attribute."
title: "IDiaSymbol::get_noReturn"
ms.date: "11/04/2016"
ms.topic: "reference"
dev_langs:
  - "C++"
helpviewer_keywords:
  - "IDiaSymbol::get_noReturn method"
author: "mikejo5000"
ms.author: "mikejo"
manager: jmartens
ms.subservice: debug-diagnostics
---
# IDiaSymbol::get_noReturn

Retrieves a flag that specifies whether the function has been marked as never returning with the [noreturn](/cpp/cpp/noreturn) attribute.

## Syntax

```C++
HRESULT get_noReturn(
   BOOL *pFlag
);
```

#### Parameters
 pFlag

[out] Returns `TRUE` if the function has been declared as never returning with the `noreturn` attribute; otherwise, returns `FALSE`.

## Return Value
 If successful, returns `S_OK`; otherwise, returns `S_FALSE` or an error code.

> [!NOTE]
> A return value of `S_FALSE` means the property is not available for the symbol.

## Requirements

|Requirement|Description|
|-----------------|-----------------|
|Header:|dia2.h|
|Version:|DIA SDK v8.0|

## See also
- [IDiaSymbol](../../debugger/debug-interface-access/idiasymbol.md)
- [noreturn](/cpp/cpp/noreturn)
