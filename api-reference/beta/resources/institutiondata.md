---
title: tipo de recurso institutionData
description: tipo de recurso institutionData
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: a528bf5bc8800b10deed2c45d84613b5ab4bd6b2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47986060"
---
# <a name="institutiondata-resource-type"></a>tipo de recurso institutionData

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa detalhes adicionais sobre um Undergraduate, graduação, graduação ou outras atividades educacionais que um usuário fez e é usado em um recurso do [educationalActivity](educationalActivity.md) .

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo                                 | Descrição                                              |
|:-------------|:-------------------------------------|:---------------------------------------------------------|
|description   |String                                |Descrição resumida da instituição em que o usuário estudou. |
|displayName   |String                                |Nome da instituição em que o usuário estudou.              |
|localização      |[physicalAddress](physicaladdress.md) |Endereço ou local da instituição.                     |
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

