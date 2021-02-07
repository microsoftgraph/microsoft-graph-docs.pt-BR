---
title: Tipo de recurso conditionalAccessUsers
description: Representa usuários, grupos e funções incluídos e excluídos do escopo da política.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 8f75eb86ab9627b2cb9d507de9321743524203b3
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129769"
---
# <a name="conditionalaccessusers-resource-type"></a>Tipo de recurso conditionalAccessUsers

Namespace: microsoft.graph

Representa usuários, grupos e funções incluídos e excluídos do escopo da política.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| includeUsers | String collection | IDs de usuário no escopo da política, a menos que explicitamente excluídos, `None` ou `All` ou `GuestsOrExternalUsers` . |
| excludeUsers | String collection | IDs de usuário excluídas do escopo da política e/ou `GuestsOrExternalUsers` . |
| includeGroups | String collection | IDs de grupo no escopo da política, a menos que explicitamente excluídos, ou `All` . |
| excludeGroups | String collection | IDs de grupo excluídas do escopo da política. |
| includeRoles | String collection | IDs de função no escopo da política, a menos que explicitamente excluídos, ou `All` . |
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

