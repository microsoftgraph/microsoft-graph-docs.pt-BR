---
title: Tipo de recurso evaluateDynamicMembershipResult
description: Representa o resultado da avaliação de associação.
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 52621ee317183a59da418ecd35309cacc0637ae3
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682639"
---
# <a name="evaluatedynamicmembershipresult-resource-type"></a>Tipo de recurso evaluateDynamicMembershipResult

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o resultado da avaliação de associação.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-------- |:---- |:----------- |
| membershipRule | String | Se uma ID de grupo for fornecida, o valor será a regra de associação para o grupo. Se uma ID de grupo não for fornecida, o valor será a regra de associação fornecida como parâmetro. Para obter mais informações, consulte [Regras de associação dinâmicas para grupos em Azure Active Directory](/azure/active-directory/users-groups-roles/groups-dynamic-membership). |
| membershipRuleEvaluationDetails | [expressionEvaluationDetails](expressionevaluationdetails.md) | Fornece uma análoga detalhada do resultado da avaliação de associação. |
| membershipRuleEvaluationResult | Boolean | O valor é `true` se o usuário ou dispositivo for um membro do grupo. O valor também pode ser se uma regra de associação tiver sido fornecida e o usuário ou dispositivo passar na avaliação `true` de regra; caso `false` contrário. |

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