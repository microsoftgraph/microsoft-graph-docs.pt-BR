---
title: tipo de recurso skypeForBusinessDeviceUsageUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 04f14ce10a93d8bff870613e644b80f554d26573
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008205"
---
# <a name="skypeforbusinessdeviceusageusercounts-resource-type"></a>tipo de recurso skypeForBusinessDeviceUsageUserCounts

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo   |
| :---------------- | :----- |
| reportRefreshDate | Data   |
| Windows           | Int64  |
| Windowsphonee      | Int64  |
| androidPhone      | Int64  |
| iPhone            | Int64  |
| iPad              | Int64  |
| reportDate        | Data   |
| reportPeriod      | String |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "windows": 1024, 
  "windowsPhone": 1024, 
  "androidPhone": 1024, 
  "iPhone": 1024, 
  "iPad": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
