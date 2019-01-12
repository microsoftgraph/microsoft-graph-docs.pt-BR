---
title: tipo de recurso de teamsDeviceUsageUserDetail
description: Veja a seguir uma representação JSON do recurso.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8cdd2fe1a212bb1d36846b80fc1b558c576deb47
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953782"
---
# <a name="teamsdeviceusageuserdetail-resource-type"></a>tipo de recurso de teamsDeviceUsageUserDetail

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
