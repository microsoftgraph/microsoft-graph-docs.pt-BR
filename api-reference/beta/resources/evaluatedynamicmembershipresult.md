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
# <a name="evaluatedynamicmembershipresult-resource-type"></a><span data-ttu-id="208c4-103">tipo de recurso evaluateDynamicMembershipResult</span><span class="sxs-lookup"><span data-stu-id="208c4-103">evaluateDynamicMembershipResult resource type</span></span>

<span data-ttu-id="208c4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="208c4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="208c4-105">Representa o resultado da avaliação de associação.</span><span class="sxs-lookup"><span data-stu-id="208c4-105">Represents the result of membership evaluation.</span></span>

## <a name="properties"></a><span data-ttu-id="208c4-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="208c4-106">Properties</span></span>

| <span data-ttu-id="208c4-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="208c4-107">Property</span></span> | <span data-ttu-id="208c4-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="208c4-108">Type</span></span> | <span data-ttu-id="208c4-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="208c4-109">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="208c4-110">membershipRule</span><span class="sxs-lookup"><span data-stu-id="208c4-110">membershipRule</span></span> | <span data-ttu-id="208c4-111">String</span><span class="sxs-lookup"><span data-stu-id="208c4-111">String</span></span> | <span data-ttu-id="208c4-112">Se uma ID de grupo for fornecida, o valor será a regra de associação do grupo.</span><span class="sxs-lookup"><span data-stu-id="208c4-112">If a group ID is provided, the value is the membership rule for the group.</span></span> <span data-ttu-id="208c4-113">Se uma ID de grupo não for fornecida, o valor será a regra de associação fornecida como um parâmetro.</span><span class="sxs-lookup"><span data-stu-id="208c4-113">If a group ID is not provided, the value is the membership rule that was provided as a parameter.</span></span> <span data-ttu-id="208c4-114">Para obter mais informações, consulte [regras de associação dinâmicas para grupos no Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/groups-dynamic-membership).</span><span class="sxs-lookup"><span data-stu-id="208c4-114">For more information, see [Dynamic membership rules for groups in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/groups-dynamic-membership).</span></span> |
| <span data-ttu-id="208c4-115">membershipRuleEvaluationDetails</span><span class="sxs-lookup"><span data-stu-id="208c4-115">membershipRuleEvaluationDetails</span></span> | [<span data-ttu-id="208c4-116">expressionEvaluationDetails</span><span class="sxs-lookup"><span data-stu-id="208c4-116">expressionEvaluationDetails</span></span>](expressionevaluationdetails.md) | <span data-ttu-id="208c4-117">Fornece uma Anaylsis detalhada do resultado de avaliação da associação.</span><span class="sxs-lookup"><span data-stu-id="208c4-117">Provides a detailed anaylsis of the membership evaluation result.</span></span> |
| <span data-ttu-id="208c4-118">membershipRuleEvaluationResult</span><span class="sxs-lookup"><span data-stu-id="208c4-118">membershipRuleEvaluationResult</span></span> | <span data-ttu-id="208c4-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="208c4-119">Boolean</span></span> | <span data-ttu-id="208c4-120">O valor é `true` se o usuário ou o dispositivo é um membro do grupo.</span><span class="sxs-lookup"><span data-stu-id="208c4-120">The value is `true` if the user or device is a member of the group.</span></span> <span data-ttu-id="208c4-121">O valor também pode ser `true` se uma regra de associação foi fornecida e o usuário ou dispositivo passa a avaliação de regra; caso contrário `false` .</span><span class="sxs-lookup"><span data-stu-id="208c4-121">The value can also be `true` if a membership rule was provided and the user or device passes the rule evaluation; otherwise `false`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="208c4-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="208c4-122">JSON representation</span></span>

<span data-ttu-id="208c4-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="208c4-123">The following is a JSON representation of the resource.</span></span>

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

