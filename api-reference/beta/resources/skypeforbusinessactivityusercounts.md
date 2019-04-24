---
title: tipo de recurso skypeForBusinessActivityUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: e98133611d669a2a85bae65195fe70571d290442
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32521975"
---
# <a name="skypeforbusinessactivityusercounts-resource-type"></a>tipo de recurso skypeForBusinessActivityUserCounts

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo   |
| :---------------- | :----- |
| peerToPeer        | Int64  |
| organiza         | Int64  |
| participaram      | Int64  |
| reportRefreshDate | Data   |
| reportDate        | Data   |
| reportPeriod      | String |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessActivityUserCounts"
} -->

```json
{
  "peerToPeer": 1024, 
  "organized": 1024, 
  "participated": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
