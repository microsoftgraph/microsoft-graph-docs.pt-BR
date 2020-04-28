---
title: tipo de recurso conditionalAccessApplications
description: Representa os aplicativos e as ações do usuário incluídos e excluídos do escopo da política.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a1ce31fd39c94299ccb6e2a0cc1330a44a149db3
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2020
ms.locfileid: "43916848"
---
# <a name="conditionalaccessapplications-resource-type"></a>tipo de recurso conditionalAccessApplications

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os aplicativos e as ações do usuário incluídos no e excluídos da política.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-------- |:---- |:----------- |
| includeApplications | Coleção de cadeias de caracteres | A lista de IDs de aplicativo à qual a política se aplica, a menos que explicitamente excluída (em excludeApplications). Também pode ser definido como `All`. |
| excludeApplications | Coleção de cadeias de caracteres | A lista de IDs de aplicativo explicitamente excluídas da política. |
| includeUserActions | Coleção de cadeias de caracteres | Ações do usuário a serem incluídas ( `urn:user:registersecurityinfo`por exemplo,) |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "includeApplications",
    "excludeApplications",
    "includeUserActions"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessApplications"
}-->

```json
{
  "includeApplications": ["String"],
  "excludeApplications": ["String"],
  "includeUserActions": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessApplications resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->