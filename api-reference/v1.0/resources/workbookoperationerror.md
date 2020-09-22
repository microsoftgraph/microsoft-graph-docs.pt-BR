---
title: tipo de recurso workbookOperationError
description: Representa um erro de uma operação de pasta de trabalho com falha.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: ce65847d6ddbb0a8db0c1277e38753ecab7080e9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015138"
---
# <a name="workbookoperationerror-resource-type"></a>tipo de recurso workbookOperationError

Representa um erro de uma operação de pasta de trabalho com falha.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|código|String| O código de erro.|
|mensagem|String| A mensagem de erro.|
|innererror|error object| Opcional. Objetos error adicionais que podem ser mais específicos do que o erro de nível superior.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookOperationError",
  "baseType": null
}-->

```json
{
  "code": "String",
  "message": "String",
  "innererror": { "@odata.type": "odata.error" }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workbookOperationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

