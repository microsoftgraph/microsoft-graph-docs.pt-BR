---
title: tipo de recurso de operação
description: O status de uma operação de execução longa.
ms.localizationpriority: medium
author: billbliss
ms.prod: teamwork
doc_type: resourcePageType
ms.openlocfilehash: e43d86c5c53ce95855bdb0ccd42c3a43049073ca
ms.sourcegitcommit: 423e698a580c3b902f2816b0216ab9d5b91e6d20
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2022
ms.locfileid: "66034527"
---
# <a name="operation-resource-type"></a>tipo de recurso de operação

Namespace: microsoft.graph

O status de uma operação de execução longa.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|createdDateTime| DateTimeOffset |A hora de início da operação.|
|lastActionDateTime| DateTimeOffset |A hora da última ação da operação.|
|status|operationStatus|O status atual da operação: `notStarted`, , `running`, `completed``failed` |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.operation"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "lastActionDateTime": "String (timestamp)",
  "status": "notStarted | running | completed | failed"
}
```

<!-- uuid: 13fa92b1-3b41-498b-aab1-f943464a124f
2018-03-30 10:29:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

