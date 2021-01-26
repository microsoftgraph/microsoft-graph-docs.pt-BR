---
title: Tipo de recurso yammerDeviceUsageUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: b7a6617b82c16fb297b684801e11876cf8178b0d
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982352"
---
# <a name="yammerdeviceusageuserdetail-resource-type"></a>Tipo de recurso yammerDeviceUsageUserDetail

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo    |
| :---------------- | :------ |
| reportRefreshDate | Data    |
| userPrincipalName | Cadeia de caracteres  |
| displayName       | Cadeia de caracteres  |
| userState         | Cadeia de caracteres  |
| stateChangeDate   | Data    |
| lastActivityDate  | Data    |
| usedWeb           | Booliano |
| usedWindowsPhone  | Booliano |
| usedAndroidPhone  | Booliano |
| usediPhone        | Booliano |
| usediPad          | Booliano |
| usedOthers        | Booliano |
| reportPeriod      | Cadeia de caracteres  |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerDeviceUsageUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "userState": "String", 
  "stateChangeDate": "Date", 
  "lastActivityDate": "Date", 
  "usedWeb": true, 
  "usedWindowsPhone": true, 
  "usedAndroidPhone": true, 
  "usediPhone": true, 
  "usediPad": true, 
  "usedOthers": true, 
  "reportPeriod": "String"
}
```


