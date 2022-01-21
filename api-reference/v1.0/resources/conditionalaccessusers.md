---
title: Tipo de recurso conditionalAccessUsers
description: Representa usuários, grupos e funções incluídas e excluídas do escopo da política.
ms.localizationpriority: medium
author: davidspooner
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 5d425a2c5387f940c1e6d475a5bac26c85ebfaaf
ms.sourcegitcommit: 3f3975916b5c531ee63d92340ccd6e73e879e8d7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/21/2022
ms.locfileid: "62162094"
---
# <a name="conditionalaccessusers-resource-type"></a>Tipo de recurso conditionalAccessUsers

Namespace: microsoft.graph

Representa usuários, grupos e funções incluídas e excluídas do escopo da política.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| includeUsers | Coleção String | IDs de usuário no escopo da política, a menos que explicitamente excluídas, `None` ou `All` ou ou `GuestsOrExternalUsers` . |
| excludeUsers | Coleção String | IDs de usuário excluídas do escopo da política e/ou `GuestsOrExternalUsers` . |
| includeGroups | Coleção String | IDs de grupo no escopo da política, a menos que explicitamente excluídas, ou `All` . |
| excludeGroups | Coleção String | IDs de grupo excluídas do escopo da política. |
| includeRoles | Coleção String | IDs de função no escopo da política, a menos que explicitamente excluídas, ou `All` . |
| excludeRoles | Coleção String | IDs de função excluídas do escopo da política. |

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

