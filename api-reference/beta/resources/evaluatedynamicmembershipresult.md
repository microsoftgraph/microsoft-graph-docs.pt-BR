---
title: tipo de recurso evaluateDynamicMembershipResult
description: Representa o resultado da avaliação de associação.
localization_priority: Normal
author: yyuank
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d00a2f1a0376c0d631354ea4f05c542dd4d1dcef
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48402532"
---
# <a name="evaluatedynamicmembershipresult-resource-type"></a><span data-ttu-id="385d1-103">tipo de recurso evaluateDynamicMembershipResult</span><span class="sxs-lookup"><span data-stu-id="385d1-103">evaluateDynamicMembershipResult resource type</span></span>

<span data-ttu-id="385d1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="385d1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="385d1-105">Representa o resultado da avaliação de associação.</span><span class="sxs-lookup"><span data-stu-id="385d1-105">Represents the result of membership evaluation.</span></span>

## <a name="properties"></a><span data-ttu-id="385d1-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="385d1-106">Properties</span></span>

| <span data-ttu-id="385d1-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="385d1-107">Property</span></span> | <span data-ttu-id="385d1-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="385d1-108">Type</span></span> | <span data-ttu-id="385d1-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="385d1-109">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="385d1-110">membershipRule</span><span class="sxs-lookup"><span data-stu-id="385d1-110">membershipRule</span></span> | <span data-ttu-id="385d1-111">String</span><span class="sxs-lookup"><span data-stu-id="385d1-111">String</span></span> | <span data-ttu-id="385d1-112">Se uma ID de grupo for fornecida, o valor será a regra de associação do grupo.</span><span class="sxs-lookup"><span data-stu-id="385d1-112">If a group ID is provided, the value is the membership rule for the group.</span></span> <span data-ttu-id="385d1-113">Se uma ID de grupo não for fornecida, o valor será a regra de associação fornecida como um parâmetro.</span><span class="sxs-lookup"><span data-stu-id="385d1-113">If a group ID is not provided, the value is the membership rule that was provided as a parameter.</span></span> <span data-ttu-id="385d1-114">Para obter mais informações, consulte [regras de associação dinâmicas para grupos no Azure Active Directory](/azure/active-directory/users-groups-roles/groups-dynamic-membership).</span><span class="sxs-lookup"><span data-stu-id="385d1-114">For more information, see [Dynamic membership rules for groups in Azure Active Directory](/azure/active-directory/users-groups-roles/groups-dynamic-membership).</span></span> |
| <span data-ttu-id="385d1-115">membershipRuleEvaluationDetails</span><span class="sxs-lookup"><span data-stu-id="385d1-115">membershipRuleEvaluationDetails</span></span> | [<span data-ttu-id="385d1-116">expressionEvaluationDetails</span><span class="sxs-lookup"><span data-stu-id="385d1-116">expressionEvaluationDetails</span></span>](expressionevaluationdetails.md) | <span data-ttu-id="385d1-117">Fornece uma Anaylsis detalhada do resultado de avaliação da associação.</span><span class="sxs-lookup"><span data-stu-id="385d1-117">Provides a detailed anaylsis of the membership evaluation result.</span></span> |
| <span data-ttu-id="385d1-118">membershipRuleEvaluationResult</span><span class="sxs-lookup"><span data-stu-id="385d1-118">membershipRuleEvaluationResult</span></span> | <span data-ttu-id="385d1-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="385d1-119">Boolean</span></span> | <span data-ttu-id="385d1-120">O valor é `true` se o usuário ou o dispositivo é um membro do grupo.</span><span class="sxs-lookup"><span data-stu-id="385d1-120">The value is `true` if the user or device is a member of the group.</span></span> <span data-ttu-id="385d1-121">O valor também pode ser `true` se uma regra de associação foi fornecida e o usuário ou dispositivo passa a avaliação de regra; caso contrário `false` .</span><span class="sxs-lookup"><span data-stu-id="385d1-121">The value can also be `true` if a membership rule was provided and the user or device passes the rule evaluation; otherwise `false`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="385d1-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="385d1-122">JSON representation</span></span>

<span data-ttu-id="385d1-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="385d1-123">The following is a JSON representation of the resource.</span></span>

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