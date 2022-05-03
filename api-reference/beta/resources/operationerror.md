---
title: Tipo de recurso operationError
description: Descreve erros em teamsAsyncOperation.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: teamwork
author: billbliss
ms.openlocfilehash: 3634e55dca6328b40a9d21577183e8a5616c53f8
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176510"
---
# <a name="operationerror-resource-type"></a>Tipo de recurso operationError

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descreve erros em [teamsAsyncOperation](teamsasyncoperation.md).

## <a name="operationerror-properties"></a>Propriedades operationError
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|código|cadeia de caracteres (somente leitura)|Código de erro da operação.|
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
<!--
{
  "type": "#page.annotation",
  "description": "operation error resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


