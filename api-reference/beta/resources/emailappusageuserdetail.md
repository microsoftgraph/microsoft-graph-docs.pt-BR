---
title: Tipo de recurso emailAppUsageUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: sarahwxy
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: fb6dded6e7c86644191f1d941900050813b84594
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981813"
---
# <a name="emailappusageuserdetail-resource-type"></a>Tipo de recurso emailAppUsageUserDetail

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo              |
| :---------------- | :---------------- |
| reportRefreshDate | Data              |
| userPrincipalName | Cadeia de caracteres            |
| displayName       | Cadeia de caracteres            |
| isDeleted         | Booliano           |
| deletedDate       | Data              |
| lastActivityDate  | Data              |
| mailForMac        | Coleção String |
| outlookForMac     | Coleção String |
| outlookForWindows | Coleção String |
| outlookForMobile  | Coleção String |
| otherForMobile    | Coleção String |
| outlookForWeb     | Coleção String |
| pop3App           | Coleção String |
| imap4App          | Coleção String |
| smtpApp           | Coleção String |
| reportPeriod      | Cadeia de caracteres            |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailAppUsageUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "lastActivityDate": "Date", 
  "mailForMac": ["String"], 
  "outlookForMac": ["String"], 
  "outlookForWindows": ["String"], 
  "outlookForMobile": ["String"], 
  "otherForMobile": ["String"], 
  "outlookForWeb": ["String"], 
  "pop3App": ["String"], 
  "imap4App": ["String"], 
  "smtpApp": ["String"], 
  "reportPeriod": "String"
}
```


