---
title: tipo de recurso workbookOperation
description: Representa o status de operações de uma área de trabalho de longa duração.
ms.localizationpriority: medium
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 1077cb078720ea76c13c5dc5ea7e3b353ad8860c
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59767465"
---
# <a name="workbookoperation-resource-type"></a>tipo de recurso workbookOperation

Representa o status de uma operação de manual de trabalho de longa duração.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Obter workbookOperation](../api/workbookoperation-get.md) | coleção [workbookOperation](workbookoperation.md) | Recupere o status de um **objeto workbookOperation.** |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String| A id da operação. Somente leitura.|
|status|Cadeia de caracteres| O status atual da operação. Os valores possíveis são: `notStarted`, `running`, `succeeded`, `failed`.|
|erro|[workbookOperationError](workbookoperationerror.md)| O erro retornado pela operação.|
|resourceLocation|Cadeia de caracteres| O URI do recurso para o resultado.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "id", "status", "error", "resourceLocation"
  ],
  "@odata.type": "microsoft.graph.workbookOperation",
  "keyProperty": "id"
}-->

```json
{
  "@odata.type": "#microsoft.graph.workbookOperation",
  "id": "String (identifier)",
  "status": "String",
  "resourceLocation": "String",
  "statusCode": "Integer",
  "error": {
    "@odata.type": "microsoft.graph.workbookOperationError"
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workbookOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


