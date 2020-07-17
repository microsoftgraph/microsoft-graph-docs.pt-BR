---
title: tipo de recurso workbookOperation
description: Representa o status de operações de uma pasta de trabalho de execução longa.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: bd015045b01d0a7f886ecf0f5165a347d76dc061
ms.sourcegitcommit: b469176f49aacbd02cd06838cc7c8d36cf5bc768
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2020
ms.locfileid: "45165119"
---
# <a name="workbookoperation-resource-type"></a>tipo de recurso workbookOperation

Representa o status de uma operação de pasta de trabalho de execução longa.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Obter workbookOperation](../api/workbookoperation-get.md) | [workbookOperation](workbookoperation.md) | Recuperar o status de um objeto **workbookOperation** . |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|Cadeia de caracteres| A ID da operação. Somente leitura.|
|status|String| O status atual da operação. Os valores possíveis são: `notStarted`, `running`, `succeeded`, `failed`.|
|erro|[workbookOperationError](workbookoperationerror.md)| O erro retornado pela operação.|
|resourceLocation|Cadeia de caracteres| O URI do recurso para o resultado.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookOperation",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "status": {"@odata.type": "microsoft.graph.workbookOperationStatus"},
  "error": {"@odata.type": "microsoft.graph.workbookOperationError"},
  "resourceLocation": "String"
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
