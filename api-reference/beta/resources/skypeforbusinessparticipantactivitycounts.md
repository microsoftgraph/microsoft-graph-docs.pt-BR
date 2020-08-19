---
title: tipo de recurso skypeForBusinessParticipantActivityCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: 31e7e52de51647faa0748995452c67325c3da83f
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808547"
---
# <a name="skypeforbusinessparticipantactivitycounts-resource-type"></a>tipo de recurso skypeForBusinessParticipantActivityCounts

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
  "@odata.type": "microsoft.graph.skypeForBusinessParticipantActivityCounts"
} -->

```json
{
  "im": 1024,
  "audioVideo": 1024,
  "appSharing": 1024,
  "web": 1024,
  "dialInOut3rdParty": 1024,
  "reportRefreshDate": "Date",
  "reportDate": "Date",
  "reportPeriod": "String"
}
```
