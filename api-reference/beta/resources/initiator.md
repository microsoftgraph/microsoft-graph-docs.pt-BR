---
title: tipo de recurso do iniciador
description: Descreve quem ou o que iniciou o evento de provisionamento.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6d279ce00855cb8125085e48bddf63f1b8f0e5e2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43461724"
---
# <a name="initiator-resource-type"></a>tipo de recurso do iniciador

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descreve quem ou o que iniciou o evento de provisionamento. 

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|displayName|Cadeia de caracteres|Nome da pessoa ou serviço que iniciou o evento de provisionamento.|
|id|String|Identifica exclusivamente a pessoa ou o serviço que iniciou o evento de provisionamento.|
|initiatortype|String| Tipo de iniciador. Os valores possíveis são: `user`, `app`, `system`, `unknownFutureValue`.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.initiator",
  "baseType": null
}-->

```json
{
  "displayName": "String",
  "id": "String",
  "initiatorType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "initiator resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
