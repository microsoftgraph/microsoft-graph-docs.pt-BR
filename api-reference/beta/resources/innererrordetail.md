---
title: tipo de recurso innerErrorDetail
description: Um erro interno contido em um objeto errorDetail.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 5a5b85f17b87343766a4edb00c6d620c185ecaf5
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939653"
---
# <a name="innererrordetail-resource-type"></a>tipo de recurso innerErrorDetail

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um erro interno contido em um objeto [errorDetail](errordetail.md) .

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
