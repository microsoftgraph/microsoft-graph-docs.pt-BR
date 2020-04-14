---
title: tipo de recurso mailboxUsageDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 485dba38275cb437f069abf1309bdc0705ad967a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473476"
---
# <a name="mailboxusagedetail-resource-type"></a>tipo de recurso mailboxUsageDetail

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade                        | Tipo    |
| :------------------------------ | :------ |
| reportRefreshDate               | Data    |
| userPrincipalName               | String  |
| displayName                     | Cadeia de caracteres  |
| isDeleted                       | Booliano |
| deletedDate                     | Data    |
| createdDate                     | Data    |
| lastActivityDate                | Data    |
| itemCount                       | Int64   |
| storageUsedInBytes              | Int64   |
| deletedItemCount                | Int64   |
| deletedItemSizeInBytes          | Int64   |
| issueWarningQuotaInBytes        | Int64   |
| prohibitSendQuotaInBytes        | Int64   |
| prohibitSendReceiveQuotaInBytes | Int64   |
| reportPeriod                    | String  |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailboxUsageDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "createdDate": "Date", 
  "lastActivityDate": "Date", 
  "itemCount": 1024, 
  "storageUsedInBytes": 1024, 
  "deletedItemCount": 1024,
  "deletedItemSizeInBytes": 1024, 
  "issueWarningQuotaInBytes": 1024, 
  "prohibitSendQuotaInBytes": 1024, 
  "prohibitSendReceiveQuotaInBytes": 1024, 
  "reportPeriod": "String"
}
```
