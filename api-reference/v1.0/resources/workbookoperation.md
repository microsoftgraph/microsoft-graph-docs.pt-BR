---
title: tipo de recurso workbookOperation
description: Representa o status de operações de uma longa execução de uma livro de trabalho.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: c674186befbb6a24c41cd8741f554876a17a4394
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158944"
---
# <a name="workbookoperation-resource-type"></a>tipo de recurso workbookOperation

Representa o status de uma operação de livro de trabalho de execução longa.


## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Obter workbookOperation](../api/workbookoperation-get.md) | [workbookOperation](workbookoperation.md) | Obter a operação com `{operation-id}` . |


## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|status|Cadeia de caracteres| O status atual da operação. Os valores possíveis são: `NotStarted`, `Running`, `Completed`, `Failed`.|
|id|Cadeia de caracteres| A ID da operação. Somente leitura.|
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
  "resourceLocation": "String",
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
