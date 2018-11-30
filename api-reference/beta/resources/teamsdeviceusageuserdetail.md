---
title: tipo de recurso de teamsDeviceUsageUserDetail
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: 4eeec5f07a0a604249617ac87a62ea12b4052395
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040428"
---
# <a name="teamsdeviceusageuserdetail-resource-type"></a>tipo de recurso de teamsDeviceUsageUserDetail

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo    |
| :---------------- | :------ |
| reportRefreshDate | Data    |
| userPrincipalName | String  |
| lastActivityDate  | Data    |
| isDeleted         | Booliano |
| deletedDate       | Data    |
| usedWeb           | Booliano |
| usedWindowsPhone  | Booliano |
| usediOS           | Booliano |
| usedMac           | Booliano |
| usedAndroidPhone  | Booliano |
| usedWindows       | Booliano |
| reportPeriod      | String  |

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
