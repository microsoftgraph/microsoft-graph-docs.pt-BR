---
title: Tipo de recurso accessReviewInstanceDecisionItem
description: Representa uma decisão sobre o acesso de um usuário em um accessReviewInstance.
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 10166dc9da512bf74a0b4e5ad97f4797cdf6c317
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159196"
---
# <a name="accessreviewinstancedecisionitem-resource-type"></a><span data-ttu-id="a3854-103">Tipo de recurso accessReviewInstanceDecisionItem</span><span class="sxs-lookup"><span data-stu-id="a3854-103">accessReviewInstanceDecisionItem resource type</span></span>

<span data-ttu-id="a3854-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3854-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3854-105">Representa uma decisão de revisão de acesso [do](accessreviewsv2-root.md) Azure AD em uma instância de uma análise.</span><span class="sxs-lookup"><span data-stu-id="a3854-105">Represents an Azure AD [access review](accessreviewsv2-root.md) decision on an instance of a review.</span></span> <span data-ttu-id="a3854-106">Essa decisão representa a determinação do acesso de um usuário ou entidade de serviço para uma determinada [instância de revisão de acesso.](accessreviewinstance.md)</span><span class="sxs-lookup"><span data-stu-id="a3854-106">This decision represents the determination of a user or service principal's access for a given [access review instance](accessreviewinstance.md).</span></span>

## <a name="methods"></a><span data-ttu-id="a3854-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="a3854-107">Methods</span></span>

| <span data-ttu-id="a3854-108">Método</span><span class="sxs-lookup"><span data-stu-id="a3854-108">Method</span></span> | <span data-ttu-id="a3854-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a3854-109">Return Type</span></span> | <span data-ttu-id="a3854-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3854-110">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="a3854-111">Listar accessReviewInstanceDecisionItems</span><span class="sxs-lookup"><span data-stu-id="a3854-111">List accessReviewInstanceDecisionItems</span></span>](../api/accessreviewinstancedecisionitem-list.md) | <span data-ttu-id="a3854-112">[Coleção accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md)</span><span class="sxs-lookup"><span data-stu-id="a3854-112">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection</span></span> | <span data-ttu-id="a3854-113">Lista cada accessReviewInstanceDecisionItem para um accessReviewInstance específico.</span><span class="sxs-lookup"><span data-stu-id="a3854-113">Lists every accessReviewInstanceDecisionItem for a specific accessReviewInstance.</span></span> |
|[<span data-ttu-id="a3854-114">Listar aprovação pendente de accessReviewInstanceDecisionItems</span><span class="sxs-lookup"><span data-stu-id="a3854-114">List accessReviewInstanceDecisionItems pending approval</span></span>](../api/accessreviewinstancedecisionitem-listpendingapproval.md) | <span data-ttu-id="a3854-115">[coleção accessReviewInstanceDecisionItem.](accessreviewinstancedecisionitem.md)</span><span class="sxs-lookup"><span data-stu-id="a3854-115">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection.</span></span> | <span data-ttu-id="a3854-116">Obter todos os accessReviewInstanceDecisionItems atribuídos ao usuário de chamada, para um accessReviewInstance específico.</span><span class="sxs-lookup"><span data-stu-id="a3854-116">Get all accessReviewInstanceDecisionItems assigned to the calling user, for a specific accessReviewInstance.</span></span> |
|[<span data-ttu-id="a3854-117">Atualizar accessReviewInstanceDecisionItem</span><span class="sxs-lookup"><span data-stu-id="a3854-117">Update accessReviewInstanceDecisionItem</span></span>](../api/accessreviewinstancedecisionitem-update.md) | <span data-ttu-id="a3854-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a3854-118">None.</span></span> | <span data-ttu-id="a3854-119">Para qualquer accessReviewInstanceDecisionItems em que o usuário de chamada é atribuído a um revisor, chamar o usuário pode registrar uma decisão, corrigindo o objeto de decisão.</span><span class="sxs-lookup"><span data-stu-id="a3854-119">For any accessReviewInstanceDecisionItems that the calling user is assigned a reviewer on, calling user can record a decision by patching the decision object.</span></span> |

## <a name="properties"></a><span data-ttu-id="a3854-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a3854-120">Properties</span></span>
| <span data-ttu-id="a3854-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a3854-121">Property</span></span> | <span data-ttu-id="a3854-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="a3854-122">Type</span></span> |  <span data-ttu-id="a3854-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3854-123">Description</span></span> |
| :---------------| :---- | :---------- |
| <span data-ttu-id="a3854-124">id</span><span class="sxs-lookup"><span data-stu-id="a3854-124">id</span></span> | <span data-ttu-id="a3854-125">String</span><span class="sxs-lookup"><span data-stu-id="a3854-125">String</span></span> | <span data-ttu-id="a3854-126">O identificador da decisão.</span><span class="sxs-lookup"><span data-stu-id="a3854-126">The identifier of the decision.</span></span> |
| <span data-ttu-id="a3854-127">accessReviewId</span><span class="sxs-lookup"><span data-stu-id="a3854-127">accessReviewId</span></span> | <span data-ttu-id="a3854-128">String</span><span class="sxs-lookup"><span data-stu-id="a3854-128">String</span></span> | <span data-ttu-id="a3854-129">O identificador do accessReviewInstance pai.</span><span class="sxs-lookup"><span data-stu-id="a3854-129">The identifier of the accessReviewInstance parent.</span></span> |
| <span data-ttu-id="a3854-130">reviewedBy</span><span class="sxs-lookup"><span data-stu-id="a3854-130">reviewedBy</span></span> | [<span data-ttu-id="a3854-131">userIdentity</span><span class="sxs-lookup"><span data-stu-id="a3854-131">userIdentity</span></span>](useridentity.md) | <span data-ttu-id="a3854-132">O identificador do revistor.</span><span class="sxs-lookup"><span data-stu-id="a3854-132">The identifier of the reviewer.</span></span> |
| <span data-ttu-id="a3854-133">reviewedDateTime</span><span class="sxs-lookup"><span data-stu-id="a3854-133">reviewedDateTime</span></span> | <span data-ttu-id="a3854-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3854-134">DateTimeOffset</span></span> | <span data-ttu-id="a3854-135">DateTime em que a revisão ocorreu.</span><span class="sxs-lookup"><span data-stu-id="a3854-135">The DateTime when the review occurred.</span></span> |
| <span data-ttu-id="a3854-136">decision</span><span class="sxs-lookup"><span data-stu-id="a3854-136">decision</span></span> | <span data-ttu-id="a3854-137">String</span><span class="sxs-lookup"><span data-stu-id="a3854-137">String</span></span> | <span data-ttu-id="a3854-138">Resultado da revisão.</span><span class="sxs-lookup"><span data-stu-id="a3854-138">Result of the review.</span></span> <span data-ttu-id="a3854-139">Valores possíveis: `Approve` `Deny` , , ou `NotReviewed` `DontKnow` .</span><span class="sxs-lookup"><span data-stu-id="a3854-139">Possible values: `Approve`, `Deny`, `NotReviewed`, or `DontKnow`.</span></span> |
| <span data-ttu-id="a3854-140">justification</span><span class="sxs-lookup"><span data-stu-id="a3854-140">justification</span></span> | <span data-ttu-id="a3854-141">String</span><span class="sxs-lookup"><span data-stu-id="a3854-141">String</span></span> | <span data-ttu-id="a3854-142">A justificativa da decisão de revisão.</span><span class="sxs-lookup"><span data-stu-id="a3854-142">The review decision justification.</span></span> |
| <span data-ttu-id="a3854-143">appliedBy</span><span class="sxs-lookup"><span data-stu-id="a3854-143">appliedBy</span></span> | [<span data-ttu-id="a3854-144">userIdentity</span><span class="sxs-lookup"><span data-stu-id="a3854-144">userIdentity</span></span>](useridentity.md) | <span data-ttu-id="a3854-145">O identificador do usuário que aplicou a decisão.</span><span class="sxs-lookup"><span data-stu-id="a3854-145">The identifier of the user who applied the decision.</span></span> |
| <span data-ttu-id="a3854-146">appliedDateTime</span><span class="sxs-lookup"><span data-stu-id="a3854-146">appliedDateTime</span></span> | <span data-ttu-id="a3854-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3854-147">DateTimeOffset</span></span> | <span data-ttu-id="a3854-148">DateTime em que a decisão de aprovação foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="a3854-148">The DateTime when the approval decision was applied.</span></span> |
| <span data-ttu-id="a3854-149">applyResult</span><span class="sxs-lookup"><span data-stu-id="a3854-149">applyResult</span></span> | <span data-ttu-id="a3854-150">String</span><span class="sxs-lookup"><span data-stu-id="a3854-150">String</span></span> | <span data-ttu-id="a3854-151">O resultado da aplicação da decisão.</span><span class="sxs-lookup"><span data-stu-id="a3854-151">The result of applying the decision.</span></span> <span data-ttu-id="a3854-152">Valores possíveis: `NotApplied` , , , ou `Success` `Failed` `NotFound` `NotSupported` .</span><span class="sxs-lookup"><span data-stu-id="a3854-152">Possible values: `NotApplied`, `Success`, `Failed`, `NotFound`, or `NotSupported`.</span></span> |
| <span data-ttu-id="a3854-153">recomendação</span><span class="sxs-lookup"><span data-stu-id="a3854-153">recommendation</span></span> | <span data-ttu-id="a3854-154">String</span><span class="sxs-lookup"><span data-stu-id="a3854-154">String</span></span> | <span data-ttu-id="a3854-155">Uma recomendação gerada pelo sistema para a decisão de aprovação.</span><span class="sxs-lookup"><span data-stu-id="a3854-155">A system-generated recommendation for the approval decision.</span></span> <span data-ttu-id="a3854-156">Valores possíveis: `Approve` `Deny` , ou `NotAvailable` .</span><span class="sxs-lookup"><span data-stu-id="a3854-156">Possible values: `Approve`, `Deny`, or `NotAvailable`.</span></span>  |
| <span data-ttu-id="a3854-157">destino</span><span class="sxs-lookup"><span data-stu-id="a3854-157">target</span></span> | [<span data-ttu-id="a3854-158">accessReviewInstanceDecisionItemTarget</span><span class="sxs-lookup"><span data-stu-id="a3854-158">accessReviewInstanceDecisionItemTarget</span></span>](accessreviewinstancedecisionitemtarget.md)  | <span data-ttu-id="a3854-159">O destino dessa decisão específica.</span><span class="sxs-lookup"><span data-stu-id="a3854-159">The target of this specific decision.</span></span> <span data-ttu-id="a3854-160">Os destinos de decisão podem ser de tipos diferentes, cada um com suas próprias propriedades específicas.</span><span class="sxs-lookup"><span data-stu-id="a3854-160">Decision targets can be of different types – each one with its own specific properties.</span></span> <span data-ttu-id="a3854-161">Consulte [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md).</span><span class="sxs-lookup"><span data-stu-id="a3854-161">See [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md).</span></span> |

## <a name="relationships"></a><span data-ttu-id="a3854-162">Relações</span><span class="sxs-lookup"><span data-stu-id="a3854-162">Relationships</span></span>

| <span data-ttu-id="a3854-163">Relação</span><span class="sxs-lookup"><span data-stu-id="a3854-163">Relationship</span></span> | <span data-ttu-id="a3854-164">Tipo</span><span class="sxs-lookup"><span data-stu-id="a3854-164">Type</span></span>   |<span data-ttu-id="a3854-165">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3854-165">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a3854-166">instância</span><span class="sxs-lookup"><span data-stu-id="a3854-166">instance</span></span> |[<span data-ttu-id="a3854-167">accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="a3854-167">accessReviewInstance</span></span>](accessreviewinstance.md) | <span data-ttu-id="a3854-168">Há exatamente um accessReviewInstance associado a cada decisão.</span><span class="sxs-lookup"><span data-stu-id="a3854-168">There is exactly one accessReviewInstance associated with each decision.</span></span> <span data-ttu-id="a3854-169">A instância é o pai do item de decisão, representando a recorrência da revisão de acesso em que a decisão foi tomada.</span><span class="sxs-lookup"><span data-stu-id="a3854-169">The instance is the parent of the decision item, representing the recurrence of the access review the decision is made on.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="a3854-170">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a3854-170">JSON representation</span></span>

<span data-ttu-id="a3854-171">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a3854-171">Here is a JSON representation of the resource.</span></span>

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
