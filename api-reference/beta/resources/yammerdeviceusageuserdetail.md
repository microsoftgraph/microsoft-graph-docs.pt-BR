---
title: tipo de recurso yammerDeviceUsageUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 982ebfc0de39bd956a4223e7bb0665ac73c42402
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518998"
---
# <a name="yammerdeviceusageuserdetail-resource-type"></a>tipo de recurso yammerDeviceUsageUserDetail

Namespace: Microsoft. Graph

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo    |
| :---------------- | :------ |
| reportRefreshDate | Data    |
| userPrincipalName | String  |
| displayName       | Cadeia de caracteres  |
| userState         | String  |
| stateChangeDate   | Data    |
| lastActivityDate  | Data    |
| usedWeb           | Boolean |
| usedWindowsPhone  | Boolean |
| usedAndroidPhone  | Boolean |
| usediPhone        | Boolean |
| usediPad          | Boolean |
| usedOthers        | Boolean |
| reportPeriod      | String  |

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
