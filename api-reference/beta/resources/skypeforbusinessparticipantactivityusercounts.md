---
title: tipo de recurso skypeForBusinessParticipantActivityUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: e53ef85ce3fbe0be2a36adc218d565bdb78f64a0
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811067"
---
# <a name="skypeforbusinessparticipantactivityusercounts-resource-type"></a>tipo de recurso skypeForBusinessParticipantActivityUserCounts

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo   |
| :---------------- | :----- |
| respectiva                | Int64  |
| audioVideo        | Int64  |
| appSharing        | Int64  |
| web               | Int64  |
| dialInOut3rdParty | Int64  |
| reportRefreshDate | Data   |
| reportDate        | Data   |
| reportPeriod      | String |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessParticipantActivityUserCounts"
} -->

```json
{
  "im": 1024,
  "audioVideo": 196,
  "appSharing": 196,
  "web": 196,
  "dialInOut3rdParty": 196,
  "reportRefreshDate": "Date",
  "reportDate": "Date",
  "reportPeriod": "String"
}
```
