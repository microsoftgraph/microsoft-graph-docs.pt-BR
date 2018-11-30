---
title: tipo de recurso de office365ActivationsUserCounts
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: 90d9d2d8616f166eb9d8b87967898daa0468db54
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039736"
---
# <a name="office365activationsusercounts-resource-type"></a>tipo de recurso de office365ActivationsUserCounts

## <a name="properties"></a>Propriedades

| Propriedade                 | Tipo   | Descrição                              |
| :----------------------- | :----- | ---------------------------------------- |
| reportRefreshDate        | Data   | A última data do conteúdo.          |
| productType              | String | O tipo de produto, como "Office 365 ProPlus", "Cliente do projeto," ou "Visio Pro para Office 365". |
| atribuído                 | Int64  | O número de usuários foram atribuído para a licença do produto. |
| ativado                | Int64  | O número de usuários que ativou o produto. |
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
