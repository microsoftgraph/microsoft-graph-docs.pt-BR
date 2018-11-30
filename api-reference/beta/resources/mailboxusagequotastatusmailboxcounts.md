---
title: tipo de recurso de mailboxUsageQuotaStatusMailboxCounts
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: ac6c597cad9d28f985da97d6f55a5726ebbf491e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036038"
---
# <a name="mailboxusagequotastatusmailboxcounts-resource-type"></a>tipo de recurso de mailboxUsageQuotaStatusMailboxCounts

## <a name="properties"></a>Propriedades

| Propriedade              | Tipo   |
| :-------------------- | :----- |
| reportRefreshDate     | Data   |
| underLimit            | Int64  |
| warningIssued         | Int64  |
| sendProhibited        | Int64  |
| sendReceiveProhibited | Int64  |
| indeterminado         | Int64  |
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
