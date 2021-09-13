---
title: Tipo de recurso skypeForBusinessPeerToPeerActivityMinuteCounts
description: Veja a seguir uma representação JSON do recurso.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: f0565deb3d37c1caa5432d5f657980f562702560
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59053872"
---
# <a name="skypeforbusinesspeertopeeractivityminutecounts-resource-type"></a>Tipo de recurso skypeForBusinessPeerToPeerActivityMinuteCounts

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo   |
| :---------------- | :----- |
| audio             | Int64  |
| video             | Int64  |
| reportRefreshDate | Data   |
| reportDate        | Data   |
| reportPeriod      | Cadeia de Caracteres |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityMinuteCounts"
} -->

```json
{
  "audio": 1024,
  "video": 1024,
  "reportRefreshDate": "Date",
  "reportDate": "Date",
  "reportPeriod": "String"
}
```


