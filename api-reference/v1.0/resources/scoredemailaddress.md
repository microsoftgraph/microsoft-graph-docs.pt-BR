---
title: tipo de recurso scoredEmailAddress
description: Representa um endereço de email pontuado.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: b8cdcd7a0192bdd97bc096ce06514e75a7184f63
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034591"
---
# <a name="scoredemailaddress-resource-type"></a>tipo de recurso scoredEmailAddress

Representa um endereço de email pontuado.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|address|cadeia de caracteres|O endereço de email.|
|relevanceScore|double|A pontuação de relevância do endereço de email. Uma pontuação de relevância é usada como uma chave de classificação em relação aos outros resultados retornados. Um valor mais alto de pontuação de relevância corresponde a um resultado mais relevante. A relevância é determinada pelos padrões de comunicação e colaboração e pelas relações comerciais do usuário. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scoredEmailAddress"
}-->

```json
{
  "address": "string",
  "relevanceScore": 1024.0
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "scoredEmailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
