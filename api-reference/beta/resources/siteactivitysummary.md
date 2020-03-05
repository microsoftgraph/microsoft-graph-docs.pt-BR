---
title: tipo de recurso siteActivitySummary
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: 0e24da683b2abe319a60e5a51144a96f9ec00135
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520545"
---
# <a name="siteactivitysummary-resource-type"></a>tipo de recurso siteActivitySummary

Namespace: Microsoft. Graph

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo   |
| :---------------- | :----- |
| reportRefreshDate | Data   |
| viewedOrEdited    | Int64  |
| sincronizados            | Int64  |
| sharedInternally  | Int64  |
| sharedExternally  | Int64  |
| reportDate        | Data   |
| reportPeriod      | String |

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
