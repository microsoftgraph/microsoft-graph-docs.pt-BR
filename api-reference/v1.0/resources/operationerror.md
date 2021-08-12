---
title: Tipo de recurso operationError
description: Descreve erros no teamsAsyncOperation.
localization_priority: Normal
author: billbliss
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 395b10dbfd3617cfe891854897c9d99be64ad4b76bc05776b4eab77d1847a44f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54223267"
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

