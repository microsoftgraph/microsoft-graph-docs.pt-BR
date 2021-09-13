---
title: Tipo de recurso skypeForBusinessDeviceUsageUserCounts
description: Veja a seguir uma representação JSON do recurso.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: 4e60915b25082c1b37fb7f173916e18417f44747
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59023154"
---
# <a name="skypeforbusinessdeviceusageusercounts-resource-type"></a>Tipo de recurso skypeForBusinessDeviceUsageUserCounts

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo   |
| :---------------- | :----- |
| reportRefreshDate | Data   |
| windows           | Int64  |
| windowsPhone      | Int64  |
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


