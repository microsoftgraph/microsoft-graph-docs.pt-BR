---
title: Tipo de recurso yammerDeviceUsageUserDetail
description: Veja a seguir uma representação JSON do recurso.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 4a3232f87775f4e08e5296c21282e80ee2f1ee88
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59128484"
---
# <a name="yammerdeviceusageuserdetail-resource-type"></a>Tipo de recurso yammerDeviceUsageUserDetail

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo    |
| :---------------- | :------ |
| reportRefreshDate | Data    |
| userPrincipalName | Cadeia de caracteres  |
| displayName       | Cadeia de caracteres  |
| userState         | Cadeia de Caracteres  |
| stateChangeDate   | Data    |
| lastActivityDate  | Data    |
| usedWeb           | Boleano |
| usedWindowsPhone  | Boleano |
| usedAndroidPhone  | Boleano |
| usediPhone        | Boleano |
| usediPad          | Boleano |
| usedOthers        | Boleano |
| reportPeriod      | Cadeia de Caracteres  |

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


