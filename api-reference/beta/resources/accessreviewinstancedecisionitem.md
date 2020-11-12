---
title: tipo de recurso accessReviewInstanceDecisionItem
description: Representa uma decisão sobre o acesso de um usuário em um accessReviewInstance.
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d9ad5f8a49d44c82f1a43a1666f08f2b49853395
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000779"
---
# <a name="accessreviewinstancedecisionitem-resource-type"></a><span data-ttu-id="fbc59-103">tipo de recurso accessReviewInstanceDecisionItem</span><span class="sxs-lookup"><span data-stu-id="fbc59-103">accessReviewInstanceDecisionItem resource type</span></span>

<span data-ttu-id="fbc59-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fbc59-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fbc59-105">Representa uma decisão de [revisão](accessreviewsv2-root.md) do Azure ad Access em uma instância de uma revisão.</span><span class="sxs-lookup"><span data-stu-id="fbc59-105">Represents an Azure AD [access review](accessreviewsv2-root.md) decision on an instance of a review.</span></span> <span data-ttu-id="fbc59-106">Essa decisão representa a determinação do acesso de um usuário ou de uma entidade de serviço para uma determinada [instância de análise do Access](accessreviewinstance.md).</span><span class="sxs-lookup"><span data-stu-id="fbc59-106">This decision represents the determination of a user or service principal's access for a given [access review instance](accessreviewinstance.md).</span></span>

## <a name="methods"></a><span data-ttu-id="fbc59-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="fbc59-107">Methods</span></span>

| <span data-ttu-id="fbc59-108">Método</span><span class="sxs-lookup"><span data-stu-id="fbc59-108">Method</span></span> | <span data-ttu-id="fbc59-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="fbc59-109">Return Type</span></span> | <span data-ttu-id="fbc59-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="fbc59-110">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="fbc59-111">Listar accessReviewInstanceDecisionItems</span><span class="sxs-lookup"><span data-stu-id="fbc59-111">List accessReviewInstanceDecisionItems</span></span>](../api/accessreviewinstancedecisionitem-list.md) | <span data-ttu-id="fbc59-112">coleção [accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md)</span><span class="sxs-lookup"><span data-stu-id="fbc59-112">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection</span></span> | <span data-ttu-id="fbc59-113">Lista todos os accessReviewInstanceDecisionItem para um accessReviewInstance específico.</span><span class="sxs-lookup"><span data-stu-id="fbc59-113">Lists every accessReviewInstanceDecisionItem for a specific accessReviewInstance.</span></span> |
|[<span data-ttu-id="fbc59-114">Listar accessReviewInstanceDecisionItems pendente de aprovação</span><span class="sxs-lookup"><span data-stu-id="fbc59-114">List accessReviewInstanceDecisionItems pending approval</span></span>](../api/accessreviewinstancedecisionitem-listpendingapproval.md) | <span data-ttu-id="fbc59-115">coleção [accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) .</span><span class="sxs-lookup"><span data-stu-id="fbc59-115">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection.</span></span> | <span data-ttu-id="fbc59-116">Obtenha todos os accessReviewInstanceDecisionItems atribuídos ao usuário de chamada, para um accessReviewInstance específico.</span><span class="sxs-lookup"><span data-stu-id="fbc59-116">Get all accessReviewInstanceDecisionItems assigned to the calling user, for a specific accessReviewInstance.</span></span> |
|[<span data-ttu-id="fbc59-117">Atualizar accessReviewInstanceDecisionItem</span><span class="sxs-lookup"><span data-stu-id="fbc59-117">Update accessReviewInstanceDecisionItem</span></span>](../api/accessreviewinstancedecisionitem-update.md) | <span data-ttu-id="fbc59-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="fbc59-118">None.</span></span> | <span data-ttu-id="fbc59-119">Para qualquer accessReviewInstanceDecisionItems ao qual o usuário de chamada tenha atribuído um revisor, o usuário de chamada pode gravar uma decisão corrigindo o objeto de decisão.</span><span class="sxs-lookup"><span data-stu-id="fbc59-119">For any accessReviewInstanceDecisionItems that the calling user is assigned a reviewer on, calling user can record a decision by patching the decision object.</span></span> |

## <a name="properties"></a><span data-ttu-id="fbc59-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fbc59-120">Properties</span></span>
| <span data-ttu-id="fbc59-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fbc59-121">Property</span></span> | <span data-ttu-id="fbc59-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="fbc59-122">Type</span></span> |  <span data-ttu-id="fbc59-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="fbc59-123">Description</span></span> |
| :---------------| :---- | :---------- |
| <span data-ttu-id="fbc59-124">id</span><span class="sxs-lookup"><span data-stu-id="fbc59-124">id</span></span> | <span data-ttu-id="fbc59-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fbc59-125">String</span></span> | <span data-ttu-id="fbc59-126">O identificador da decisão.</span><span class="sxs-lookup"><span data-stu-id="fbc59-126">The identifier of the decision.</span></span> |
| <span data-ttu-id="fbc59-127">accessReviewId</span><span class="sxs-lookup"><span data-stu-id="fbc59-127">accessReviewId</span></span> | <span data-ttu-id="fbc59-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fbc59-128">String</span></span> | <span data-ttu-id="fbc59-129">O identificador do accessReviewInstance pai.</span><span class="sxs-lookup"><span data-stu-id="fbc59-129">The identifier of the accessReviewInstance parent.</span></span> |
| <span data-ttu-id="fbc59-130">reviewedBy</span><span class="sxs-lookup"><span data-stu-id="fbc59-130">reviewedBy</span></span> | [<span data-ttu-id="fbc59-131">userIdentity</span><span class="sxs-lookup"><span data-stu-id="fbc59-131">userIdentity</span></span>](useridentity.md) | <span data-ttu-id="fbc59-132">O identificador do revisor.</span><span class="sxs-lookup"><span data-stu-id="fbc59-132">The identifier of the reviewer.</span></span> |
| <span data-ttu-id="fbc59-133">reviewedDateTime</span><span class="sxs-lookup"><span data-stu-id="fbc59-133">reviewedDateTime</span></span> | <span data-ttu-id="fbc59-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbc59-134">DateTimeOffset</span></span> | <span data-ttu-id="fbc59-135">O DateTime quando a revisão ocorreu.</span><span class="sxs-lookup"><span data-stu-id="fbc59-135">The DateTime when the review occurred.</span></span> |
| <span data-ttu-id="fbc59-136">sobre</span><span class="sxs-lookup"><span data-stu-id="fbc59-136">decision</span></span> | <span data-ttu-id="fbc59-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fbc59-137">String</span></span> | <span data-ttu-id="fbc59-138">Resultado da revisão.</span><span class="sxs-lookup"><span data-stu-id="fbc59-138">Result of the review.</span></span> <span data-ttu-id="fbc59-139">Valores possíveis: `Approve` , `Deny` , `NotReviewed` ou `DontKnow` .</span><span class="sxs-lookup"><span data-stu-id="fbc59-139">Possible values: `Approve`, `Deny`, `NotReviewed`, or `DontKnow`.</span></span> |
| <span data-ttu-id="fbc59-140">elabora</span><span class="sxs-lookup"><span data-stu-id="fbc59-140">justification</span></span> | <span data-ttu-id="fbc59-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fbc59-141">String</span></span> | <span data-ttu-id="fbc59-142">A justificativa de decisão de revisão.</span><span class="sxs-lookup"><span data-stu-id="fbc59-142">The review decision justification.</span></span> |
| <span data-ttu-id="fbc59-143">appliedBy</span><span class="sxs-lookup"><span data-stu-id="fbc59-143">appliedBy</span></span> | [<span data-ttu-id="fbc59-144">userIdentity</span><span class="sxs-lookup"><span data-stu-id="fbc59-144">userIdentity</span></span>](useridentity.md) | <span data-ttu-id="fbc59-145">O identificador do usuário que aplicou a decisão.</span><span class="sxs-lookup"><span data-stu-id="fbc59-145">The identifier of the user who applied the decision.</span></span> |
| <span data-ttu-id="fbc59-146">appliedDateTime</span><span class="sxs-lookup"><span data-stu-id="fbc59-146">appliedDateTime</span></span> | <span data-ttu-id="fbc59-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbc59-147">DateTimeOffset</span></span> | <span data-ttu-id="fbc59-148">O DateTime quando a decisão de aprovação foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="fbc59-148">The DateTime when the approval decision was applied.</span></span> |
| <span data-ttu-id="fbc59-149">applyResult</span><span class="sxs-lookup"><span data-stu-id="fbc59-149">applyResult</span></span> | <span data-ttu-id="fbc59-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fbc59-150">String</span></span> | <span data-ttu-id="fbc59-151">O resultado da aplicação da decisão.</span><span class="sxs-lookup"><span data-stu-id="fbc59-151">The result of applying the decision.</span></span> <span data-ttu-id="fbc59-152">Valores possíveis: `NotApplied` , `Success` , `Failed` , `NotFound` , ou `NotSupported` .</span><span class="sxs-lookup"><span data-stu-id="fbc59-152">Possible values: `NotApplied`, `Success`, `Failed`, `NotFound`, or `NotSupported`.</span></span> |
| <span data-ttu-id="fbc59-153">recomendação</span><span class="sxs-lookup"><span data-stu-id="fbc59-153">recommendation</span></span> | <span data-ttu-id="fbc59-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fbc59-154">String</span></span> | <span data-ttu-id="fbc59-155">Uma recomendação gerada pelo sistema para a decisão de aprovação.</span><span class="sxs-lookup"><span data-stu-id="fbc59-155">A system-generated recommendation for the approval decision.</span></span> <span data-ttu-id="fbc59-156">Valores possíveis: `Approve` , `Deny` , ou `NotAvailable` .</span><span class="sxs-lookup"><span data-stu-id="fbc59-156">Possible values: `Approve`, `Deny`, or `NotAvailable`.</span></span>  |
| <span data-ttu-id="fbc59-157">destino</span><span class="sxs-lookup"><span data-stu-id="fbc59-157">target</span></span> | [<span data-ttu-id="fbc59-158">accessReviewInstanceDecisionItemTarget</span><span class="sxs-lookup"><span data-stu-id="fbc59-158">accessReviewInstanceDecisionItemTarget</span></span>](accessreviewinstancedecisionitemtarget.md)  | <span data-ttu-id="fbc59-159">O alvo dessa decisão específica.</span><span class="sxs-lookup"><span data-stu-id="fbc59-159">The target of this specific decision.</span></span> <span data-ttu-id="fbc59-160">Os alvos de decisão podem ser de tipos diferentes, cada um com suas próprias propriedades específicas.</span><span class="sxs-lookup"><span data-stu-id="fbc59-160">Decision targets can be of different types – each one with its own specific properties.</span></span> <span data-ttu-id="fbc59-161">Consulte [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md).</span><span class="sxs-lookup"><span data-stu-id="fbc59-161">See [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md).</span></span> |

## <a name="relationships"></a><span data-ttu-id="fbc59-162">Relações</span><span class="sxs-lookup"><span data-stu-id="fbc59-162">Relationships</span></span>

| <span data-ttu-id="fbc59-163">Relação</span><span class="sxs-lookup"><span data-stu-id="fbc59-163">Relationship</span></span> | <span data-ttu-id="fbc59-164">Tipo</span><span class="sxs-lookup"><span data-stu-id="fbc59-164">Type</span></span>   |<span data-ttu-id="fbc59-165">Descrição</span><span class="sxs-lookup"><span data-stu-id="fbc59-165">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fbc59-166">sessão</span><span class="sxs-lookup"><span data-stu-id="fbc59-166">instance</span></span> |[<span data-ttu-id="fbc59-167">accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="fbc59-167">accessReviewInstance</span></span>](accessreviewinstance.md) | <span data-ttu-id="fbc59-168">Há exatamente um accessReviewInstance associado a cada decisão.</span><span class="sxs-lookup"><span data-stu-id="fbc59-168">There is exactly one accessReviewInstance associated with each decision.</span></span> <span data-ttu-id="fbc59-169">A instância é pai do item de decisão, representando a recorrência da revisão do Access na qual a decisão é realizada.</span><span class="sxs-lookup"><span data-stu-id="fbc59-169">The instance is the parent of the decision item, representing the recurrence of the access review the decision is made on.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="fbc59-170">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fbc59-170">JSON representation</span></span>

<span data-ttu-id="fbc59-171">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fbc59-171">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItem",
  "baseType": "",
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
