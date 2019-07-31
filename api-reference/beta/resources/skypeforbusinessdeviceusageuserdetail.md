---
title: tipo de recurso skypeForBusinessDeviceUsageUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: b84cf9c7654354446fb7c6a5005befe3d17a0fa4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964911"
---
# <a name="skypeforbusinessdeviceusageuserdetail-resource-type"></a>tipo de recurso skypeForBusinessDeviceUsageUserDetail

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo    |
| :---------------- | :------ |
| reportRefreshDate | Data    |
| userPrincipalName | String  |
| lastActivityDate  | Data    |
| usedWindows       | Booliano |
| usedWindowsPhone  | Booliano |
| usedAndroidPhone  | Booliano |
| usediPhone        | Booliano |
| usediPad          | Booliano |
| reportPeriod      | String  |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "usedWindows": true, 
  "usedWindowsPhone": true, 
  "usedAndroidPhone": true, 
  "usediPhone": true, 
  "usediPad": true, 
  "reportPeriod": "String"
}
```
