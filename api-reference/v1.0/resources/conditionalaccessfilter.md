---
title: Tipo de recurso conditionalAccessFilter
description: Representa o filtro no escopo da política.
ms.localizationpriority: medium
author: sandeo
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3821fe6268887232d8db3cfd8f84ba2c67f07926
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/19/2021
ms.locfileid: "60494280"
---
# <a name="conditionalaccessfilter-resource-type"></a>Tipo de recurso conditionalAccessFilter

Namespace: microsoft.graph

Representa o filtro no escopo da política.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| modo | filterMode | Modo a ser usado para o filtro. Os valores possíveis são: `include` ou `exclude`. |
| rule | Cadeia de caracteres | A sintaxe de regra é semelhante à usada para regras de associação para grupos Azure Active Directory (Azure AD). Para obter detalhes, consulte [regras com várias expressões](/azure/active-directory/enterprise-users/groups-dynamic-membership#rules-with-multiple-expressions) |

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


