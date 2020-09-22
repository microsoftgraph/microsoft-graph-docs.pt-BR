---
title: tipo de recurso conditionalAccessLocations
description: Representa os locais incluídos e excluídos do escopo da política.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2a6b4175decf2d4985d17b64014b09d9299af06e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021949"
---
# <a name="conditionalaccesslocations-resource-type"></a>tipo de recurso conditionalAccessLocations

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os locais incluídos e excluídos do escopo da política.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| includeLocations | Coleção String | IDs de local em escopo de política, a menos que explicitamente excluído, `All` ou `AllTrusted` . |
| excludeLocations | Coleção String | IDs de local excluídas do escopo da política. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

## <a name="relationships"></a>Relações

Nenhum

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "includeLocations",
    "excludeLocations"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessLocations",
  "baseType": null
}-->

```json
{
  "excludeLocations": ["String"],
  "includeLocations": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessLocations resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

