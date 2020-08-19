---
title: tipo de recurso skypeForBusinessDeviceUsageUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: 50f37fdfd3441c256241b76ebcc6b144eb1486d7
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811045"
---
# <a name="skypeforbusinessdeviceusageuserdetail-resource-type"></a>tipo de recurso skypeForBusinessDeviceUsageUserDetail

Namespace: microsoft.graph

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
