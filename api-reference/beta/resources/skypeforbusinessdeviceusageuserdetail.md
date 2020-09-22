---
title: tipo de recurso skypeForBusinessDeviceUsageUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: 36cd6aba954206b60317520534284cd17f8d42e8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997526"
---
# <a name="skypeforbusinessdeviceusageuserdetail-resource-type"></a>tipo de recurso skypeForBusinessDeviceUsageUserDetail

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo    |
| :---------------- | :------ |
| reportRefreshDate | Data    |
| userPrincipalName | String  |
| lastActivityDate  | Data    |
| usedWindows       | Boolean |
| usedWindowsPhone  | Boolean |
| usedAndroidPhone  | Boolean |
| usediPhone        | Boolean |
| usediPad          | Boolean |
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


