---
title: tipo de recurso emailAppUsageUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: ae0409124569f4318df94f97729402a91d4b8e45
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972142"
---
# <a name="emailappusageuserdetail-resource-type"></a>tipo de recurso emailAppUsageUserDetail

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo              |
| :---------------- | :---------------- |
| reportRefreshDate | Data              |
| userPrincipalName | String            |
| displayName       | String            |
| isDeleted         | Booliano           |
| deletedDate       | Data              |
| lastActivityDate  | Data              |
| mailForMac        | Coleção de cadeias de caracteres |
| outlookForMac     | Coleção de cadeias de caracteres |
| outlookForWindows | Coleção de cadeias de caracteres |
| outlookForMobile  | Coleção de cadeias de caracteres |
| otherForMobile    | Coleção de cadeias de caracteres |
| outlookForWeb     | Coleção de cadeias de caracteres |
| pop3App           | Coleção de cadeias de caracteres |
| imap4App          | Coleção de cadeias de caracteres |
| smtpApp           | Coleção de cadeias de caracteres |
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
