---
title: tipo de recurso office365ActivationsUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: b8746d58b03b15a3118e8fc51a42e61e3c22cb78
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896802"
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
