---
title: tipo de recurso de office365ActivationsUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: f57393a538631664be8845fdaeda9f35d07c986f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849305"
---
# <a name="office365activationsusercounts-resource-type"></a>tipo de recurso de office365ActivationsUserCounts

## <a name="properties"></a>Propriedades

| Propriedade                 | Tipo   | Descrição                              |
| :----------------------- | :----- | ---------------------------------------- |
| reportRefreshDate        | Data   | A última data do conteúdo.          |
| productType              | Cadeia de caracteres | O tipo de produto, como "Office 365 ProPlus", "Cliente do projeto," ou "Visio Pro para Office 365". |
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
