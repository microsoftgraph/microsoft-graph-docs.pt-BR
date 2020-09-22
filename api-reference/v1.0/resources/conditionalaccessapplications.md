---
title: tipo de recurso conditionalAccessApplications
description: Representa os aplicativos e as ações do usuário incluídos e excluídos do escopo da política.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5a9794a274b876ba93cc3fdbe14ea7731776daa3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057042"
---
# <a name="conditionalaccessapplications-resource-type"></a>tipo de recurso conditionalAccessApplications

Namespace: microsoft.graph

Representa os aplicativos e as ações do usuário incluídos no e excluídos da política.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| includeApplications | Coleção de cadeias de caracteres | A lista de IDs de aplicativo à qual a política se aplica, a menos que explicitamente excluída (em excludeApplications). Também pode ser definido como `All` . |
| excludeApplications | Coleção de cadeias de caracteres | A lista de IDs de aplicativo explicitamente excluídas da política. |
| includeUserActions | Coleção de cadeias de caracteres | Ações do usuário a serem incluídas. Por exemplo, `urn:user:registersecurityinfo` |

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

