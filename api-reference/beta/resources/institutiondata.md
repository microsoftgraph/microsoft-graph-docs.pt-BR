---
title: tipo de recurso institutionData
description: tipo de recurso institutionData
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 5724f56a5e68c059126eaac910d34999dcded632
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939450"
---
# <a name="institutiondata-resource-type"></a>tipo de recurso institutionData

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa detalhes adicionais sobre um Undergraduate, graduação, graduação ou outras atividades educacionais que um usuário fez e é usado em um recurso do [educationalActivity](educationalActivity.md) .

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo                                 | Descrição                                              |
|:-------------|:-------------------------------------|:---------------------------------------------------------|
|description   |String                                |Descrição resumida da instituição em que o usuário estudou. |
|displayName   |Cadeia de caracteres                                |Nome da instituição em que o usuário estudou.              |
|location      |[physicalAddress](physicaladdress.md) |Endereço ou local da instituição.                     |
|webUrl        |String                                |Link para a instituição ou a home page do departamento.           |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.institutionData",
  "baseType": null
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "location": {"@odata.type": "microsoft.graph.physicalAddress"},
  "webUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "institutionData resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->