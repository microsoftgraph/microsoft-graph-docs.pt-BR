---
title: Tipo de recurso conditionalAccessApplications
description: Representa aplicativos e ações do usuário incluídas e excluídas do escopo da política.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 0a787a1c22209b502e4eed68790629e2e6e1b03b
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137395"
---
# <a name="conditionalaccessapplications-resource-type"></a>Tipo de recurso conditionalAccessApplications

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os aplicativos e as ações do usuário incluídas e excluídas da política.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-------- |:---- |:----------- |
| includeApplications | Coleção de cadeias de caracteres | A lista de IDs de aplicativos a que a política se aplica, a menos que explicitamente excluída (em excludeApplications). Também pode ser definido como `All` . |
| excludeApplications | Coleção de cadeias de caracteres | A lista de IDs de aplicativo explicitamente excluída da política. |
| includeUserActions | Coleção de cadeias de caracteres | Ações do usuário a incluir. Os valores com suporte `urn:user:registersecurityinfo` são e `urn:user:registerdevice` |

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

