---
title: Tipo de recurso conditionalAccessApplications
description: Representa aplicativos e ações do usuário incluídas e excluídas do escopo da política.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 42ceafb6c786666378d1327ecd158a04559d7f0d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132157"
---
# <a name="conditionalaccessapplications-resource-type"></a>Tipo de recurso conditionalAccessApplications

Namespace: microsoft.graph

Representa os aplicativos e as ações do usuário incluídas e excluídas da política.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| includeApplications | String collection | A lista de IDs de aplicativos a que a política se aplica, a menos que explicitamente excluída (em excludeApplications). Também pode ser definido como `All` . |
| excludeApplications | String collection | A lista de IDs de aplicativo explicitamente excluída da política. |
| includeUserActions | String collection | Ações do usuário a incluir. Por exemplo, `urn:user:registersecurityinfo` |

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

