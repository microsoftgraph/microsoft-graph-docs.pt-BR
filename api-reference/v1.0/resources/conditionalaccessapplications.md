---
title: tipo de recurso conditionalAccessApplications
description: Representa os aplicativos e as ações do usuário incluídos e excluídos do escopo da política.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8b09a3531d3734aed67e9ff91fee1d917f76054b
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384410"
---
# <a name="conditionalaccessapplications-resource-type"></a>tipo de recurso conditionalAccessApplications

Namespace: microsoft.graph

Representa os aplicativos e as ações do usuário incluídos no e excluídos da política.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| includeApplications | String collection | A lista de IDs de aplicativo à qual a política se aplica, a menos que explicitamente excluída (em excludeApplications). Também pode ser definido como `All` . |
| excludeApplications | String collection | A lista de IDs de aplicativo explicitamente excluídas da política. |
| includeUserActions | String collection | Ações do usuário a serem incluídas. Por exemplo, `urn:user:registersecurityinfo` |

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