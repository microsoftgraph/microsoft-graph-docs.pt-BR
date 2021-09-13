---
title: Tipo de recurso emailActivitySummary
description: Veja a seguir uma representação JSON do recurso.
ms.localizationpriority: medium
author: sarahwxy
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: ae2c1d52ab736106f9f76ef07b93b09db4de4d94
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59129296"
---
# <a name="emailactivitysummary-resource-type"></a>Tipo de recurso emailActivitySummary

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo   |
| :---------------- | :----- |
| reportRefreshDate | Data   |
| send              | Int64  |
| receive           | Int64  |
| leitura              | Int64  |
| reportDate        | Data   |
| reportPeriod      | Cadeia de Caracteres |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailActivitySummary"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "send": 1024, 
  "receive": 1024, 
  "read": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```


