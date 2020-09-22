---
title: tipo de recurso skypeForBusinessOrganizerActivityCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: aa0721c13d78be8b88e399b1342d8f0c0ecd3efa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997513"
---
# <a name="skypeforbusinessorganizeractivitycounts-resource-type"></a>tipo de recurso skypeForBusinessOrganizerActivityCounts

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade           | Tipo   |
| :----------------- | :----- |
| respectiva                 | Int64  |
| audioVideo         | Int64  |
| appSharing         | Int64  |
| web                | Int64  |
| dialInOut3rdParty  | Int64  |
| dialInOutMicrosoft | Int64  |
| reportRefreshDate  | Data   |
| reportDate         | Data   |
| reportPeriod       | String |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessOrganizerActivityCounts"
} -->

```json
{
  "im": 1024,
  "audioVideo": 1024,
  "appSharing": 1024,
  "web": 1024,
  "dialInOut3rdParty": 1024,
  "dialInOutMicrosoft": 1024,
  "reportRefreshDate": "Date",
  "reportDate": "Date",
  "reportPeriod": "String"
}
```


