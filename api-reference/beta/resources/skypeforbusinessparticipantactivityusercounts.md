---
title: Tipo de recurso skypeForBusinessParticipantActivityUserCounts
description: Veja a seguir uma representação JSON do recurso.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: 9f8d5cbfb67b4d4ad5b4203fc9c8bfeea8d9a917
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59053956"
---
# <a name="skypeforbusinessparticipantactivityusercounts-resource-type"></a>Tipo de recurso skypeForBusinessParticipantActivityUserCounts

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo   |
| :---------------- | :----- |
| im                | Int64  |
| audioVideo        | Int64  |
| appSharing        | Int64  |
| web               | Int64  |
| dialInOut3rdParty | Int64  |
| reportRefreshDate | Data   |
| reportDate        | Data   |
| reportPeriod      | Cadeia de Caracteres |

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


