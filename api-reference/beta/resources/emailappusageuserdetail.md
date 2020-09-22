---
title: tipo de recurso emailAppUsageUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 8365e856ee1b34b15b1aea3369b6cc22f99991e2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081675"
---
# <a name="emailappusageuserdetail-resource-type"></a>tipo de recurso emailAppUsageUserDetail

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo              |
| :---------------- | :---------------- |
| reportRefreshDate | Data              |
| userPrincipalName | Cadeia de caracteres            |
| displayName       | Cadeia de caracteres            |
| isDeleted         | Boolean           |
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


