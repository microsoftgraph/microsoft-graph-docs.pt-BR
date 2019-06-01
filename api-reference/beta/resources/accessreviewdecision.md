---
title: tipo de recurso accessReviewDecision
description: No recurso de revisões do Azure AD Access, `accessReviewDecision` o representa uma decisão de revisão do Azure ad Access de um determinado acesso de uma entidade.  Em uma revisão do Access, ou uma instância de uma revisão de acesso recorrente, há uma `accessReviewDecision` por usuário revisado.  Por exemplo, se um grupo tiver dois convidados e um não convidado como membros, e uma revisão de acesso de convidados for executada para esse grupo, haverá dois objetos de decisão de análise do Access.  Se um revisor alterar sua decisão ou outro revisor o substituir, o `accessReviewDecision` será atualizado.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 034ecbdaa108d0c63378d1c00136f0415019b262
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657739"
---
# <a name="accessreviewdecision-resource-type"></a><span data-ttu-id="65e84-106">tipo de recurso accessReviewDecision</span><span class="sxs-lookup"><span data-stu-id="65e84-106">accessReviewDecision resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65e84-107">No recurso de revisões do Azure AD [Access](accessreviews-root.md) , `accessReviewDecision` o representa uma decisão de revisão do Azure ad Access de um determinado acesso de uma entidade.</span><span class="sxs-lookup"><span data-stu-id="65e84-107">In the Azure AD [access reviews](accessreviews-root.md) feature, the `accessReviewDecision` represents an Azure AD access review decision of a particular entity's access.</span></span>  <span data-ttu-id="65e84-108">Em uma revisão do Access, ou uma instância de uma revisão de acesso recorrente, há uma `accessReviewDecision` por usuário revisado.</span><span class="sxs-lookup"><span data-stu-id="65e84-108">Within an access review, or an instance of a recurring access review, there is one `accessReviewDecision` per reviewed user.</span></span>  <span data-ttu-id="65e84-109">Por exemplo, se um grupo tiver dois convidados e um não convidado como membros, e uma revisão de acesso de convidados for executada para esse grupo, haverá dois objetos de decisão de análise do Access.</span><span class="sxs-lookup"><span data-stu-id="65e84-109">For example, if a group has two guests and one non-guest as members, and an access review of guests is performed for that group, then there will be two access review decision objects.</span></span>  <span data-ttu-id="65e84-110">Se um revisor alterar sua decisão ou outro revisor o substituir, o `accessReviewDecision` será atualizado.</span><span class="sxs-lookup"><span data-stu-id="65e84-110">If a reviewer changes their decision, or another reviewer overrides them, then the `accessReviewDecision` is updated.</span></span>


## <a name="methods"></a><span data-ttu-id="65e84-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="65e84-111">Methods</span></span>

<span data-ttu-id="65e84-112">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="65e84-112">None.</span></span>  <span data-ttu-id="65e84-113">Os objetos desse tipo são criados automaticamente pelo recurso quando uma revisão do Access Inicializa e não pode ser excluída.</span><span class="sxs-lookup"><span data-stu-id="65e84-113">Objects of this type are automatically created by the feature when an access review initializes, and cannot be deleted.</span></span>  <span data-ttu-id="65e84-114">Eles podem ser recuperados de uma revisão de acesso usando as relações de [decisões](../api/accessreview-listdecisions.md) e mydecisions. [](../api/accessreview-listmydecisions.md)</span><span class="sxs-lookup"><span data-stu-id="65e84-114">They can be retrieved from an access review using the [decisions](../api/accessreview-listdecisions.md) and [mydecisions](../api/accessreview-listmydecisions.md) relationships.</span></span>

## <a name="properties"></a><span data-ttu-id="65e84-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="65e84-115">Properties</span></span>

<span data-ttu-id="65e84-116">Esta tabela ilustra as propriedades básicas de objetos desse tipo.</span><span class="sxs-lookup"><span data-stu-id="65e84-116">This table illustrates the base properties of objects of this type.</span></span> 

| <span data-ttu-id="65e84-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="65e84-117">Property</span></span>                        | <span data-ttu-id="65e84-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="65e84-118">Type</span></span>                         | <span data-ttu-id="65e84-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="65e84-119">Description</span></span>                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `id`                            |`String`                      | <span data-ttu-id="65e84-120">A identificação da decisão dentro da revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="65e84-120">The id of the decision within the access review.</span></span>                                                                                     |
| `accessReviewId`                |`String`                      | <span data-ttu-id="65e84-121">A ID gerada pelo recurso da revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="65e84-121">The feature-generated id of the access review.</span></span>                                                                                       |
| `reviewedBy`                    |[<span data-ttu-id="65e84-122">userIdentity</span><span class="sxs-lookup"><span data-stu-id="65e84-122">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="65e84-123">A identidade do revisor.</span><span class="sxs-lookup"><span data-stu-id="65e84-123">The identity of the reviewer.</span></span>                                                                                       |
| `reviewedDate`                  |`DateTimeOffset`              | <span data-ttu-id="65e84-124">A data e a hora em que a revisão mais recente desse direito de acesso foi fornecida.</span><span class="sxs-lookup"><span data-stu-id="65e84-124">The date and time the most recent review for this access right was supplied.</span></span>                                                                         |
| `reviewResult`                  |`String`                      | <span data-ttu-id="65e84-125">O resultado da revisão.</span><span class="sxs-lookup"><span data-stu-id="65e84-125">The result of the review.</span></span>                                                                                    |
| `justification`                 |`String`                      | <span data-ttu-id="65e84-126">A justificativa de negócios do revisor, se fornecido.</span><span class="sxs-lookup"><span data-stu-id="65e84-126">The reviewer's business justification, if supplied.</span></span>                                                                         |
| `appliedBy`                     |[<span data-ttu-id="65e84-127">userIdentity</span><span class="sxs-lookup"><span data-stu-id="65e84-127">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="65e84-128">Quando a revisão for concluída, se os resultados forem aplicados manualmente, a identidade do usuário que aplicou a decisão.</span><span class="sxs-lookup"><span data-stu-id="65e84-128">When the review completes, if the results were manually applied, the user identity of the user who applied the decision.</span></span>                                                           |
| `appliedDateTime`               |`DateTimeOffset`              | <span data-ttu-id="65e84-129">A data e a hora em que a decisão de revisão foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="65e84-129">The date and time when the review decision was applied.</span></span>                                                          |
| `applyResult`                   |`String`                      | <span data-ttu-id="65e84-130">O resultado da aplicação da decisão, um de `NotApplied`, `Success` `Failed` `NotFound` ou `NotSupported`.</span><span class="sxs-lookup"><span data-stu-id="65e84-130">The outcome of applying the decision, one of `NotApplied`, `Success`, `Failed`, `NotFound` or `NotSupported`.</span></span>                      |
| `accessRecommendation`          |`String`                      | <span data-ttu-id="65e84-131">A recomendação gerada pelo recurso mostrada para o revisor, um `Approve` `Deny` ou. `NotAvailable`</span><span class="sxs-lookup"><span data-stu-id="65e84-131">The feature- generated recommendation shown to the reviewer, one of `Approve`, `Deny` or `NotAvailable`.</span></span> |


<span data-ttu-id="65e84-132">Além disso, as propriedades adicionais podem estar presentes dependendo do tipo de objeto do objeto que possui o acesso que foi escolhido.</span><span class="sxs-lookup"><span data-stu-id="65e84-132">In addition, additional properties may be present depending on the object type of the object possessing the access that was decided upon.</span></span>  <span data-ttu-id="65e84-133">Por exemplo, se a decisão de revisão do Access for a associação de grupo ou o acesso de um usuário específico, o usuário que estiver possivelmente com o acesso será removido é identificado por estas propriedades:</span><span class="sxs-lookup"><span data-stu-id="65e84-133">For example, if the access review decision is a particular user's group membership or application access, the user who is potentially going to have their access be removed is identified through these properties:</span></span>

| <span data-ttu-id="65e84-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="65e84-134">Property</span></span>                        | <span data-ttu-id="65e84-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="65e84-135">Type</span></span>                         | <span data-ttu-id="65e84-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="65e84-136">Description</span></span>                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `userId`                            |`String`                      | <span data-ttu-id="65e84-137">A ID do usuário cujo acesso foi revisado.</span><span class="sxs-lookup"><span data-stu-id="65e84-137">The id of user whose access was reviewed.</span></span>                                                                                    |
| `userDisplayName`                            |`String`                      | <span data-ttu-id="65e84-138">O nome de exibição do usuário cujo acesso foi revisado.</span><span class="sxs-lookup"><span data-stu-id="65e84-138">The display name of the user whose access was reviewed.</span></span>                                                                                     |
| `userPrincipalName`                            |`String`                      | <span data-ttu-id="65e84-139">O nome principal de usuário do usuário cujo acesso foi revisado.</span><span class="sxs-lookup"><span data-stu-id="65e84-139">The user principal name of the user whose access was reviewed.</span></span>                                                                                     |



## <a name="relationships"></a><span data-ttu-id="65e84-140">Relações</span><span class="sxs-lookup"><span data-stu-id="65e84-140">Relationships</span></span>

<span data-ttu-id="65e84-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="65e84-141">None.</span></span>  <span data-ttu-id="65e84-142">Os objetos desse tipo podem ser recuperados de uma análise do Access usando as relações de [decisões](../api/accessreview-listdecisions.md) e mydecisions do objeto [accessReview](accessreview.md) . [](../api/accessreview-listmydecisions.md)</span><span class="sxs-lookup"><span data-stu-id="65e84-142">Objects of this type can be retrieved from an access review using the [decisions](../api/accessreview-listdecisions.md) and [mydecisions](../api/accessreview-listmydecisions.md) relationships of the [accessReview](accessreview.md) object.</span></span>

## <a name="see-also"></a><span data-ttu-id="65e84-143">Confira também</span><span class="sxs-lookup"><span data-stu-id="65e84-143">See also</span></span>

| <span data-ttu-id="65e84-144">Método</span><span class="sxs-lookup"><span data-stu-id="65e84-144">Method</span></span>           | <span data-ttu-id="65e84-145">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="65e84-145">Return Type</span></span>    |<span data-ttu-id="65e84-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="65e84-146">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="65e84-147">Listar decisões accessReview</span><span class="sxs-lookup"><span data-stu-id="65e84-147">List accessReview decisions</span></span>](../api/accessreview-listdecisions.md) |      <span data-ttu-id="65e84-148">coleção [accessReviewDecision](accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="65e84-148">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="65e84-149">Obtenha as decisões de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="65e84-149">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="65e84-150">Listar minhas decisões do accessReview</span><span class="sxs-lookup"><span data-stu-id="65e84-150">List my accessReview decisions</span></span>](../api/accessreview-listmydecisions.md) |     <span data-ttu-id="65e84-151">coleção [accessReviewDecision](accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="65e84-151">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="65e84-152">Como revisor, obtenha as minhas decisões de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="65e84-152">As a reviewer, get my decisions of an accessReview.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="65e84-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="65e84-153">JSON representation</span></span>

<span data-ttu-id="65e84-154">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="65e84-154">Here is a JSON representation of the resource.</span></span>

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
