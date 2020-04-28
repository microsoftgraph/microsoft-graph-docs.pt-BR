---
title: tipo de recurso conditionalAccessUsers
description: Representa usuários, grupos e funções incluídos e excluídos do escopo da política.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ad9c41e91a71fa00af71c05bc5c9d0591f81826b
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2020
ms.locfileid: "43916673"
---
# <a name="conditionalaccessusers-resource-type"></a>tipo de recurso conditionalAccessUsers

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa usuários, grupos e funções incluídos e excluídos do escopo da política.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| includeUsers | Coleção de cadeias de caracteres | IDs de usuário em escopo de política, a menos que `None` explicitamente `All` excluído `GuestsOrExternalUsers`ou ou. |
| excludeUsers | Coleção de cadeias de caracteres | IDs de usuário excluídas do escopo da política e `GuestsOrExternalUsers`/ou. |
| includeGroups | Coleção de cadeias de caracteres | IDs de grupo em escopo de política, a menos que `All`explicitamente excluído ou. |
| excludeGroups | Coleção de cadeias de caracteres | IDs de grupo excluídas do escopo da política. |
| includeRoles | Coleção de cadeias de caracteres | IDs de função em escopo de política, a menos que `All`explicitamente excluído ou. |
| excludeRoles | Coleção de cadeias de caracteres | IDs de função excluídas do escopo da política. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "includeUsers",
    "excludeUsers",
    "includeGroups",
    "excludeGroups",
    "includeRoles",
    "excludeRoles"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessUsers",
  "baseType": null
}-->

```json
{
  "excludeGroups": ["String"],
  "excludeRoles": ["String"],
  "excludeUsers": ["String"],
  "includeGroups": ["String"],
  "includeRoles": ["String"],
  "includeUsers": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessUsers resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->