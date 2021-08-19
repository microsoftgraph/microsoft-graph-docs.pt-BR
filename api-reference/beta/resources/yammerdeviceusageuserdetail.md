---
title: Tipo de recurso yammerDeviceUsageUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: e93dde1a1cdd034461a44766df6538da663093ed5d7f4674a3688d0e847aa9f4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54197769"
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
| usedWeb           | Boolean |
| usedWindowsPhone  | Boolean |
| usedAndroidPhone  | Boolean |
| usediPhone        | Boolean |
| usediPad          | Boolean |
| usedOthers        | Boolean |
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


