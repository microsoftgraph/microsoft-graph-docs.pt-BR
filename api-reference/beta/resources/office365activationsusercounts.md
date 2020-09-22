---
title: tipo de recurso office365ActivationsUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 21e18b35dc4e4ff639087617d679ae1583516026
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021221"
---
# <a name="office365activationsusercounts-resource-type"></a>tipo de recurso office365ActivationsUserCounts

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade                 | Tipo   | Descrição                              |
| :----------------------- | :----- | ---------------------------------------- |
| reportRefreshDate        | Data   | A última data do conteúdo.          |
| ProductType              | String | O tipo de produto como "Microsoft 365 ProPlus" ou "Project Client". |
| atribuí                 | Int64  | O número de usuários foi atribuído para a licença de produto. |
| ativado                | Int64  | O número de usuários que ativaram o produto. |
| sharedComputerActivation | Int64  | O número de usuários que usaram o produto em um computador compartilhado. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActivationsUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "productType": "String", 
  "assigned": 1024, 
  "activated": 1024,
  "sharedComputerActivation": 1024
}
```


