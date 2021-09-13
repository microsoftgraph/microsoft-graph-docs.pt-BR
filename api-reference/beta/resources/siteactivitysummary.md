---
title: Tipo de recurso siteActivitySummary
description: Veja a seguir uma representação JSON do recurso.
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: d008e263640c42d4531404f69e659124333c58a8
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59033214"
---
# <a name="siteactivitysummary-resource-type"></a>Tipo de recurso siteActivitySummary

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo   |
| :---------------- | :----- |
| reportRefreshDate | Data   |
| viewedOrEdited    | Int64  |
| sincronizado            | Int64  |
| sharedInternally  | Int64  |
| sharedExternally  | Int64  |
| reportDate        | Data   |
| reportPeriod      | Cadeia de Caracteres |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.siteActivitySummary"
} -->

```json
{
  "reportRefreshDate": "Date",
  "viewedOrEdited": 1024,
  "synced": 1024,
  "sharedInternally": 1024,
  "sharedExternally": 1024,
  "reportDate": "Date",
  "reportPeriod": "String"
}
```


