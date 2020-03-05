---
title: tipo de recurso conditionalAccessUsers
description: Representa usuários, grupos e funções incluídos e excluídos do escopo da política.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 269fe0552c69773fa62b97cf9803b3e0127f655b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507503"
---
# <a name="conditionalaccessusers-resource-type"></a>tipo de recurso conditionalAccessUsers

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa usuários, grupos e funções incluídos e excluídos do escopo da política.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| includeUsers | String collection | IDs de usuário em escopo de política, a menos que `None` explicitamente `All` excluído `GuestsOrExternalUsers`ou ou. |
| excludeUsers | String collection | IDs de usuário excluídas do escopo da política e `GuestsOrExternalUsers`/ou. |
| includeGroups | String collection | IDs de grupo em escopo de política, a menos que `All`explicitamente excluído ou. |
| excludeGroups | String collection | IDs de grupo excluídas do escopo da política. |
| includeRoles | String collection | IDs de função em escopo de política, a menos que `All`explicitamente excluído ou. |
| excludeRoles | String collection | IDs de função excluídas do escopo da política. |

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