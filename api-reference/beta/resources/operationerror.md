---
title: tipo de recurso operationError
description: Descreve erros no teamsAsyncOperation.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: billbliss
ms.openlocfilehash: 2419d4230e5618f601a5d8fe0743ec9ef807cf00
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809318"
---
# <a name="operationerror-resource-type"></a>tipo de recurso operationError

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
