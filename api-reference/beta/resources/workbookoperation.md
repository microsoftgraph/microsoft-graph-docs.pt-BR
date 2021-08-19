---
title: tipo de recurso workbookOperation
description: Representa o status de operações de uma área de trabalho de longa duração.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 373183806b6c23e494aeb8a76f0b156ac5cac62ac064b7f78f66c9650968df4b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54200261"
---
# <a name="workbookoperation-resource-type"></a>tipo de recurso workbookOperation

Representa o status de uma operação de manual de trabalho de longa duração.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Obter workbookOperation](../api/workbookoperation-get.md) | [workbookOperation](workbookoperation.md) | Recupere o status de um **objeto workbookOperation.** |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|Cadeia de caracteres| A id da operação. Somente leitura.|
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

  ],
  "@odata.type": "microsoft.graph.workbookOperation",
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


