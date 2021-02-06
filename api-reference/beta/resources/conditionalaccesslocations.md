---
title: Tipo de recurso conditionalAccessLocations
description: Representa locais incluídos e excluídos do escopo da política.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 153d64d32015fcd6119a4d880bbc786905c39b9f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132375"
---
# <a name="conditionalaccesslocations-resource-type"></a>Tipo de recurso conditionalAccessLocations

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa locais incluídos e excluídos do escopo da política.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| includeLocations | Coleção de cadeias de caracteres | IDs de local no escopo da política, a menos que explicitamente `All` excluído, ou `AllTrusted` . |
| excludeLocations | Coleção de cadeias de caracteres | IDs de local excluídas do escopo da política. |

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

