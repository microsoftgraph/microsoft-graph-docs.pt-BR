---
title: tipo de recurso conditionalAccessUsers
description: Representa usuários, grupos e funções incluídos e excluídos do escopo da política.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d1294551fd568b9f41072d3707d64a88d4b04edc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47994229"
---
# <a name="conditionalaccessusers-resource-type"></a>tipo de recurso conditionalAccessUsers

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa usuários, grupos e funções incluídos e excluídos do escopo da política.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| includeUsers | Coleção de cadeias de caracteres | IDs de usuário em escopo de política, a menos que explicitamente excluído ou ou `None` `All` `GuestsOrExternalUsers` . |
| excludeUsers | Coleção de cadeias de caracteres | IDs de usuário excluídas do escopo da política e/ou `GuestsOrExternalUsers` . |
| includeGroups | Coleção de cadeias de caracteres | IDs de grupo em escopo de política, a menos que explicitamente excluído ou `All` . |
| excludeGroups | Coleção de cadeias de caracteres | IDs de grupo excluídas do escopo da política. |
| includeRoles | Coleção de cadeias de caracteres | IDs de função em escopo de política, a menos que explicitamente excluído ou `All` . |
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

