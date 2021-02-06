---
title: Tipo de recurso evaluateDynamicMembershipResult
description: Representa o resultado da avaliação de associação.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 1df07449605f3b1d48c01b1e352100d534fc9b1d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129503"
---
# <a name="evaluatedynamicmembershipresult-resource-type"></a>Tipo de recurso evaluateDynamicMembershipResult

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o resultado da avaliação de associação.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-------- |:---- |:----------- |
| membershipRule | String | Se uma ID de grupo for fornecida, o valor será a regra de associação para o grupo. Se uma ID de grupo não for fornecida, o valor será a regra de associação que foi fornecida como um parâmetro. Para saber mais, confira [Regras de associação dinâmica para grupos no Azure Active Directory.](/azure/active-directory/users-groups-roles/groups-dynamic-membership) |
| membershipRuleEvaluationDetails | [expressionEvaluationDetails](expressionevaluationdetails.md) | Fornece uma análoga detalhada do resultado da avaliação de associação. |
| membershipRuleEvaluationResult | Boolean | O valor é `true` se o usuário ou dispositivo for um membro do grupo. O valor também pode ser se uma regra de associação foi fornecida e o usuário ou dispositivo passa na `true` avaliação de regra; caso `false` contrário. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.evaluateDynamicMembershipResult",
  "baseType": null
}-->

```json
{
  "membershipRule": "String",
  "membershipRuleEvaluationDetails": {"@odata.type": "microsoft.graph.expressionEvaluationDetails"},
  "membershipRuleEvaluationResult": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "evaluateDynamicMembershipResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->