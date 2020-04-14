---
title: tipo de recurso mailboxUsageQuotaStatusMailboxCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 1ebbfe0f134848d78e9c42a159c1c56bdbd21b39
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473422"
---
# <a name="mailboxusagequotastatusmailboxcounts-resource-type"></a>tipo de recurso mailboxUsageQuotaStatusMailboxCounts

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade              | Tipo   |
| :-------------------- | :----- |
| reportRefreshDate     | Data   |
| Limite máximo            | Int64  |
| warningIssued         | Int64  |
| sendProhibited        | Int64  |
| sendReceiveProhibited | Int64  |
| determinado         | Int64  |
| reportDate            | Data   |
| reportPeriod          | String |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailboxUsageQuotaStatusMailboxCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "underLimit": 1024, 
  "warningIssued": 1024, 
  "sendProhibited": 1024, 
  "sendReceiveProhibited": 1024, 
  "indeterminate": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
