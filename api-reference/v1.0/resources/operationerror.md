---
title: tipo de recurso operationError
description: Descreve erros no teamsAsyncOperation.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 0cf550b0c15d5bd6632490d40eae04c0b4f5f3f1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447280"
---
# <a name="operationerror-resource-type"></a>tipo de recurso operationError

Namespace: Microsoft. Graph



Descreve erros no [teamsAsyncOperation](teamsasyncoperation.md).

## <a name="operationerror-properties"></a>Propriedades operationError
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|código|cadeia de caracteres (somente leitura)|Código de erro de operação.|
|message|cadeia de caracteres (somente leitura)|Mensagem de erro de operação.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.operationError"
}-->

```json
{
    "code": "TeamUnavailable",
    "message": "The team was not found."
}
```

<!-- uuid: 069fadaa-52db-4ced-85d5-74f7caa2c66f
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "operation error resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
