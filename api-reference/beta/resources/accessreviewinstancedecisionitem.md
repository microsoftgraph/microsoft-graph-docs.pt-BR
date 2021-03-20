---
title: Tipo de recurso accessReviewInstanceDecisionItem
description: Representa uma decisão sobre o acesso de um usuário em um accessReviewInstance.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: e5d9b64faafb7dfe4ec4e6f3487643e62885236a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952807"
---
# <a name="accessreviewinstancedecisionitem-resource-type"></a><span data-ttu-id="1df1b-103">Tipo de recurso accessReviewInstanceDecisionItem</span><span class="sxs-lookup"><span data-stu-id="1df1b-103">accessReviewInstanceDecisionItem resource type</span></span>

<span data-ttu-id="1df1b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1df1b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="1df1b-105">Representa uma decisão de revisão [de](accessreviewsv2-root.md) acesso do Azure AD em uma instância de uma revisão.</span><span class="sxs-lookup"><span data-stu-id="1df1b-105">Represents an Azure AD [access review](accessreviewsv2-root.md) decision on an instance of a review.</span></span> <span data-ttu-id="1df1b-106">Essa decisão representa a determinação do acesso de um usuário ou entidade de serviço para uma determinada instância de revisão [de acesso.](accessreviewinstance.md)</span><span class="sxs-lookup"><span data-stu-id="1df1b-106">This decision represents the determination of a user or service principal's access for a given [access review instance](accessreviewinstance.md).</span></span>

## <a name="methods"></a><span data-ttu-id="1df1b-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="1df1b-107">Methods</span></span>

| <span data-ttu-id="1df1b-108">Método</span><span class="sxs-lookup"><span data-stu-id="1df1b-108">Method</span></span> | <span data-ttu-id="1df1b-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1df1b-109">Return Type</span></span> | <span data-ttu-id="1df1b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1df1b-110">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="1df1b-111">Listar accessReviewInstanceDecisionItems</span><span class="sxs-lookup"><span data-stu-id="1df1b-111">List accessReviewInstanceDecisionItems</span></span>](../api/accessreviewinstancedecisionitem-list.md) | <span data-ttu-id="1df1b-112">[Coleção accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md)</span><span class="sxs-lookup"><span data-stu-id="1df1b-112">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection</span></span> | <span data-ttu-id="1df1b-113">Lista cada accessReviewInstanceDecisionItem para um accessReviewInstance específico.</span><span class="sxs-lookup"><span data-stu-id="1df1b-113">Lists every accessReviewInstanceDecisionItem for a specific accessReviewInstance.</span></span> |
|[<span data-ttu-id="1df1b-114">Listar accessReviewInstanceDecisionItems aguardando aprovação</span><span class="sxs-lookup"><span data-stu-id="1df1b-114">List accessReviewInstanceDecisionItems pending approval</span></span>](../api/accessreviewinstancedecisionitem-listpendingapproval.md) | <span data-ttu-id="1df1b-115">[Coleção accessReviewInstanceDecisionItem.](accessreviewinstancedecisionitem.md)</span><span class="sxs-lookup"><span data-stu-id="1df1b-115">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection.</span></span> | <span data-ttu-id="1df1b-116">Obter todos os accessReviewInstanceDecisionItems atribuídos ao usuário de chamada, para um accessReviewInstance específico.</span><span class="sxs-lookup"><span data-stu-id="1df1b-116">Get all accessReviewInstanceDecisionItems assigned to the calling user, for a specific accessReviewInstance.</span></span> |
|[<span data-ttu-id="1df1b-117">Atualizar accessReviewInstanceDecisionItem</span><span class="sxs-lookup"><span data-stu-id="1df1b-117">Update accessReviewInstanceDecisionItem</span></span>](../api/accessreviewinstancedecisionitem-update.md) | <span data-ttu-id="1df1b-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1df1b-118">None.</span></span> | <span data-ttu-id="1df1b-119">Para qualquer accessReviewInstanceDecisionItems em que o usuário de chamada recebe um revisor, chamar o usuário pode registrar uma decisão corrigindo o objeto decision.</span><span class="sxs-lookup"><span data-stu-id="1df1b-119">For any accessReviewInstanceDecisionItems that the calling user is assigned a reviewer on, calling user can record a decision by patching the decision object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1df1b-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1df1b-120">Properties</span></span>
| <span data-ttu-id="1df1b-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1df1b-121">Property</span></span> | <span data-ttu-id="1df1b-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="1df1b-122">Type</span></span> |  <span data-ttu-id="1df1b-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="1df1b-123">Description</span></span> |
| :---------------| :---- | :---------- |
| <span data-ttu-id="1df1b-124">id</span><span class="sxs-lookup"><span data-stu-id="1df1b-124">id</span></span> | <span data-ttu-id="1df1b-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1df1b-125">String</span></span> | <span data-ttu-id="1df1b-126">O identificador da decisão.</span><span class="sxs-lookup"><span data-stu-id="1df1b-126">The identifier of the decision.</span></span> |
| <span data-ttu-id="1df1b-127">accessReviewId</span><span class="sxs-lookup"><span data-stu-id="1df1b-127">accessReviewId</span></span> | <span data-ttu-id="1df1b-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1df1b-128">String</span></span> | <span data-ttu-id="1df1b-129">O identificador do pai accessReviewInstance.</span><span class="sxs-lookup"><span data-stu-id="1df1b-129">The identifier of the accessReviewInstance parent.</span></span> |
| <span data-ttu-id="1df1b-130">reviewedBy</span><span class="sxs-lookup"><span data-stu-id="1df1b-130">reviewedBy</span></span> | [<span data-ttu-id="1df1b-131">userIdentity</span><span class="sxs-lookup"><span data-stu-id="1df1b-131">userIdentity</span></span>](useridentity.md) | <span data-ttu-id="1df1b-132">O identificador do revistor.</span><span class="sxs-lookup"><span data-stu-id="1df1b-132">The identifier of the reviewer.</span></span> |
| <span data-ttu-id="1df1b-133">reviewedDateTime</span><span class="sxs-lookup"><span data-stu-id="1df1b-133">reviewedDateTime</span></span> | <span data-ttu-id="1df1b-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1df1b-134">DateTimeOffset</span></span> | <span data-ttu-id="1df1b-135">O timestamp quando a revisão ocorreu.</span><span class="sxs-lookup"><span data-stu-id="1df1b-135">The timestamp when the review occurred.</span></span> |
| <span data-ttu-id="1df1b-136">decision</span><span class="sxs-lookup"><span data-stu-id="1df1b-136">decision</span></span> | <span data-ttu-id="1df1b-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1df1b-137">String</span></span> | <span data-ttu-id="1df1b-138">Resultado da revisão.</span><span class="sxs-lookup"><span data-stu-id="1df1b-138">Result of the review.</span></span> <span data-ttu-id="1df1b-139">Valores possíveis: `Approve` `Deny` , , ou `NotReviewed` `DontKnow` .</span><span class="sxs-lookup"><span data-stu-id="1df1b-139">Possible values: `Approve`, `Deny`, `NotReviewed`, or `DontKnow`.</span></span> |
| <span data-ttu-id="1df1b-140">justification</span><span class="sxs-lookup"><span data-stu-id="1df1b-140">justification</span></span> | <span data-ttu-id="1df1b-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1df1b-141">String</span></span> | <span data-ttu-id="1df1b-142">A justificativa da decisão de revisão.</span><span class="sxs-lookup"><span data-stu-id="1df1b-142">The review decision justification.</span></span> |
| <span data-ttu-id="1df1b-143">appliedBy</span><span class="sxs-lookup"><span data-stu-id="1df1b-143">appliedBy</span></span> | [<span data-ttu-id="1df1b-144">userIdentity</span><span class="sxs-lookup"><span data-stu-id="1df1b-144">userIdentity</span></span>](useridentity.md) | <span data-ttu-id="1df1b-145">O identificador do usuário que aplicou a decisão.</span><span class="sxs-lookup"><span data-stu-id="1df1b-145">The identifier of the user who applied the decision.</span></span> |
| <span data-ttu-id="1df1b-146">appliedDateTime</span><span class="sxs-lookup"><span data-stu-id="1df1b-146">appliedDateTime</span></span> | <span data-ttu-id="1df1b-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1df1b-147">DateTimeOffset</span></span> | <span data-ttu-id="1df1b-148">O timestamp quando a decisão de aprovação foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="1df1b-148">The timestamp when the approval decision was applied.</span></span> <span data-ttu-id="1df1b-149">O tipo DatetimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre em horário UTC.</span><span class="sxs-lookup"><span data-stu-id="1df1b-149">The DatetimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1df1b-150">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="1df1b-150">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
| <span data-ttu-id="1df1b-151">applyResult</span><span class="sxs-lookup"><span data-stu-id="1df1b-151">applyResult</span></span> | <span data-ttu-id="1df1b-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1df1b-152">String</span></span> | <span data-ttu-id="1df1b-153">O resultado da aplicação da decisão.</span><span class="sxs-lookup"><span data-stu-id="1df1b-153">The result of applying the decision.</span></span> <span data-ttu-id="1df1b-154">Valores possíveis: `NotApplied` , , , ou `Success` `Failed` `NotFound` `NotSupported` .</span><span class="sxs-lookup"><span data-stu-id="1df1b-154">Possible values: `NotApplied`, `Success`, `Failed`, `NotFound`, or `NotSupported`.</span></span> |
| <span data-ttu-id="1df1b-155">recommendation</span><span class="sxs-lookup"><span data-stu-id="1df1b-155">recommendation</span></span> | <span data-ttu-id="1df1b-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1df1b-156">String</span></span> | <span data-ttu-id="1df1b-157">Uma recomendação gerada pelo sistema para a decisão de aprovação.</span><span class="sxs-lookup"><span data-stu-id="1df1b-157">A system-generated recommendation for the approval decision.</span></span> <span data-ttu-id="1df1b-158">Valores possíveis: `Approve` `Deny` , ou `NotAvailable` .</span><span class="sxs-lookup"><span data-stu-id="1df1b-158">Possible values: `Approve`, `Deny`, or `NotAvailable`.</span></span>  |
| <span data-ttu-id="1df1b-159">destino</span><span class="sxs-lookup"><span data-stu-id="1df1b-159">target</span></span> | [<span data-ttu-id="1df1b-160">accessReviewInstanceDecisionItemTarget</span><span class="sxs-lookup"><span data-stu-id="1df1b-160">accessReviewInstanceDecisionItemTarget</span></span>](accessreviewinstancedecisionitemtarget.md)  | <span data-ttu-id="1df1b-161">O destino dessa decisão específica.</span><span class="sxs-lookup"><span data-stu-id="1df1b-161">The target of this specific decision.</span></span> <span data-ttu-id="1df1b-162">Os destinos de decisão podem ser de tipos diferentes– cada um com suas próprias propriedades específicas.</span><span class="sxs-lookup"><span data-stu-id="1df1b-162">Decision targets can be of different types – each one with its own specific properties.</span></span> <span data-ttu-id="1df1b-163">Consulte [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md).</span><span class="sxs-lookup"><span data-stu-id="1df1b-163">See [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md).</span></span> |

## <a name="relationships"></a><span data-ttu-id="1df1b-164">Relações</span><span class="sxs-lookup"><span data-stu-id="1df1b-164">Relationships</span></span>

| <span data-ttu-id="1df1b-165">Relação</span><span class="sxs-lookup"><span data-stu-id="1df1b-165">Relationship</span></span> | <span data-ttu-id="1df1b-166">Tipo</span><span class="sxs-lookup"><span data-stu-id="1df1b-166">Type</span></span>   |<span data-ttu-id="1df1b-167">Descrição</span><span class="sxs-lookup"><span data-stu-id="1df1b-167">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1df1b-168">instância</span><span class="sxs-lookup"><span data-stu-id="1df1b-168">instance</span></span> |[<span data-ttu-id="1df1b-169">accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="1df1b-169">accessReviewInstance</span></span>](accessreviewinstance.md) | <span data-ttu-id="1df1b-170">Há exatamente um accessReviewInstance associado a cada decisão.</span><span class="sxs-lookup"><span data-stu-id="1df1b-170">There is exactly one accessReviewInstance associated with each decision.</span></span> <span data-ttu-id="1df1b-171">A instância é o pai do item de decisão, representando a recorrência da revisão de acesso em que a decisão é tomada.</span><span class="sxs-lookup"><span data-stu-id="1df1b-171">The instance is the parent of the decision item, representing the recurrence of the access review the decision is made on.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="1df1b-172">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1df1b-172">JSON representation</span></span>

<span data-ttu-id="1df1b-173">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1df1b-173">Here is a JSON representation of the resource.</span></span>

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
