---
title: tipo de recurso teamsDeviceUsageUserDetail
description: Veja a seguir uma representação JSON do recurso.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ddfdef3e9d5500951fc24de5beb333e822c9bbda
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046451"
---
# <a name="teamsdeviceusageuserdetail-resource-type"></a>tipo de recurso teamsDeviceUsageUserDetail

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo    |
| :---------------- | :------ |
| reportRefreshDate | Data    |
| userPrincipalName | Cadeia de caracteres  |
| lastActivityDate  | Data    |
| isDeleted         | Booliano |
| deletedDate       | Data    |
| usedWeb           | Booliano |
| usedWindowsPhone  | Booliano |
| usediOS           | Booliano |
| usedMac           | Booliano |
| usedAndroidPhone  | Booliano |
| usedWindows       | Booliano |
| reportPeriod      | Cadeia de caracteres  |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "usedWeb": true, 
  "usedWindowsPhone": true, 
  "usediOS": true, 
  "usedMac": true, 
  "usedAndroidPhone": true, 
  "usedWindows": true, 
  "reportPeriod": "String"
}
```


