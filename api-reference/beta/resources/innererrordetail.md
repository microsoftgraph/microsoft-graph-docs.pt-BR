---
title: tipo de recurso innerErrorDetail
description: Um erro interno contido em um objeto errorDetail.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 6b3dfb2ec4caf8ae2b8ec9a279a6d001ad3aaae7
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703774"
---
# <a name="innererrordetail-resource-type"></a>tipo de recurso innerErrorDetail

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um erro interno contido em um objeto [errorDetail](errordetail.md) .

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a>Propriedades

| Propriedade | Tipo   | Descrição                                  |
|:---------|:-------|:---------------------------------------------|
| mensagem  | String | A mensagem de erro legível por pessoas. Somente leitura. |
| source   | String | A origem do erro. Somente leitura.          |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.innerErrorDetail",
  "baseType": null
}-->

```json
{
  "message": "String",
  "source": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "innerErrorDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
