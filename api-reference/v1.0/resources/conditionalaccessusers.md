---
title: Tipo de recurso conditionalAccessUsers
description: Representa usuários, grupos e funções incluídas e excluídas do escopo da política.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 9f9930d1d1ac1b5d355699b893bfbf59f047162d1d0c0f39d0303a98b889ab7f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54229301"
---
# <a name="conditionalaccessusers-resource-type"></a>Tipo de recurso conditionalAccessUsers

Namespace: microsoft.graph

Representa usuários, grupos e funções incluídas e excluídas do escopo da política.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| includeUsers | Coleção de cadeias de caracteres | IDs de usuário no escopo da política, a menos que explicitamente excluídas, `None` ou `All` ou ou `GuestsOrExternalUsers` . |
| excludeUsers | Coleção de cadeias de caracteres | IDs de usuário excluídas do escopo da política e/ou `GuestsOrExternalUsers` . |
| includeGroups | Coleção de cadeias de caracteres | IDs de grupo no escopo da política, a menos que explicitamente excluídas, ou `All` . |
| excludeGroups | Coleção de cadeias de caracteres | IDs de grupo excluídas do escopo da política. |
| includeRoles | Coleção de cadeias de caracteres | IDs de função no escopo da política, a menos que explicitamente excluídas, ou `All` . |
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

