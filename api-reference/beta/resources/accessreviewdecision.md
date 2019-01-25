---
title: tipo de recurso de accessReviewDecision
description: No Windows Azure AD access analisa o recurso, o `accessReviewDecision` representa uma decisão de revisão de acesso do Azure AD de acesso de uma entidade específica.  Dentro de uma revisão de acesso ou uma instância de uma análise mais acesso recorrentes, há um `accessReviewDecision` por usuário revisado.  Por exemplo, se um grupo tem dois convidados e um não-convidado como membros e uma revisão de acesso de convidados é executada para esse grupo, e em seguida, haverá dois objetos de decisão de revisão de acesso.  Se um revisor altera sua decisão ou outro revisor substitui-los, em seguida, a `accessReviewDecision` é atualizado.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9642c8a51e4e9efe1a1748243b0e24aeff07cfa0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517397"
---
# <a name="accessreviewdecision-resource-type"></a><span data-ttu-id="cd0e5-106">tipo de recurso de accessReviewDecision</span><span class="sxs-lookup"><span data-stu-id="cd0e5-106">accessReviewDecision resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd0e5-107">No recurso de [acesso analisa](accessreviews-root.md) Azure AD, o `accessReviewDecision` representa uma decisão de revisão de acesso do Azure AD de acesso de uma entidade específica.</span><span class="sxs-lookup"><span data-stu-id="cd0e5-107">In the Azure AD [access reviews](accessreviews-root.md) feature, the `accessReviewDecision` represents an Azure AD access review decision of a particular entity's access.</span></span>  <span data-ttu-id="cd0e5-108">Dentro de uma revisão de acesso ou uma instância de uma análise mais acesso recorrentes, há um `accessReviewDecision` por usuário revisado.</span><span class="sxs-lookup"><span data-stu-id="cd0e5-108">Within an access review, or an instance of a recurring access review, there is one `accessReviewDecision` per reviewed user.</span></span>  <span data-ttu-id="cd0e5-109">Por exemplo, se um grupo tem dois convidados e um não-convidado como membros e uma revisão de acesso de convidados é executada para esse grupo, e em seguida, haverá dois objetos de decisão de revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="cd0e5-109">For example, if a group has two guests and one non-guest as members, and an access review of guests is performed for that group, then there will be two access review decision objects.</span></span>  <span data-ttu-id="cd0e5-110">Se um revisor altera sua decisão ou outro revisor substitui-los, em seguida, a `accessReviewDecision` é atualizado.</span><span class="sxs-lookup"><span data-stu-id="cd0e5-110">If a reviewer changes their decision, or another reviewer overrides them, then the `accessReviewDecision` is updated.</span></span>


## <a name="methods"></a><span data-ttu-id="cd0e5-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="cd0e5-111">Methods</span></span>

<span data-ttu-id="cd0e5-112">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="cd0e5-112">None.</span></span>  <span data-ttu-id="cd0e5-113">Objetos desse tipo são criados automaticamente pelo recurso quando um acesso Revise inicializa e não podem ser excluídas.</span><span class="sxs-lookup"><span data-stu-id="cd0e5-113">Objects of this type are automatically created by the feature when an access review initializes, and cannot be deleted.</span></span>  <span data-ttu-id="cd0e5-114">Eles podem ser recuperados de uma revisão de acesso usando as relações de [decisões](../api/accessreview-listdecisions.md) e [mydecisions](../api/accessreview-listmydecisions.md) .</span><span class="sxs-lookup"><span data-stu-id="cd0e5-114">They can be retrieved from an access review using the [decisions](../api/accessreview-listdecisions.md) and [mydecisions](../api/accessreview-listmydecisions.md) relationships.</span></span>

## <a name="properties"></a><span data-ttu-id="cd0e5-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cd0e5-115">Properties</span></span>

<span data-ttu-id="cd0e5-116">Esta tabela ilustra as propriedades de base dos objetos desse tipo.</span><span class="sxs-lookup"><span data-stu-id="cd0e5-116">This table illustrates the base properties of objects of this type.</span></span> 

| <span data-ttu-id="cd0e5-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cd0e5-117">Property</span></span>                        | <span data-ttu-id="cd0e5-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="cd0e5-118">Type</span></span>                         | <span data-ttu-id="cd0e5-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd0e5-119">Description</span></span>                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `id`                            |`String`                      | <span data-ttu-id="cd0e5-120">A identificação da decisão dentro da revisão do access.</span><span class="sxs-lookup"><span data-stu-id="cd0e5-120">The id of the decision within the access review.</span></span>                                                                                     |
| `accessReviewId`                |`String`                      | <span data-ttu-id="cd0e5-121">A id da revisão acesso gerados pelo recurso.</span><span class="sxs-lookup"><span data-stu-id="cd0e5-121">The feature-generated id of the access review.</span></span>                                                                                       |
| `reviewedBy`                    |[<span data-ttu-id="cd0e5-122">userIdentity</span><span class="sxs-lookup"><span data-stu-id="cd0e5-122">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="cd0e5-123">A identidade do revisor.</span><span class="sxs-lookup"><span data-stu-id="cd0e5-123">The identity of the reviewer.</span></span>                                                                                       |
| `reviewedDate`                  |`DateTimeOffset`              | <span data-ttu-id="cd0e5-124">A data e hora da revisão mais recente para que isso direito de acesso foi fornecido.</span><span class="sxs-lookup"><span data-stu-id="cd0e5-124">The date and time the most recent review for this access right was supplied.</span></span>                                                                         |
| `reviewResult`                  |`String`                      | <span data-ttu-id="cd0e5-125">O resultado da revisão.</span><span class="sxs-lookup"><span data-stu-id="cd0e5-125">The result of the review.</span></span>                                                                                    |
| `justification`                 |`String`                      | <span data-ttu-id="cd0e5-126">Justificativa do revisor comercial, se fornecido.</span><span class="sxs-lookup"><span data-stu-id="cd0e5-126">The reviewer's business justification, if supplied.</span></span>                                                                         |
| `appliedBy`                     |[<span data-ttu-id="cd0e5-127">userIdentity</span><span class="sxs-lookup"><span data-stu-id="cd0e5-127">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="cd0e5-128">Quando a revisão completa, se os resultados foram aplicados manualmente, a identidade do usuário do usuário que é aplicado a decisão.</span><span class="sxs-lookup"><span data-stu-id="cd0e5-128">When the review completes, if the results were manually applied, the user identity of the user who applied the decision.</span></span>                                                           |
| `appliedDateTime`               |`DateTimeOffset`              | <span data-ttu-id="cd0e5-129">A data e a hora quando a decisão de revisão foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="cd0e5-129">The date and time when the review decision was applied.</span></span>                                                          |
| `applyResult`                   |`String`                      | <span data-ttu-id="cd0e5-130">O resultado da aplicação a decisão, uma das `NotApplied`, `Success`, `Failed`, `NotFound` ou `NotSupported`.</span><span class="sxs-lookup"><span data-stu-id="cd0e5-130">The outcome of applying the decision, one of `NotApplied`, `Success`, `Failed`, `NotFound` or `NotSupported`.</span></span>                      |
| `accessRecommendation`          |`String`                      | <span data-ttu-id="cd0e5-131">A recomendação recurso-gerado mostrada ao revisor, uma das `Approve`, `Deny` ou `NotAvailable`.</span><span class="sxs-lookup"><span data-stu-id="cd0e5-131">The feature- generated recommendation shown to the reviewer, one of `Approve`, `Deny` or `NotAvailable`.</span></span> |


<span data-ttu-id="cd0e5-132">Além disso, as propriedades adicionais podem estar presentes dependendo do tipo de objeto do objeto com o access que foi decidido.</span><span class="sxs-lookup"><span data-stu-id="cd0e5-132">In addition, additional properties may be present depending on the object type of the object possessing the access that was decided upon.</span></span>  <span data-ttu-id="cd0e5-133">Por exemplo, se a decisão de revisão de acesso é a associação de grupo de um usuário específico ou acesso de aplicativo, o usuário que será potencialmente ter seu acesso a ser removida é identificado através dessas propriedades:</span><span class="sxs-lookup"><span data-stu-id="cd0e5-133">For example, if the access review decision is a particular user's group membership or application access, the user who is potentially going to have their access be removed is identified through these properties:</span></span>

| <span data-ttu-id="cd0e5-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cd0e5-134">Property</span></span>                        | <span data-ttu-id="cd0e5-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="cd0e5-135">Type</span></span>                         | <span data-ttu-id="cd0e5-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd0e5-136">Description</span></span>                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `userId`                            |`String`                      | <span data-ttu-id="cd0e5-137">A id de usuário cujo acesso foi examinado.</span><span class="sxs-lookup"><span data-stu-id="cd0e5-137">The id of user whose access was reviewed.</span></span>                                                                                    |
| `userDisplayName`                            |`String`                      | <span data-ttu-id="cd0e5-138">O nome de exibição do usuário cujo acesso foi examinado.</span><span class="sxs-lookup"><span data-stu-id="cd0e5-138">The display name of the user whose access was reviewed.</span></span>                                                                                     |
| `userPrincipalName`                            |`String`                      | <span data-ttu-id="cd0e5-139">O nome principal de usuário do usuário cujo acesso foi examinado.</span><span class="sxs-lookup"><span data-stu-id="cd0e5-139">The user principal name of the user whose access was reviewed.</span></span>                                                                                     |



## <a name="relationships"></a><span data-ttu-id="cd0e5-140">Relações</span><span class="sxs-lookup"><span data-stu-id="cd0e5-140">Relationships</span></span>

<span data-ttu-id="cd0e5-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cd0e5-141">None.</span></span>  <span data-ttu-id="cd0e5-142">Objetos desse tipo podem ser recuperados de uma revisão de acesso usando as relações de [decisões](../api/accessreview-listdecisions.md) e [mydecisions](../api/accessreview-listmydecisions.md) do objeto [accessReview](accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="cd0e5-142">Objects of this type can be retrieved from an access review using the [decisions](../api/accessreview-listdecisions.md) and [mydecisions](../api/accessreview-listmydecisions.md) relationships of the [accessReview](accessreview.md) object.</span></span>

## <a name="see-also"></a><span data-ttu-id="cd0e5-143">Confira também</span><span class="sxs-lookup"><span data-stu-id="cd0e5-143">See also</span></span>

| <span data-ttu-id="cd0e5-144">Método</span><span class="sxs-lookup"><span data-stu-id="cd0e5-144">Method</span></span>           | <span data-ttu-id="cd0e5-145">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="cd0e5-145">Return Type</span></span>    |<span data-ttu-id="cd0e5-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd0e5-146">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cd0e5-147">Lista accessReview decisões</span><span class="sxs-lookup"><span data-stu-id="cd0e5-147">List accessReview decisions</span></span>](../api/accessreview-listdecisions.md) |      <span data-ttu-id="cd0e5-148">coleção [accessReviewDecision](accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="cd0e5-148">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="cd0e5-149">Obtenha as decisões de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="cd0e5-149">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="cd0e5-150">Listar meus decisões accessReview</span><span class="sxs-lookup"><span data-stu-id="cd0e5-150">List my accessReview decisions</span></span>](../api/accessreview-listmydecisions.md) |     <span data-ttu-id="cd0e5-151">coleção [accessReviewDecision](accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="cd0e5-151">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="cd0e5-152">Como um revisor, obtenha Minhas decisões de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="cd0e5-152">As a reviewer, get my decisions of an accessReview.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cd0e5-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cd0e5-153">JSON representation</span></span>

<span data-ttu-id="cd0e5-154">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cd0e5-154">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/accessreviewdecision.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
