---
title: Tipo de recurso accessReviewInstanceDecisionItem
description: Representa uma decisão sobre o acesso de um usuário em um accessReviewInstance.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 228fbe473fe65fe84c9dfa7c62f3689681d47e39
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443185"
---
# <a name="accessreviewinstancedecisionitem-resource-type"></a><span data-ttu-id="7be49-103">Tipo de recurso accessReviewInstanceDecisionItem</span><span class="sxs-lookup"><span data-stu-id="7be49-103">accessReviewInstanceDecisionItem resource type</span></span>

<span data-ttu-id="7be49-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7be49-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="7be49-105">Representa uma decisão de revisão [de](accessreviewsv2-root.md) acesso do Azure AD em uma instância de uma revisão.</span><span class="sxs-lookup"><span data-stu-id="7be49-105">Represents an Azure AD [access review](accessreviewsv2-root.md) decision on an instance of a review.</span></span> <span data-ttu-id="7be49-106">Essa decisão representa a determinação do acesso de um usuário ou entidade de serviço para uma determinada instância de revisão [de acesso.](accessreviewinstance.md)</span><span class="sxs-lookup"><span data-stu-id="7be49-106">This decision represents the determination of a user or service principal's access for a given [access review instance](accessreviewinstance.md).</span></span>

## <a name="methods"></a><span data-ttu-id="7be49-107">Methods</span><span class="sxs-lookup"><span data-stu-id="7be49-107">Methods</span></span>

| <span data-ttu-id="7be49-108">Método</span><span class="sxs-lookup"><span data-stu-id="7be49-108">Method</span></span> | <span data-ttu-id="7be49-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7be49-109">Return Type</span></span> | <span data-ttu-id="7be49-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7be49-110">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="7be49-111">Listar accessReviewInstanceDecisionItems</span><span class="sxs-lookup"><span data-stu-id="7be49-111">List accessReviewInstanceDecisionItems</span></span>](../api/accessreviewinstancedecisionitem-list.md) | <span data-ttu-id="7be49-112">[Coleção accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md)</span><span class="sxs-lookup"><span data-stu-id="7be49-112">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection</span></span> | <span data-ttu-id="7be49-113">Lista cada accessReviewInstanceDecisionItem para um accessReviewInstance específico.</span><span class="sxs-lookup"><span data-stu-id="7be49-113">Lists every accessReviewInstanceDecisionItem for a specific accessReviewInstance.</span></span> |
|[<span data-ttu-id="7be49-114">Listar accessReviewInstanceDecisionItems aguardando aprovação</span><span class="sxs-lookup"><span data-stu-id="7be49-114">List accessReviewInstanceDecisionItems pending approval</span></span>](../api/accessreviewinstancedecisionitem-listpendingapproval.md) | <span data-ttu-id="7be49-115">[Coleção accessReviewInstanceDecisionItem.](accessreviewinstancedecisionitem.md)</span><span class="sxs-lookup"><span data-stu-id="7be49-115">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection.</span></span> | <span data-ttu-id="7be49-116">Obter todos os accessReviewInstanceDecisionItems atribuídos ao usuário de chamada, para um accessReviewInstance específico.</span><span class="sxs-lookup"><span data-stu-id="7be49-116">Get all accessReviewInstanceDecisionItems assigned to the calling user, for a specific accessReviewInstance.</span></span> |
|[<span data-ttu-id="7be49-117">Atualizar accessReviewInstanceDecisionItem</span><span class="sxs-lookup"><span data-stu-id="7be49-117">Update accessReviewInstanceDecisionItem</span></span>](../api/accessreviewinstancedecisionitem-update.md) | <span data-ttu-id="7be49-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7be49-118">None.</span></span> | <span data-ttu-id="7be49-119">Para qualquer accessReviewInstanceDecisionItems em que o usuário de chamada recebe um revisor, chamar o usuário pode registrar uma decisão corrigindo o objeto decision.</span><span class="sxs-lookup"><span data-stu-id="7be49-119">For any accessReviewInstanceDecisionItems that the calling user is assigned a reviewer on, calling user can record a decision by patching the decision object.</span></span> |

## <a name="properties"></a><span data-ttu-id="7be49-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7be49-120">Properties</span></span>
| <span data-ttu-id="7be49-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7be49-121">Property</span></span> | <span data-ttu-id="7be49-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="7be49-122">Type</span></span> |  <span data-ttu-id="7be49-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="7be49-123">Description</span></span> |
| :---------------| :---- | :---------- |
| <span data-ttu-id="7be49-124">id</span><span class="sxs-lookup"><span data-stu-id="7be49-124">id</span></span> | <span data-ttu-id="7be49-125">String</span><span class="sxs-lookup"><span data-stu-id="7be49-125">String</span></span> | <span data-ttu-id="7be49-126">O identificador da decisão.</span><span class="sxs-lookup"><span data-stu-id="7be49-126">The identifier of the decision.</span></span> |
| <span data-ttu-id="7be49-127">accessReviewId</span><span class="sxs-lookup"><span data-stu-id="7be49-127">accessReviewId</span></span> | <span data-ttu-id="7be49-128">String</span><span class="sxs-lookup"><span data-stu-id="7be49-128">String</span></span> | <span data-ttu-id="7be49-129">O identificador do pai accessReviewInstance.</span><span class="sxs-lookup"><span data-stu-id="7be49-129">The identifier of the accessReviewInstance parent.</span></span> |
| <span data-ttu-id="7be49-130">reviewedBy</span><span class="sxs-lookup"><span data-stu-id="7be49-130">reviewedBy</span></span> | [<span data-ttu-id="7be49-131">userIdentity</span><span class="sxs-lookup"><span data-stu-id="7be49-131">userIdentity</span></span>](useridentity.md) | <span data-ttu-id="7be49-132">O identificador do revistor.</span><span class="sxs-lookup"><span data-stu-id="7be49-132">The identifier of the reviewer.</span></span> |
| <span data-ttu-id="7be49-133">reviewedDateTime</span><span class="sxs-lookup"><span data-stu-id="7be49-133">reviewedDateTime</span></span> | <span data-ttu-id="7be49-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7be49-134">DateTimeOffset</span></span> | <span data-ttu-id="7be49-135">DateTime quando a revisão ocorreu.</span><span class="sxs-lookup"><span data-stu-id="7be49-135">The DateTime when the review occurred.</span></span> |
| <span data-ttu-id="7be49-136">decision</span><span class="sxs-lookup"><span data-stu-id="7be49-136">decision</span></span> | <span data-ttu-id="7be49-137">String</span><span class="sxs-lookup"><span data-stu-id="7be49-137">String</span></span> | <span data-ttu-id="7be49-138">Resultado da revisão.</span><span class="sxs-lookup"><span data-stu-id="7be49-138">Result of the review.</span></span> <span data-ttu-id="7be49-139">Valores possíveis: `Approve` `Deny` , , ou `NotReviewed` `DontKnow` .</span><span class="sxs-lookup"><span data-stu-id="7be49-139">Possible values: `Approve`, `Deny`, `NotReviewed`, or `DontKnow`.</span></span> |
| <span data-ttu-id="7be49-140">justification</span><span class="sxs-lookup"><span data-stu-id="7be49-140">justification</span></span> | <span data-ttu-id="7be49-141">String</span><span class="sxs-lookup"><span data-stu-id="7be49-141">String</span></span> | <span data-ttu-id="7be49-142">A justificativa da decisão de revisão.</span><span class="sxs-lookup"><span data-stu-id="7be49-142">The review decision justification.</span></span> |
| <span data-ttu-id="7be49-143">appliedBy</span><span class="sxs-lookup"><span data-stu-id="7be49-143">appliedBy</span></span> | [<span data-ttu-id="7be49-144">userIdentity</span><span class="sxs-lookup"><span data-stu-id="7be49-144">userIdentity</span></span>](useridentity.md) | <span data-ttu-id="7be49-145">O identificador do usuário que aplicou a decisão.</span><span class="sxs-lookup"><span data-stu-id="7be49-145">The identifier of the user who applied the decision.</span></span> |
| <span data-ttu-id="7be49-146">appliedDateTime</span><span class="sxs-lookup"><span data-stu-id="7be49-146">appliedDateTime</span></span> | <span data-ttu-id="7be49-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7be49-147">DateTimeOffset</span></span> | <span data-ttu-id="7be49-148">DateTime quando a decisão de aprovação foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="7be49-148">The DateTime when the approval decision was applied.</span></span> |
| <span data-ttu-id="7be49-149">applyResult</span><span class="sxs-lookup"><span data-stu-id="7be49-149">applyResult</span></span> | <span data-ttu-id="7be49-150">String</span><span class="sxs-lookup"><span data-stu-id="7be49-150">String</span></span> | <span data-ttu-id="7be49-151">O resultado da aplicação da decisão.</span><span class="sxs-lookup"><span data-stu-id="7be49-151">The result of applying the decision.</span></span> <span data-ttu-id="7be49-152">Valores possíveis: `NotApplied` , , , ou `Success` `Failed` `NotFound` `NotSupported` .</span><span class="sxs-lookup"><span data-stu-id="7be49-152">Possible values: `NotApplied`, `Success`, `Failed`, `NotFound`, or `NotSupported`.</span></span> |
| <span data-ttu-id="7be49-153">recommendation</span><span class="sxs-lookup"><span data-stu-id="7be49-153">recommendation</span></span> | <span data-ttu-id="7be49-154">String</span><span class="sxs-lookup"><span data-stu-id="7be49-154">String</span></span> | <span data-ttu-id="7be49-155">Uma recomendação gerada pelo sistema para a decisão de aprovação.</span><span class="sxs-lookup"><span data-stu-id="7be49-155">A system-generated recommendation for the approval decision.</span></span> <span data-ttu-id="7be49-156">Valores possíveis: `Approve` `Deny` , ou `NotAvailable` .</span><span class="sxs-lookup"><span data-stu-id="7be49-156">Possible values: `Approve`, `Deny`, or `NotAvailable`.</span></span>  |
| <span data-ttu-id="7be49-157">destino</span><span class="sxs-lookup"><span data-stu-id="7be49-157">target</span></span> | [<span data-ttu-id="7be49-158">accessReviewInstanceDecisionItemTarget</span><span class="sxs-lookup"><span data-stu-id="7be49-158">accessReviewInstanceDecisionItemTarget</span></span>](accessreviewinstancedecisionitemtarget.md)  | <span data-ttu-id="7be49-159">O destino dessa decisão específica.</span><span class="sxs-lookup"><span data-stu-id="7be49-159">The target of this specific decision.</span></span> <span data-ttu-id="7be49-160">Os destinos de decisão podem ser de tipos diferentes– cada um com suas próprias propriedades específicas.</span><span class="sxs-lookup"><span data-stu-id="7be49-160">Decision targets can be of different types – each one with its own specific properties.</span></span> <span data-ttu-id="7be49-161">Consulte [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md).</span><span class="sxs-lookup"><span data-stu-id="7be49-161">See [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md).</span></span> |

## <a name="relationships"></a><span data-ttu-id="7be49-162">Relações</span><span class="sxs-lookup"><span data-stu-id="7be49-162">Relationships</span></span>

| <span data-ttu-id="7be49-163">Relação</span><span class="sxs-lookup"><span data-stu-id="7be49-163">Relationship</span></span> | <span data-ttu-id="7be49-164">Tipo</span><span class="sxs-lookup"><span data-stu-id="7be49-164">Type</span></span>   |<span data-ttu-id="7be49-165">Descrição</span><span class="sxs-lookup"><span data-stu-id="7be49-165">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7be49-166">instância</span><span class="sxs-lookup"><span data-stu-id="7be49-166">instance</span></span> |[<span data-ttu-id="7be49-167">accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="7be49-167">accessReviewInstance</span></span>](accessreviewinstance.md) | <span data-ttu-id="7be49-168">Há exatamente um accessReviewInstance associado a cada decisão.</span><span class="sxs-lookup"><span data-stu-id="7be49-168">There is exactly one accessReviewInstance associated with each decision.</span></span> <span data-ttu-id="7be49-169">A instância é o pai do item de decisão, representando a recorrência da revisão de acesso em que a decisão é tomada.</span><span class="sxs-lookup"><span data-stu-id="7be49-169">The instance is the parent of the decision item, representing the recurrence of the access review the decision is made on.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="7be49-170">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7be49-170">JSON representation</span></span>

<span data-ttu-id="7be49-171">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7be49-171">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItem",
  "openType": true
}
-->

```json
{
 "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItem",
 "id": "string (identifier)",
 "accessReviewId": "string",
 "reviewedBy": {
    "@odata.type": "microsoft.graph.userIdentity"
 },
 "reviewedDateTime": "string (timestamp)",
 "decision": "string",
 "justification": "string",
 "appliedBy": {
    "@odata.type": "microsoft.graph.userIdentity"
  },
 "appliedDateTime": "DateTimeOffset",
 "applyResult": "string",
 "recommendation": "string",
 "target": {
    "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemTarget"
  }
}
```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewInstanceDecisionItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
