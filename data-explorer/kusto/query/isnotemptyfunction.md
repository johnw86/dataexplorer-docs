---
title: isnotempty() - Azure Data Explorer
description: This article describes isnotempty() in Azure Data Explorer.
ms.reviewer: alexans
ms.topic: reference
ms.date: 02/13/2020
---
# isnotempty()

Returns `true` if the argument isn't an empty string, and it isn't null.

```kusto
isnotempty("") == false
```

> **Depricated aliases:** notempty()

## Syntax

`isnotempty(`[*value*]`)`

## Example

```kusto
T
| where isnotempty(fieldName)
| count
```
