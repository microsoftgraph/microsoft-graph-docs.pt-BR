---
title: tipo de recurso skypeForBusinessPeerToPeerActivityMinuteCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: fda548f97a2aa3a2236d920a0f3439fb20710dc7
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810976"
---
# <a name="skypeforbusinesspeertopeeractivityminutecounts-resource-type"></a>tipo de recurso skypeForBusinessPeerToPeerActivityMinuteCounts

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo   |
| :---------------- | :----- |
| audio             | Int64  |
| video             | Int64  |
| reportRefreshDate | Data   |
| reportDate        | Data   |
| reportPeriod      | String |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityMinuteCounts"
} -->

```json
{
  "audio": 1024,
  "video": 1024,
  "reportRefreshDate": "Date",
  "reportDate": "Date",
  "reportPeriod": "String"
}
```
