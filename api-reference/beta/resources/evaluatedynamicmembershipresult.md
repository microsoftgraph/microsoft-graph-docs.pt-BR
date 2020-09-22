---
title: tipo de recurso evaluateDynamicMembershipResult
description: Representa o resultado da avaliação de associação.
localization_priority: Normal
author: yyuank
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a38ae33d59ea8deba8a71e48698baeddf709ae9e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071231"
---
# <a name="evaluatedynamicmembershipresult-resource-type"></a>tipo de recurso evaluateDynamicMembershipResult

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o resultado da avaliação de associação.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-------- |:---- |:----------- |
| membershipRule | String | Se uma ID de grupo for fornecida, o valor será a regra de associação do grupo. Se uma ID de grupo não for fornecida, o valor será a regra de associação fornecida como um parâmetro. Para obter mais informações, consulte [regras de associação dinâmicas para grupos no Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/groups-dynamic-membership). |
| membershipRuleEvaluationDetails | [expressionEvaluationDetails](expressionevaluationdetails.md) | Fornece uma Anaylsis detalhada do resultado de avaliação da associação. |
| membershipRuleEvaluationResult | Booliano | O valor é `true` se o usuário ou o dispositivo é um membro do grupo. O valor também pode ser `true` se uma regra de associação foi fornecida e o usuário ou dispositivo passa a avaliação de regra; caso contrário `false` . |

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

