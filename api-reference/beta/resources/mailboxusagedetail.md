---
title: Tipo de recurso mailboxUsageDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: sarahwxy
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 5b3eb643f74129d481b379d72515dbffaafd336c
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980756"
---
# <a name="mailboxusagedetail-resource-type"></a>Tipo de recurso mailboxUsageDetail

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade                        | Tipo    |
| :------------------------------ | :------ |
| reportRefreshDate               | Data    |
| userPrincipalName               | Cadeia de caracteres  |
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
| reportPeriod                    | Cadeia de caracteres  |

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


