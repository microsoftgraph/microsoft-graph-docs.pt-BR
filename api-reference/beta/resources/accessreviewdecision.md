---
title: tipo de recurso accessReviewDecision
description: No recurso de revisões do Azure AD Access, `accessReviewDecision` o representa uma decisão de revisão do Azure ad Access de um determinado acesso de uma entidade.  Em uma revisão do Access, ou uma instância de uma revisão de acesso recorrente, há uma `accessReviewDecision` por usuário revisado.  Por exemplo, se um grupo tiver dois convidados e um não convidado como membros, e uma revisão de acesso de convidados for executada para esse grupo, haverá dois objetos de decisão de análise do Access.  Se um revisor alterar sua decisão ou outro revisor o substituir, o `accessReviewDecision` será atualizado.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e92eb6b17b76ac3f8e44404dfbc776463170e0fc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508475"
---
# <a name="accessreviewdecision-resource-type"></a><span data-ttu-id="30a17-106">tipo de recurso accessReviewDecision</span><span class="sxs-lookup"><span data-stu-id="30a17-106">accessReviewDecision resource type</span></span>

<span data-ttu-id="30a17-107">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="30a17-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30a17-108">No recurso de revisões do Azure AD [Access](accessreviews-root.md) , `accessReviewDecision` o representa uma decisão de revisão do Azure ad Access de um determinado acesso de uma entidade.</span><span class="sxs-lookup"><span data-stu-id="30a17-108">In the Azure AD [access reviews](accessreviews-root.md) feature, the `accessReviewDecision` represents an Azure AD access review decision of a particular entity's access.</span></span>  <span data-ttu-id="30a17-109">Em uma revisão do Access, ou uma instância de uma revisão de acesso recorrente, há uma `accessReviewDecision` por usuário revisado.</span><span class="sxs-lookup"><span data-stu-id="30a17-109">Within an access review, or an instance of a recurring access review, there is one `accessReviewDecision` per reviewed user.</span></span>  <span data-ttu-id="30a17-110">Por exemplo, se um grupo tiver dois convidados e um não convidado como membros, e uma revisão de acesso de convidados for executada para esse grupo, haverá dois objetos de decisão de análise do Access.</span><span class="sxs-lookup"><span data-stu-id="30a17-110">For example, if a group has two guests and one non-guest as members, and an access review of guests is performed for that group, then there will be two access review decision objects.</span></span>  <span data-ttu-id="30a17-111">Se um revisor alterar sua decisão ou outro revisor o substituir, o `accessReviewDecision` será atualizado.</span><span class="sxs-lookup"><span data-stu-id="30a17-111">If a reviewer changes their decision, or another reviewer overrides them, then the `accessReviewDecision` is updated.</span></span>


## <a name="methods"></a><span data-ttu-id="30a17-112">Métodos</span><span class="sxs-lookup"><span data-stu-id="30a17-112">Methods</span></span>

<span data-ttu-id="30a17-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="30a17-113">None.</span></span>  <span data-ttu-id="30a17-114">Os objetos desse tipo são criados automaticamente pelo recurso quando uma revisão do Access Inicializa e não pode ser excluída.</span><span class="sxs-lookup"><span data-stu-id="30a17-114">Objects of this type are automatically created by the feature when an access review initializes, and cannot be deleted.</span></span>  <span data-ttu-id="30a17-115">Eles podem ser recuperados de uma revisão de acesso usando as relações de [decisões](../api/accessreview-listdecisions.md) e [mydecisions](../api/accessreview-listmydecisions.md) .</span><span class="sxs-lookup"><span data-stu-id="30a17-115">They can be retrieved from an access review using the [decisions](../api/accessreview-listdecisions.md) and [mydecisions](../api/accessreview-listmydecisions.md) relationships.</span></span>

## <a name="properties"></a><span data-ttu-id="30a17-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="30a17-116">Properties</span></span>

<span data-ttu-id="30a17-117">Esta tabela ilustra as propriedades básicas de objetos desse tipo.</span><span class="sxs-lookup"><span data-stu-id="30a17-117">This table illustrates the base properties of objects of this type.</span></span> 

| <span data-ttu-id="30a17-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="30a17-118">Property</span></span>                        | <span data-ttu-id="30a17-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="30a17-119">Type</span></span>                         | <span data-ttu-id="30a17-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="30a17-120">Description</span></span>                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `id`                            |`String`                      | <span data-ttu-id="30a17-121">A identificação da decisão dentro da revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="30a17-121">The id of the decision within the access review.</span></span>                                                                                     |
| `accessReviewId`                |`String`                      | <span data-ttu-id="30a17-122">A ID gerada pelo recurso da revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="30a17-122">The feature-generated id of the access review.</span></span>                                                                                       |
| `reviewedBy`                    |[<span data-ttu-id="30a17-123">userIdentity</span><span class="sxs-lookup"><span data-stu-id="30a17-123">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="30a17-124">A identidade do revisor.</span><span class="sxs-lookup"><span data-stu-id="30a17-124">The identity of the reviewer.</span></span> <span data-ttu-id="30a17-125">Se a recomendação tiver sido usada como revisão, o userPrincipalName estará vazio.</span><span class="sxs-lookup"><span data-stu-id="30a17-125">If the recommendation was used as the review, the userPrincipalName is empty.</span></span>                                                                                      |
| `reviewedDate`                  |`DateTimeOffset`              | <span data-ttu-id="30a17-126">A data e a hora em que a revisão mais recente desse direito de acesso foi fornecida.</span><span class="sxs-lookup"><span data-stu-id="30a17-126">The date and time the most recent review for this access right was supplied.</span></span>                                                                         |
| `reviewResult`                  |`String`                      | <span data-ttu-id="30a17-127">O resultado da revisão, um `NotReviewed`de, `Deny` `DontKnow` ou. `Approve`</span><span class="sxs-lookup"><span data-stu-id="30a17-127">The result of the review, one of `NotReviewed`, `Deny`, `DontKnow` or `Approve`.</span></span>                                                                                    |
| `justification`                 |`String`                      | <span data-ttu-id="30a17-128">A justificativa de negócios do revisor, se fornecido.</span><span class="sxs-lookup"><span data-stu-id="30a17-128">The reviewer's business justification, if supplied.</span></span>                                                                         |
| `appliedBy`                     |[<span data-ttu-id="30a17-129">userIdentity</span><span class="sxs-lookup"><span data-stu-id="30a17-129">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="30a17-130">Quando a revisão for concluída, se os resultados forem aplicados manualmente, a identidade do usuário que aplicou a decisão.</span><span class="sxs-lookup"><span data-stu-id="30a17-130">When the review completes, if the results were manually applied, the user identity of the user who applied the decision.</span></span> <span data-ttu-id="30a17-131">Se a revisão foi aplicada automaticamente, o userPrincipalName estará vazio.</span><span class="sxs-lookup"><span data-stu-id="30a17-131">If the review was auto-applied, the userPrincipalName is empty.</span></span>                                                          |
| `appliedDateTime`               |`DateTimeOffset`              | <span data-ttu-id="30a17-132">A data e a hora em que a decisão de revisão foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="30a17-132">The date and time when the review decision was applied.</span></span>                                                          |
| `applyResult`                   |`String`                      | <span data-ttu-id="30a17-133">O resultado da aplicação da decisão, um de `NotApplied`, `Success` `Failed` `NotFound` ou `NotSupported`.</span><span class="sxs-lookup"><span data-stu-id="30a17-133">The outcome of applying the decision, one of `NotApplied`, `Success`, `Failed`, `NotFound` or `NotSupported`.</span></span>                      |
| `accessRecommendation`          |`String`                      | <span data-ttu-id="30a17-134">A recomendação gerada pelo recurso mostrada para o revisor, um `Approve` `Deny` ou. `NotAvailable`</span><span class="sxs-lookup"><span data-stu-id="30a17-134">The feature- generated recommendation shown to the reviewer, one of `Approve`, `Deny` or `NotAvailable`.</span></span> |


<span data-ttu-id="30a17-135">Além disso, as propriedades adicionais podem estar presentes dependendo do tipo de objeto do objeto que possui o acesso que foi escolhido.</span><span class="sxs-lookup"><span data-stu-id="30a17-135">In addition, additional properties may be present depending on the object type of the object possessing the access that was decided upon.</span></span>  <span data-ttu-id="30a17-136">Por exemplo, se a decisão de revisão do Access for a associação de grupo ou o acesso de um usuário específico, o usuário que estiver possivelmente com o acesso será removido é identificado por estas propriedades:</span><span class="sxs-lookup"><span data-stu-id="30a17-136">For example, if the access review decision is a particular user's group membership or application access, the user who is potentially going to have their access be removed is identified through these properties:</span></span>

| <span data-ttu-id="30a17-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="30a17-137">Property</span></span>                        | <span data-ttu-id="30a17-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="30a17-138">Type</span></span>                         | <span data-ttu-id="30a17-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="30a17-139">Description</span></span>                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `userId`                            |`String`                      | <span data-ttu-id="30a17-140">A ID do usuário cujo acesso foi revisado.</span><span class="sxs-lookup"><span data-stu-id="30a17-140">The id of user whose access was reviewed.</span></span>                                                                                    |
| `userDisplayName`                            |`String`                      | <span data-ttu-id="30a17-141">O nome de exibição do usuário cujo acesso foi revisado.</span><span class="sxs-lookup"><span data-stu-id="30a17-141">The display name of the user whose access was reviewed.</span></span>                                                                                     |
| `userPrincipalName`                            |`String`                      | <span data-ttu-id="30a17-142">O nome principal de usuário do usuário cujo acesso foi revisado.</span><span class="sxs-lookup"><span data-stu-id="30a17-142">The user principal name of the user whose access was reviewed.</span></span>                                                                                     |



## <a name="relationships"></a><span data-ttu-id="30a17-143">Relações</span><span class="sxs-lookup"><span data-stu-id="30a17-143">Relationships</span></span>

<span data-ttu-id="30a17-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="30a17-144">None.</span></span>  <span data-ttu-id="30a17-145">Os objetos desse tipo podem ser recuperados de uma análise do Access usando as relações de [decisões](../api/accessreview-listdecisions.md) e [mydecisions](../api/accessreview-listmydecisions.md) do objeto [accessReview](accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="30a17-145">Objects of this type can be retrieved from an access review using the [decisions](../api/accessreview-listdecisions.md) and [mydecisions](../api/accessreview-listmydecisions.md) relationships of the [accessReview](accessreview.md) object.</span></span>

## <a name="see-also"></a><span data-ttu-id="30a17-146">Confira também</span><span class="sxs-lookup"><span data-stu-id="30a17-146">See also</span></span>

| <span data-ttu-id="30a17-147">Método</span><span class="sxs-lookup"><span data-stu-id="30a17-147">Method</span></span>           | <span data-ttu-id="30a17-148">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="30a17-148">Return Type</span></span>    |<span data-ttu-id="30a17-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="30a17-149">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="30a17-150">Listar decisões accessReview</span><span class="sxs-lookup"><span data-stu-id="30a17-150">List accessReview decisions</span></span>](../api/accessreview-listdecisions.md) |      <span data-ttu-id="30a17-151">coleção [accessReviewDecision](accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="30a17-151">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="30a17-152">Obtenha as decisões de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="30a17-152">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="30a17-153">Listar minhas decisões do accessReview</span><span class="sxs-lookup"><span data-stu-id="30a17-153">List my accessReview decisions</span></span>](../api/accessreview-listmydecisions.md) |     <span data-ttu-id="30a17-154">coleção [accessReviewDecision](accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="30a17-154">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="30a17-155">Como revisor, obtenha as minhas decisões de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="30a17-155">As a reviewer, get my decisions of an accessReview.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="30a17-156">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="30a17-156">JSON representation</span></span>

<span data-ttu-id="30a17-157">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="30a17-157">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessReviewDecision"
}-->

```json
{
"id": "string (identifier)",
"accessReviewId": "string (identifier)",
"reviewedBy": "microsoft.graph.userIdentity",
"reviewedDate": "string (timestamp)",
"reviewResult": "string",
"justification": "string",
"appliedBy": "microsoft.graph.userIdentity",
"appliedDateTime": "string (timestamp)",
"applyResult": "string",
"accessRecommendation": "string",
"userId": "string",
"userDisplayName": "string",
"userPrincipalName": "string"
}

```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewDecision resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
