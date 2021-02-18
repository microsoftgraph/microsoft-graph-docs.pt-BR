---
title: Tipo de recurso accessReviewDecision
description: The accessReviewDecision represents an Azure AD access review decision of a particular entity's access.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 52d4e2a262d3a90010cc0e254e11f2d723a5e550
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292690"
---
# <a name="accessreviewdecision-resource-type"></a><span data-ttu-id="f82ea-103">Tipo de recurso accessReviewDecision</span><span class="sxs-lookup"><span data-stu-id="f82ea-103">accessReviewDecision resource type</span></span>

<span data-ttu-id="f82ea-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f82ea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

<span data-ttu-id="f82ea-105">No recurso de revisões de acesso do Azure [AD,](accessreviews-root.md) ele representa uma decisão de revisão de acesso do `accessReviewDecision` Azure AD do acesso de uma entidade específica.</span><span class="sxs-lookup"><span data-stu-id="f82ea-105">In the Azure AD [access reviews](accessreviews-root.md) feature, the `accessReviewDecision` represents an Azure AD access review decision of a particular entity's access.</span></span>  <span data-ttu-id="f82ea-106">Em uma revisão de acesso ou em uma instância de uma revisão de acesso recorrente, há um `accessReviewDecision` por usuário revisado.</span><span class="sxs-lookup"><span data-stu-id="f82ea-106">Within an access review, or an instance of a recurring access review, there is one `accessReviewDecision` per reviewed user.</span></span>  <span data-ttu-id="f82ea-107">Por exemplo, se um grupo tiver dois convidados e um não convidado como membros e uma revisão de acesso dos convidados for executada para esse grupo, haverá dois objetos de decisão de revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="f82ea-107">For example, if a group has two guests and one non-guest as members, and an access review of guests is performed for that group, then there will be two access review decision objects.</span></span>  <span data-ttu-id="f82ea-108">Se um revisador alterar sua decisão ou outro revisá-los, a `accessReviewDecision` atualização será atualizada.</span><span class="sxs-lookup"><span data-stu-id="f82ea-108">If a reviewer changes their decision, or another reviewer overrides them, then the `accessReviewDecision` is updated.</span></span>


## <a name="methods"></a><span data-ttu-id="f82ea-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="f82ea-109">Methods</span></span>

<span data-ttu-id="f82ea-110">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f82ea-110">None.</span></span>  <span data-ttu-id="f82ea-111">Os objetos desse tipo são criados automaticamente pelo recurso quando uma revisão de acesso é inicializada e não podem ser excluídos.</span><span class="sxs-lookup"><span data-stu-id="f82ea-111">Objects of this type are automatically created by the feature when an access review initializes, and cannot be deleted.</span></span>  <span data-ttu-id="f82ea-112">Eles podem ser recuperados de uma revisão de acesso usando [as decisões](../api/accessreview-listdecisions.md) e as relações de [mydecisions.](../api/accessreview-listmydecisions.md)</span><span class="sxs-lookup"><span data-stu-id="f82ea-112">They can be retrieved from an access review using the [decisions](../api/accessreview-listdecisions.md) and [mydecisions](../api/accessreview-listmydecisions.md) relationships.</span></span>

## <a name="properties"></a><span data-ttu-id="f82ea-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f82ea-113">Properties</span></span>

<span data-ttu-id="f82ea-114">Esta tabela ilustra as propriedades base dos objetos desse tipo.</span><span class="sxs-lookup"><span data-stu-id="f82ea-114">This table illustrates the base properties of objects of this type.</span></span> 

| <span data-ttu-id="f82ea-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f82ea-115">Property</span></span>                        | <span data-ttu-id="f82ea-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="f82ea-116">Type</span></span>                         | <span data-ttu-id="f82ea-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="f82ea-117">Description</span></span>                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `id`                            |`String`                      | <span data-ttu-id="f82ea-118">A id da decisão dentro da revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="f82ea-118">The id of the decision within the access review.</span></span>                                                                                     |
| `accessReviewId`                |`String`                      | <span data-ttu-id="f82ea-119">A ID gerada pelo recurso da revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="f82ea-119">The feature-generated id of the access review.</span></span>                                                                                       |
| `reviewedBy`                    |[<span data-ttu-id="f82ea-120">userIdentity</span><span class="sxs-lookup"><span data-stu-id="f82ea-120">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="f82ea-121">A identidade do revistor.</span><span class="sxs-lookup"><span data-stu-id="f82ea-121">The identity of the reviewer.</span></span> <span data-ttu-id="f82ea-122">Se a recomendação foi usada como revisão, o userPrincipalName está vazio.</span><span class="sxs-lookup"><span data-stu-id="f82ea-122">If the recommendation was used as the review, the userPrincipalName is empty.</span></span>                                                                                      |
| `reviewedDate`                  |`DateTimeOffset`              | <span data-ttu-id="f82ea-123">A data e a hora em que a revisão mais recente desse direito de acesso foi fornecida.</span><span class="sxs-lookup"><span data-stu-id="f82ea-123">The date and time the most recent review for this access right was supplied.</span></span>                                                                         |
| `reviewResult`                  |`String`                      | <span data-ttu-id="f82ea-124">O resultado da revisão, um de `NotReviewed` , `Deny` ou `DontKnow` `Approve` .</span><span class="sxs-lookup"><span data-stu-id="f82ea-124">The result of the review, one of `NotReviewed`, `Deny`, `DontKnow` or `Approve`.</span></span>                                                                                    |
| `justification`                 |`String`                      | <span data-ttu-id="f82ea-125">A justificativa comercial do revisador, se fornecida.</span><span class="sxs-lookup"><span data-stu-id="f82ea-125">The reviewer's business justification, if supplied.</span></span>                                                                         |
| `appliedBy`                     |[<span data-ttu-id="f82ea-126">userIdentity</span><span class="sxs-lookup"><span data-stu-id="f82ea-126">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="f82ea-127">Quando a revisão for concluída, se os resultados foram aplicados manualmente, a identidade do usuário que aplicou a decisão.</span><span class="sxs-lookup"><span data-stu-id="f82ea-127">When the review completes, if the results were manually applied, the user identity of the user who applied the decision.</span></span> <span data-ttu-id="f82ea-128">Se a revisão foi aplicada automaticamente, o userPrincipalName está vazio.</span><span class="sxs-lookup"><span data-stu-id="f82ea-128">If the review was auto-applied, the userPrincipalName is empty.</span></span>                                                          |
| `appliedDateTime`               |`DateTimeOffset`              | <span data-ttu-id="f82ea-129">A data e a hora em que a decisão de revisão foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="f82ea-129">The date and time when the review decision was applied.</span></span>                                                          |
| `applyResult`                   |`String`                      | <span data-ttu-id="f82ea-130">O resultado da aplicação da decisão, um dos `NotApplied` `Success` , ou `Failed` `NotFound` `NotSupported` .</span><span class="sxs-lookup"><span data-stu-id="f82ea-130">The outcome of applying the decision, one of `NotApplied`, `Success`, `Failed`, `NotFound` or `NotSupported`.</span></span>                      |
| `accessRecommendation`          |`String`                      | <span data-ttu-id="f82ea-131">O recurso - gerado recomendação mostrada para o revisador, um dos `Approve` ou `Deny` `NotAvailable` .</span><span class="sxs-lookup"><span data-stu-id="f82ea-131">The feature- generated recommendation shown to the reviewer, one of `Approve`, `Deny` or `NotAvailable`.</span></span> |


<span data-ttu-id="f82ea-132">Além disso, propriedades adicionais podem estar presentes dependendo do tipo de objeto do objeto que possui o acesso que foi decidido.</span><span class="sxs-lookup"><span data-stu-id="f82ea-132">In addition, additional properties may be present depending on the object type of the object possessing the access that was decided upon.</span></span>  <span data-ttu-id="f82ea-133">Por exemplo, se a decisão de revisão de acesso for a associação de grupo de um usuário específico ou o acesso a aplicativos, o usuário que potencialmente terá seu acesso removido será identificado por meio dessas propriedades:</span><span class="sxs-lookup"><span data-stu-id="f82ea-133">For example, if the access review decision is a particular user's group membership or application access, the user who is potentially going to have their access be removed is identified through these properties:</span></span>

| <span data-ttu-id="f82ea-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f82ea-134">Property</span></span>                        | <span data-ttu-id="f82ea-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="f82ea-135">Type</span></span>                         | <span data-ttu-id="f82ea-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="f82ea-136">Description</span></span>                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `userId`                            |`String`                      | <span data-ttu-id="f82ea-137">A id do usuário cujo acesso foi revisado.</span><span class="sxs-lookup"><span data-stu-id="f82ea-137">The id of user whose access was reviewed.</span></span>                                                                                    |
| `userDisplayName`                            |`String`                      | <span data-ttu-id="f82ea-138">O nome de exibição do usuário cujo acesso foi revisado.</span><span class="sxs-lookup"><span data-stu-id="f82ea-138">The display name of the user whose access was reviewed.</span></span>                                                                                     |
| `userPrincipalName`                            |`String`                      | <span data-ttu-id="f82ea-139">O nome principal do usuário cujo acesso foi revisado.</span><span class="sxs-lookup"><span data-stu-id="f82ea-139">The user principal name of the user whose access was reviewed.</span></span>                                                                                     |



## <a name="relationships"></a><span data-ttu-id="f82ea-140">Relações</span><span class="sxs-lookup"><span data-stu-id="f82ea-140">Relationships</span></span>

<span data-ttu-id="f82ea-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f82ea-141">None.</span></span>  <span data-ttu-id="f82ea-142">Objetos desse tipo podem ser recuperados de [](../api/accessreview-listdecisions.md) uma revisão de acesso usando as decisões e as relações de [mydecisions](../api/accessreview-listmydecisions.md) do [objeto accessReview](accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="f82ea-142">Objects of this type can be retrieved from an access review using the [decisions](../api/accessreview-listdecisions.md) and [mydecisions](../api/accessreview-listmydecisions.md) relationships of the [accessReview](accessreview.md) object.</span></span>

## <a name="see-also"></a><span data-ttu-id="f82ea-143">Confira também</span><span class="sxs-lookup"><span data-stu-id="f82ea-143">See also</span></span>

| <span data-ttu-id="f82ea-144">Método</span><span class="sxs-lookup"><span data-stu-id="f82ea-144">Method</span></span>           | <span data-ttu-id="f82ea-145">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f82ea-145">Return Type</span></span>    |<span data-ttu-id="f82ea-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="f82ea-146">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f82ea-147">Listar decisões de accessReview</span><span class="sxs-lookup"><span data-stu-id="f82ea-147">List accessReview decisions</span></span>](../api/accessreview-listdecisions.md) |      <span data-ttu-id="f82ea-148">[coleção accessReviewDecision](accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="f82ea-148">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="f82ea-149">Obter as decisões de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="f82ea-149">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="f82ea-150">Listar minhas decisões de accessReview</span><span class="sxs-lookup"><span data-stu-id="f82ea-150">List my accessReview decisions</span></span>](../api/accessreview-listmydecisions.md) |     <span data-ttu-id="f82ea-151">[coleção accessReviewDecision](accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="f82ea-151">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="f82ea-152">Como revisor, receba minhas decisões de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="f82ea-152">As a reviewer, get my decisions of an accessReview.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f82ea-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f82ea-153">JSON representation</span></span>

<span data-ttu-id="f82ea-154">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f82ea-154">Here is a JSON representation of the resource.</span></span>

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


