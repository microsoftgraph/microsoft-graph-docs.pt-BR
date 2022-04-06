---
title: Tipo de recurso evaluateDynamicMembershipResult
description: Representa o resultado da avaliação de associação.
ms.localizationpriority: medium
author: psaffaie
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 551c2c87a09b7f2ddafc2079ab97c7f7e36837cd
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2022
ms.locfileid: "64588516"
---
# <a name="evaluatedynamicmembershipresult-resource-type"></a>Tipo de recurso evaluateDynamicMembershipResult

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o resultado da avaliação de associação.

## <a name="properties"></a>Propriedades

| Propriedade                        | Tipo                                                          | Descrição                                                                                                                                                                                                                                                                                                                                   |
| :------------------------------ | :------------------------------------------------------------ | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| membershipRule                  | String                                                        | Se uma ID de grupo for fornecida, o valor será a regra de associação para o grupo. Se uma ID de grupo não for fornecida, o valor será a regra de associação fornecida como parâmetro. Para obter mais informações, [regras de associação dinâmica para grupos no Azure Active Directory](/azure/active-directory/users-groups-roles/groups-dynamic-membership). |
| membershipRuleEvaluationDetails | [expressionEvaluationDetails](expressionevaluationdetails.md) | Fornece uma análoga detalhada do resultado da avaliação de associação.                                                                                                                                                                                                                                                                             |
| membershipRuleEvaluationResult  | Booliano                                                       | O valor é `true` se o usuário ou dispositivo for um membro do grupo. O valor também pode ser se `true` uma regra de associação tiver sido fornecida e o usuário ou dispositivo passar na avaliação de regra; caso contrário `false`.                                                                                                                                      |

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
  "membershipRuleEvaluationDetails": {
    "@odata.type": "microsoft.graph.expressionEvaluationDetails"
  },
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
