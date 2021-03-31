---
title: Tipo de recurso accessReviewInstanceDecisionItem
description: Representa uma decisão sobre o acesso de um usuário em um accessReviewInstance.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 968af49a9033ea749522132204d63b4f55ba25c7
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469238"
---
# <a name="accessreviewinstancedecisionitem-resource-type"></a><span data-ttu-id="f26c5-103">Tipo de recurso accessReviewInstanceDecisionItem</span><span class="sxs-lookup"><span data-stu-id="f26c5-103">accessReviewInstanceDecisionItem resource type</span></span>

<span data-ttu-id="f26c5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f26c5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

>[!NOTE]
><span data-ttu-id="f26c5-105">A propriedade `target` será preterida em v1.0 e substituída por propriedades `principal` e `resource` .</span><span class="sxs-lookup"><span data-stu-id="f26c5-105">The property `target` will be deprecated in v1.0 and replaced by properties `principal` and `resource`.</span></span>

<span data-ttu-id="f26c5-106">Representa uma decisão de revisão [de](accessreviewsv2-root.md) acesso do Azure AD em uma instância de uma revisão.</span><span class="sxs-lookup"><span data-stu-id="f26c5-106">Represents an Azure AD [access review](accessreviewsv2-root.md) decision on an instance of a review.</span></span> <span data-ttu-id="f26c5-107">Essa decisão representa a determinação do acesso de um usuário ou entidade de serviço para uma determinada instância de revisão [de acesso.](accessreviewinstance.md)</span><span class="sxs-lookup"><span data-stu-id="f26c5-107">This decision represents the determination of a user or service principal's access for a given [access review instance](accessreviewinstance.md).</span></span>

## <a name="methods"></a><span data-ttu-id="f26c5-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="f26c5-108">Methods</span></span>

| <span data-ttu-id="f26c5-109">Método</span><span class="sxs-lookup"><span data-stu-id="f26c5-109">Method</span></span> | <span data-ttu-id="f26c5-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f26c5-110">Return Type</span></span> | <span data-ttu-id="f26c5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f26c5-111">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="f26c5-112">Listar accessReviewInstanceDecisionItems</span><span class="sxs-lookup"><span data-stu-id="f26c5-112">List accessReviewInstanceDecisionItems</span></span>](../api/accessreviewinstancedecisionitem-list.md) | <span data-ttu-id="f26c5-113">[Coleção accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md)</span><span class="sxs-lookup"><span data-stu-id="f26c5-113">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection</span></span> | <span data-ttu-id="f26c5-114">Lista cada accessReviewInstanceDecisionItem para um accessReviewInstance específico.</span><span class="sxs-lookup"><span data-stu-id="f26c5-114">Lists every accessReviewInstanceDecisionItem for a specific accessReviewInstance.</span></span> |
|[<span data-ttu-id="f26c5-115">Listar accessReviewInstanceDecisionItems aguardando aprovação</span><span class="sxs-lookup"><span data-stu-id="f26c5-115">List accessReviewInstanceDecisionItems pending approval</span></span>](../api/accessreviewinstancedecisionitem-listpendingapproval.md) | <span data-ttu-id="f26c5-116">[Coleção accessReviewInstanceDecisionItem.](accessreviewinstancedecisionitem.md)</span><span class="sxs-lookup"><span data-stu-id="f26c5-116">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection.</span></span> | <span data-ttu-id="f26c5-117">Obter todos os accessReviewInstanceDecisionItems atribuídos ao usuário de chamada, para um accessReviewInstance específico.</span><span class="sxs-lookup"><span data-stu-id="f26c5-117">Get all accessReviewInstanceDecisionItems assigned to the calling user, for a specific accessReviewInstance.</span></span> |
|[<span data-ttu-id="f26c5-118">Atualizar accessReviewInstanceDecisionItem</span><span class="sxs-lookup"><span data-stu-id="f26c5-118">Update accessReviewInstanceDecisionItem</span></span>](../api/accessreviewinstancedecisionitem-update.md) | <span data-ttu-id="f26c5-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f26c5-119">None.</span></span> | <span data-ttu-id="f26c5-120">Para qualquer accessReviewInstanceDecisionItems em que o usuário de chamada recebe um revisor, chamar o usuário pode registrar uma decisão corrigindo o objeto decision.</span><span class="sxs-lookup"><span data-stu-id="f26c5-120">For any accessReviewInstanceDecisionItems that the calling user is assigned a reviewer on, calling user can record a decision by patching the decision object.</span></span> |

## <a name="properties"></a><span data-ttu-id="f26c5-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f26c5-121">Properties</span></span>
| <span data-ttu-id="f26c5-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f26c5-122">Property</span></span> | <span data-ttu-id="f26c5-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="f26c5-123">Type</span></span> |  <span data-ttu-id="f26c5-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="f26c5-124">Description</span></span> |
| :---------------| :---- | :---------- |
| <span data-ttu-id="f26c5-125">id</span><span class="sxs-lookup"><span data-stu-id="f26c5-125">id</span></span> | <span data-ttu-id="f26c5-126">String</span><span class="sxs-lookup"><span data-stu-id="f26c5-126">String</span></span> | <span data-ttu-id="f26c5-127">O identificador da decisão.</span><span class="sxs-lookup"><span data-stu-id="f26c5-127">The identifier of the decision.</span></span> |
| <span data-ttu-id="f26c5-128">accessReviewId</span><span class="sxs-lookup"><span data-stu-id="f26c5-128">accessReviewId</span></span> | <span data-ttu-id="f26c5-129">String</span><span class="sxs-lookup"><span data-stu-id="f26c5-129">String</span></span> | <span data-ttu-id="f26c5-130">O identificador do pai accessReviewInstance.</span><span class="sxs-lookup"><span data-stu-id="f26c5-130">The identifier of the accessReviewInstance parent.</span></span> |
| <span data-ttu-id="f26c5-131">reviewedBy</span><span class="sxs-lookup"><span data-stu-id="f26c5-131">reviewedBy</span></span> | [<span data-ttu-id="f26c5-132">userIdentity</span><span class="sxs-lookup"><span data-stu-id="f26c5-132">userIdentity</span></span>](useridentity.md) | <span data-ttu-id="f26c5-133">O identificador do revistor.</span><span class="sxs-lookup"><span data-stu-id="f26c5-133">The identifier of the reviewer.</span></span> |
| <span data-ttu-id="f26c5-134">reviewedDateTime</span><span class="sxs-lookup"><span data-stu-id="f26c5-134">reviewedDateTime</span></span> | <span data-ttu-id="f26c5-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f26c5-135">DateTimeOffset</span></span> | <span data-ttu-id="f26c5-136">O timestamp quando a revisão ocorreu.</span><span class="sxs-lookup"><span data-stu-id="f26c5-136">The timestamp when the review occurred.</span></span> |
| <span data-ttu-id="f26c5-137">decision</span><span class="sxs-lookup"><span data-stu-id="f26c5-137">decision</span></span> | <span data-ttu-id="f26c5-138">String</span><span class="sxs-lookup"><span data-stu-id="f26c5-138">String</span></span> | <span data-ttu-id="f26c5-139">Resultado da revisão.</span><span class="sxs-lookup"><span data-stu-id="f26c5-139">Result of the review.</span></span> <span data-ttu-id="f26c5-140">Valores possíveis: `Approve` `Deny` , , ou `NotReviewed` `DontKnow` .</span><span class="sxs-lookup"><span data-stu-id="f26c5-140">Possible values: `Approve`, `Deny`, `NotReviewed`, or `DontKnow`.</span></span> |
| <span data-ttu-id="f26c5-141">justification</span><span class="sxs-lookup"><span data-stu-id="f26c5-141">justification</span></span> | <span data-ttu-id="f26c5-142">String</span><span class="sxs-lookup"><span data-stu-id="f26c5-142">String</span></span> | <span data-ttu-id="f26c5-143">A justificativa da decisão de revisão.</span><span class="sxs-lookup"><span data-stu-id="f26c5-143">The review decision justification.</span></span> |
| <span data-ttu-id="f26c5-144">appliedBy</span><span class="sxs-lookup"><span data-stu-id="f26c5-144">appliedBy</span></span> | [<span data-ttu-id="f26c5-145">userIdentity</span><span class="sxs-lookup"><span data-stu-id="f26c5-145">userIdentity</span></span>](useridentity.md) | <span data-ttu-id="f26c5-146">O identificador do usuário que aplicou a decisão.</span><span class="sxs-lookup"><span data-stu-id="f26c5-146">The identifier of the user who applied the decision.</span></span> |
| <span data-ttu-id="f26c5-147">appliedDateTime</span><span class="sxs-lookup"><span data-stu-id="f26c5-147">appliedDateTime</span></span> | <span data-ttu-id="f26c5-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f26c5-148">DateTimeOffset</span></span> | <span data-ttu-id="f26c5-149">O timestamp quando a decisão de aprovação foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="f26c5-149">The timestamp when the approval decision was applied.</span></span> <span data-ttu-id="f26c5-150">O tipo DatetimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre em horário UTC.</span><span class="sxs-lookup"><span data-stu-id="f26c5-150">The DatetimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f26c5-151">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="f26c5-151">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
| <span data-ttu-id="f26c5-152">applyResult</span><span class="sxs-lookup"><span data-stu-id="f26c5-152">applyResult</span></span> | <span data-ttu-id="f26c5-153">String</span><span class="sxs-lookup"><span data-stu-id="f26c5-153">String</span></span> | <span data-ttu-id="f26c5-154">O resultado da aplicação da decisão.</span><span class="sxs-lookup"><span data-stu-id="f26c5-154">The result of applying the decision.</span></span> <span data-ttu-id="f26c5-155">Valores possíveis: `NotApplied` , , , ou `Success` `Failed` `NotFound` `NotSupported` .</span><span class="sxs-lookup"><span data-stu-id="f26c5-155">Possible values: `NotApplied`, `Success`, `Failed`, `NotFound`, or `NotSupported`.</span></span> |
| <span data-ttu-id="f26c5-156">recommendation</span><span class="sxs-lookup"><span data-stu-id="f26c5-156">recommendation</span></span> | <span data-ttu-id="f26c5-157">String</span><span class="sxs-lookup"><span data-stu-id="f26c5-157">String</span></span> | <span data-ttu-id="f26c5-158">Uma recomendação gerada pelo sistema para a decisão de aprovação.</span><span class="sxs-lookup"><span data-stu-id="f26c5-158">A system-generated recommendation for the approval decision.</span></span> <span data-ttu-id="f26c5-159">Valores possíveis: `Approve` `Deny` , ou `NotAvailable` .</span><span class="sxs-lookup"><span data-stu-id="f26c5-159">Possible values: `Approve`, `Deny`, or `NotAvailable`.</span></span>  |
| <span data-ttu-id="f26c5-160">destino</span><span class="sxs-lookup"><span data-stu-id="f26c5-160">target</span></span> | [<span data-ttu-id="f26c5-161">accessReviewInstanceDecisionItemTarget</span><span class="sxs-lookup"><span data-stu-id="f26c5-161">accessReviewInstanceDecisionItemTarget</span></span>](accessreviewinstancedecisionitemtarget.md)  | <span data-ttu-id="f26c5-162">O destino dessa decisão específica.</span><span class="sxs-lookup"><span data-stu-id="f26c5-162">The target of this specific decision.</span></span> <span data-ttu-id="f26c5-163">Os destinos de decisão podem ser de tipos diferentes– cada um com suas próprias propriedades específicas.</span><span class="sxs-lookup"><span data-stu-id="f26c5-163">Decision targets can be of different types – each one with its own specific properties.</span></span> <span data-ttu-id="f26c5-164">Consulte [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md).</span><span class="sxs-lookup"><span data-stu-id="f26c5-164">See [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md).</span></span> |
|<span data-ttu-id="f26c5-165">principal</span><span class="sxs-lookup"><span data-stu-id="f26c5-165">principal</span></span>|[<span data-ttu-id="f26c5-166">identity</span><span class="sxs-lookup"><span data-stu-id="f26c5-166">identity</span></span>](../resources/identity.md)|<span data-ttu-id="f26c5-167">Cada item de decisão em uma revisão de acesso representa o acesso de uma entidade a um recurso.</span><span class="sxs-lookup"><span data-stu-id="f26c5-167">Every decision item in an access review represents a principal's access to a resource.</span></span> <span data-ttu-id="f26c5-168">Essa propriedade representa detalhes da entidade.</span><span class="sxs-lookup"><span data-stu-id="f26c5-168">This property represents details of the principal.</span></span> <span data-ttu-id="f26c5-169">Por exemplo, se um item de decisão representa o acesso de Usuário "Bob" ao Grupo "Vendas" - a entidade é "Bob" e o recurso é "Vendas".</span><span class="sxs-lookup"><span data-stu-id="f26c5-169">For example, if a decision item represents access of User "Bob" to Group "Sales" - The principal is "Bob" and the resource is "Sales".</span></span> <span data-ttu-id="f26c5-170">Os principais podem ser de dois tipos - userIdentity e servicePrincipalIdentity.</span><span class="sxs-lookup"><span data-stu-id="f26c5-170">Principals can be of two types - userIdentity and servicePrincipalIdentity.</span></span>|
|<span data-ttu-id="f26c5-171">recurso</span><span class="sxs-lookup"><span data-stu-id="f26c5-171">resource</span></span>|[<span data-ttu-id="f26c5-172">accessReviewInstanceDecisionItemResource</span><span class="sxs-lookup"><span data-stu-id="f26c5-172">accessReviewInstanceDecisionItemResource</span></span>](../resources/accessreviewinstancedecisionitemresource.md)|<span data-ttu-id="f26c5-173">Cada item de decisão em uma revisão de acesso representa o acesso de uma entidade a um recurso.</span><span class="sxs-lookup"><span data-stu-id="f26c5-173">Every decision item in an access review represents a principal's access to a resource.</span></span> <span data-ttu-id="f26c5-174">Essa propriedade representa detalhes do recurso.</span><span class="sxs-lookup"><span data-stu-id="f26c5-174">This property represents details of the resource.</span></span> <span data-ttu-id="f26c5-175">Por exemplo, se um item de decisão representa o acesso de Usuário "Bob" ao Grupo "Vendas" - a entidade é Bob e o recurso é "Vendas".</span><span class="sxs-lookup"><span data-stu-id="f26c5-175">For example, if a decision item represents access of User "Bob" to Group "Sales" - The principal is Bob and the resource is "Sales".</span></span> <span data-ttu-id="f26c5-176">Os recursos podem ser de vários tipos.</span><span class="sxs-lookup"><span data-stu-id="f26c5-176">Resources can be of multiple types.</span></span> <span data-ttu-id="f26c5-177">Consulte [accessReviewInstanceDecisionItemResource](../resources/accessreviewinstancedecisionitemresource.md)</span><span class="sxs-lookup"><span data-stu-id="f26c5-177">See [accessReviewInstanceDecisionItemResource](../resources/accessreviewinstancedecisionitemresource.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="f26c5-178">Relações</span><span class="sxs-lookup"><span data-stu-id="f26c5-178">Relationships</span></span>

| <span data-ttu-id="f26c5-179">Relação</span><span class="sxs-lookup"><span data-stu-id="f26c5-179">Relationship</span></span> | <span data-ttu-id="f26c5-180">Tipo</span><span class="sxs-lookup"><span data-stu-id="f26c5-180">Type</span></span>   |<span data-ttu-id="f26c5-181">Descrição</span><span class="sxs-lookup"><span data-stu-id="f26c5-181">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f26c5-182">instância</span><span class="sxs-lookup"><span data-stu-id="f26c5-182">instance</span></span> |[<span data-ttu-id="f26c5-183">accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="f26c5-183">accessReviewInstance</span></span>](accessreviewinstance.md) | <span data-ttu-id="f26c5-184">Há exatamente um accessReviewInstance associado a cada decisão.</span><span class="sxs-lookup"><span data-stu-id="f26c5-184">There is exactly one accessReviewInstance associated with each decision.</span></span> <span data-ttu-id="f26c5-185">A instância é o pai do item de decisão, representando a recorrência da revisão de acesso em que a decisão é tomada.</span><span class="sxs-lookup"><span data-stu-id="f26c5-185">The instance is the parent of the decision item, representing the recurrence of the access review the decision is made on.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="f26c5-186">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f26c5-186">JSON representation</span></span>

<span data-ttu-id="f26c5-187">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f26c5-187">Here is a JSON representation of the resource.</span></span>

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
  "id": "String (identifier)",
  "accessReviewId": "String",
  "reviewedBy": {
    "@odata.type": "microsoft.graph.userIdentity"
  },
  "reviewedDateTime": "String (timestamp)",
  "decision": "String",
  "justification": "String",
  "appliedBy": {
    "@odata.type": "microsoft.graph.userIdentity"
  },
  "appliedDateTime": "String (timestamp)",
  "applyResult": "String",
  "recommendation": "String",
  "target": {
    "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemTarget"
  },
  "principal": {
    "@odata.type": "microsoft.graph.identity"
  },
  "resource": {
    "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemResource"
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
