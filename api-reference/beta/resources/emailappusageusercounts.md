---
title: tipo de recurso de emailAppUsageUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: a018776f092e9b7f378e8069666d015e1cd3e4a0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835445"
---
# <a name="emailappusageusercounts-resource-type"></a>tipo de recurso de emailAppUsageUserCounts

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo   |
| :---------------- | :----- |
| reportRefreshDate | Data   |
| mailForMac        | Int64  |
| outlookForMac     | Int64  |
| outlookForWindows | Int64  |
| outlookForMobile  | Int64  |
| otherForMobile    | Int64  |
| outlookForWeb     | Int64  |
| pop3App           | Int64  |
| imap4App          | Int64  |
| smtpApp           | Int64  |
| reportDate        | Data   |
| reportPeriod      | Cadeia de caracteres |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailAppUsageUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "mailForMac": 1024, 
  "outlookForMac": 1024, 
  "outlookForWindows": 1024, 
  "outlookForMobile": 1024, 
  "otherForMobile": 1024, 
  "outlookForWeb": 1024, 
  "pop3App": 1024, 
  "imap4App": 1024, 
  "smtpApp": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
