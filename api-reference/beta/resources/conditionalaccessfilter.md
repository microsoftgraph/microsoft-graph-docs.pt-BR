---
title: Tipo de recurso conditionalAccessFilter
description: Representa o filtro no escopo da política.
localization_priority: Normal
author: sandeo
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 9f5b14a3faa593453c88cc155f7e44348fcfda35
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082402"
---
# <a name="conditionalaccessfilter-resource-type"></a>Tipo de recurso conditionalAccessFilter

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o filtro no escopo da política.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| modo | filterMode | Modo a ser usado para o filtro. Os valores possíveis são: `include` ou `exclude`. |
| rule | String | A sintaxe de regra é semelhante à usada para regras de associação para grupos no Azure AD. Para obter detalhes, consulte [regras com várias expressões](/azure/active-directory/enterprise-users/groups-dynamic-membership#rules-with-multiple-expressions) |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "mode",
    "rule"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessFilter",
  "baseType": null
}-->

```json
{
  "mode": "String",
  "rule": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessFilter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


