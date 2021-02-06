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
# <a name="evaluatedynamicmembershipresult-resource-type"></a><span data-ttu-id="b53f3-103">Tipo de recurso evaluateDynamicMembershipResult</span><span class="sxs-lookup"><span data-stu-id="b53f3-103">evaluateDynamicMembershipResult resource type</span></span>

<span data-ttu-id="b53f3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b53f3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b53f3-105">Representa o resultado da avaliação de associação.</span><span class="sxs-lookup"><span data-stu-id="b53f3-105">Represents the result of membership evaluation.</span></span>

## <a name="properties"></a><span data-ttu-id="b53f3-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b53f3-106">Properties</span></span>

| <span data-ttu-id="b53f3-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b53f3-107">Property</span></span> | <span data-ttu-id="b53f3-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b53f3-108">Type</span></span> | <span data-ttu-id="b53f3-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b53f3-109">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="b53f3-110">membershipRule</span><span class="sxs-lookup"><span data-stu-id="b53f3-110">membershipRule</span></span> | <span data-ttu-id="b53f3-111">String</span><span class="sxs-lookup"><span data-stu-id="b53f3-111">String</span></span> | <span data-ttu-id="b53f3-112">Se uma ID de grupo for fornecida, o valor será a regra de associação para o grupo.</span><span class="sxs-lookup"><span data-stu-id="b53f3-112">If a group ID is provided, the value is the membership rule for the group.</span></span> <span data-ttu-id="b53f3-113">Se uma ID de grupo não for fornecida, o valor será a regra de associação que foi fornecida como um parâmetro.</span><span class="sxs-lookup"><span data-stu-id="b53f3-113">If a group ID is not provided, the value is the membership rule that was provided as a parameter.</span></span> <span data-ttu-id="b53f3-114">Para saber mais, confira [Regras de associação dinâmica para grupos no Azure Active Directory.](/azure/active-directory/users-groups-roles/groups-dynamic-membership)</span><span class="sxs-lookup"><span data-stu-id="b53f3-114">For more information, see [Dynamic membership rules for groups in Azure Active Directory](/azure/active-directory/users-groups-roles/groups-dynamic-membership).</span></span> |
| <span data-ttu-id="b53f3-115">membershipRuleEvaluationDetails</span><span class="sxs-lookup"><span data-stu-id="b53f3-115">membershipRuleEvaluationDetails</span></span> | [<span data-ttu-id="b53f3-116">expressionEvaluationDetails</span><span class="sxs-lookup"><span data-stu-id="b53f3-116">expressionEvaluationDetails</span></span>](expressionevaluationdetails.md) | <span data-ttu-id="b53f3-117">Fornece uma análoga detalhada do resultado da avaliação de associação.</span><span class="sxs-lookup"><span data-stu-id="b53f3-117">Provides a detailed anaylsis of the membership evaluation result.</span></span> |
| <span data-ttu-id="b53f3-118">membershipRuleEvaluationResult</span><span class="sxs-lookup"><span data-stu-id="b53f3-118">membershipRuleEvaluationResult</span></span> | <span data-ttu-id="b53f3-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="b53f3-119">Boolean</span></span> | <span data-ttu-id="b53f3-120">O valor é `true` se o usuário ou dispositivo for um membro do grupo.</span><span class="sxs-lookup"><span data-stu-id="b53f3-120">The value is `true` if the user or device is a member of the group.</span></span> <span data-ttu-id="b53f3-121">O valor também pode ser se uma regra de associação foi fornecida e o usuário ou dispositivo passa na `true` avaliação de regra; caso `false` contrário.</span><span class="sxs-lookup"><span data-stu-id="b53f3-121">The value can also be `true` if a membership rule was provided and the user or device passes the rule evaluation; otherwise `false`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b53f3-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b53f3-122">JSON representation</span></span>

<span data-ttu-id="b53f3-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b53f3-123">The following is a JSON representation of the resource.</span></span>

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