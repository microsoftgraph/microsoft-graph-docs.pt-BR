---
title: Tipo de recurso operationError
description: Descreve erros no teamsAsyncOperation.
ms.localizationpriority: medium
author: billbliss
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: b30a945dcbd19a6c1be0c276eec0b650b8251ea1
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59098507"
---
# <a name="operationerror-resource-type"></a>Tipo de recurso operationError

Namespace: microsoft.graph



Descreve erros em [teamsAsyncOperation](teamsasyncoperation.md).

## <a name="operationerror-properties"></a>propriedades operationError
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

