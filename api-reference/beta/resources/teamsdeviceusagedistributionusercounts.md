---
title: tipo de recurso teamsDeviceUsageDistributionUserCounts
description: Veja a seguir uma representação JSON do recurso.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 1842d2edc9e527d577b6a44e61443018f8309c17
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007610"
---
# <a name="teamsdeviceusagedistributionusercounts-resource-type"></a>tipo de recurso teamsDeviceUsageDistributionUserCounts

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
| reportPeriod      | String |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageDistributionUserCounts"
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
  "reportPeriod": "String"
}
```
