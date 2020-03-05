---
title: tipo de recurso institutionData
description: tipo de recurso institutionData
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: a0734966d8a92aef5cd515043047bfcade35df47
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42495442"
---
# <a name="institutiondata-resource-type"></a>tipo de recurso institutionData

Namespace: Microsoft. Graph

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