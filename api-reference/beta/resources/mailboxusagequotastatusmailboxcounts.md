---
title: tipo de recurso mailboxUsageQuotaStatusMailboxCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: sarahwxy
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 2be392d12aea4dfe5dfd9a7ae21a78fe79bb2fdbb8b571633277ede95687190d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54195068"
---
# <a name="mailboxusagequotastatusmailboxcounts-resource-type"></a>tipo de recurso mailboxUsageQuotaStatusMailboxCounts

Namespace: microsoft.graph

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
| reportPeriod          | Cadeia de caracteres |

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


