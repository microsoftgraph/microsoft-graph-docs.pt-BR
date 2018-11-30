---
title: tipo de recurso de skypeForBusinessOrganizerActivityCounts
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: 0729aef6367ebcb0a5edfaa461d80ffd8cb0775c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041160"
---
# <a name="skypeforbusinessorganizeractivitycounts-resource-type"></a>tipo de recurso de skypeForBusinessOrganizerActivityCounts

## <a name="properties"></a>Propriedades

| Propriedade           | Tipo   |
| :----------------- | :----- |
| mensagens instantâneas                 | Int64  |
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
