---
title: tipo de recurso emailAppUsageUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 700ef4b222860d19ef3ba78ae583a50e8cf8d0cc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42499481"
---
# <a name="emailappusageuserdetail-resource-type"></a>tipo de recurso emailAppUsageUserDetail

Namespace: Microsoft. Graph

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo              |
| :---------------- | :---------------- |
| reportRefreshDate | Data              |
| userPrincipalName | String            |
| displayName       | Cadeia de caracteres            |
| isDeleted         | Boolean           |
| deletedDate       | Data              |
| lastActivityDate  | Data              |
| mailForMac        | String collection |
| outlookForMac     | String collection |
| outlookForWindows | String collection |
| outlookForMobile  | String collection |
| otherForMobile    | String collection |
| outlookForWeb     | String collection |
| pop3App           | String collection |
| imap4App          | String collection |
| smtpApp           | String collection |
| reportPeriod      | String            |

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
