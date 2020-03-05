---
title: tipo de recurso teamsDeviceUsageUserCounts
description: Veja a seguir uma representação JSON do recurso.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 02dc1b734e039e7c5eac7b8ffaed7a418e443c71
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519866"
---
# <a name="teamsdeviceusageusercounts-resource-type"></a>tipo de recurso teamsDeviceUsageUserCounts

Namespace: Microsoft. Graph

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo   |
| :---------------- | :----- |
| reportRefreshDate | Data   |
| web               | Int64  |
| Windowsphonee      | Int64  |
| androidPhone      | Int64  |
| emiti               | Int64  |
| mac               | Int64  |
| Windows           | Int64  |
| reportDate        | Data   |
| reportPeriod      | String |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "web": 1024, 
  "windowsPhone": 1024, 
  "androidPhone": 1024, 
  "ios": 1024, 
  "mac": 1024, 
  "windows": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
