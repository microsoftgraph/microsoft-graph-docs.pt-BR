---
title: Tipo de recurso conditionalAccessLocations
description: Representa locais incluídos e excluídos do escopo da política.
ms.localizationpriority: medium
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 68804b5728fd058d2502ac041a24c3a218692b93
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59109240"
---
# <a name="conditionalaccesslocations-resource-type"></a>Tipo de recurso conditionalAccessLocations

Namespace: microsoft.graph

Representa locais incluídos e excluídos do escopo da política.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| includeLocations | Coleção String | IDs de local no escopo da política, a menos que explicitamente `All` excluídas, ou `AllTrusted` . |
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

