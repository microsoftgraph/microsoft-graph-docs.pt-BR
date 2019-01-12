---
title: tipo de recurso de emailAppUsageUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 1ebc99f25bf0b16343f48686496c1dbd7d329e65
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977651"
---
# <a name="emailappusageuserdetail-resource-type"></a>tipo de recurso de emailAppUsageUserDetail

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo              |
| :---------------- | :---------------- |
| reportRefreshDate | Data              |
| userPrincipalName | Cadeia de caracteres            |
| displayName       | Cadeia de caracteres            |
| isDeleted         | Booliano           |
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
