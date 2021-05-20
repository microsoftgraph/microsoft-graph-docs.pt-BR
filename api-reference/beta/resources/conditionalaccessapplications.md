---
title: Tipo de recurso conditionalAccessApplications
description: Representa aplicativos e ações do usuário incluídas e excluídas do escopo da política.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: d688b529e32390c2330cf8cb3558994c3e752a25
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547680"
---
# <a name="conditionalaccessapplications-resource-type"></a>Tipo de recurso conditionalAccessApplications

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os aplicativos e as ações do usuário incluídas e excluídas da política.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-------- |:---- |:----------- |
| includeApplications | Coleção de cadeias de caracteres | A lista de IDs de aplicativo a que a política se aplica, a menos que seja explicitamente excluída (em excludeApplications). Também pode ser definido como `All` . |
| excludeApplications | Coleção de cadeias de caracteres | A lista de IDs de aplicativos excluídas explicitamente da política. |
| includeUserActions | Coleção de cadeias de caracteres | Ações do usuário a incluir. Os valores com suporte `urn:user:registersecurityinfo` são e `urn:user:registerdevice` |
| includeAuthenticationContextClassReferences | Coleção de cadeias de caracteres | As referências de classe de contexto de autenticação incluem. Os valores suportados são `c1` através `c25` de . |

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

