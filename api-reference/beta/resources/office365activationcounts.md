---
title: tipo de recurso de office365ActivationCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: 30386b3833b8140d4c602e27cb3a78f3a68670dc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824987"
---
# <a name="office365activationcounts-resource-type"></a>tipo de recurso de office365ActivationCounts

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo   | Descrição                              |
| :---------------- | :----- | ---------------------------------------- |
| reportRefreshDate | Data   | A última data do conteúdo.          |
| productType       | Cadeia de caracteres | O tipo de produto, como "Office 365 ProPlus", "Cliente do projeto," ou "Visio Pro para Office 365". |
| Windows           | Int64  | A contagem de ativação do Windows. Esse número inclui cada ativação em qualquer computador do Windows. |
| mac               | Int64  | A contagem de ativação no Mac OS.          |
| Android           | Int64  | A contagem de ativação em um dispositivo Android.  |
| IOS               | Int64  | A contagem de ativação no iOS.             |
| windows10Mobile   | Int64  | A ativação contar com 10 do Windows mobile. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActivationCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "productType": "String", 
  "windows": 1024, 
  "mac": 1024, 
  "android": 1024, 
  "ios": 1024, 
  "windows10Mobile": 1024
}
```
