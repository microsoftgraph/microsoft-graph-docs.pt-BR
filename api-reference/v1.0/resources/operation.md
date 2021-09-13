---
title: tipo de recurso operation
description: O status de uma operação de longa duração.
ms.localizationpriority: medium
author: billbliss
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 58473fcdfdd98a269299aba495cd1bd397423a6d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59098521"
---
# <a name="operation-resource-type"></a>tipo de recurso operation

Namespace: microsoft.graph

O status de uma operação de longa duração.

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
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|createdDateTime| DateTimeOffset |A hora de início da operação.|
|lastActionDateTime| DateTimeOffset |A hora da última ação da operação.|
|status|operationStatus|O status atual da operação: `notStarted` , `running` , `completed` , `failed` |

<!-- uuid: 13fa92b1-3b41-498b-aab1-f943464a124f
2018-03-30 10:29:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

