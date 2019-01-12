---
title: tipo de recurso de accessReviewDecision
description: No Windows Azure AD access analisa o recurso, o `accessReviewDecision` representa uma decisão de revisão de acesso do Azure AD de acesso de uma entidade específica.  Dentro de uma revisão de acesso ou uma instância de uma análise mais acesso recorrentes, há um `accessReviewDecision` por usuário revisado.  Por exemplo, se um grupo tem dois convidados e um não-convidado como membros e uma revisão de acesso de convidados é executada para esse grupo, e em seguida, haverá dois objetos de decisão de revisão de acesso.  Se um revisor altera sua decisão ou outro revisor substitui-los, em seguida, a `accessReviewDecision` é atualizado.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b6b10a53726e12c37a598f8df735a3f70174c807
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977553"
---
# <a name="accessreviewdecision-resource-type"></a><span data-ttu-id="a5705-106">tipo de recurso de accessReviewDecision</span><span class="sxs-lookup"><span data-stu-id="a5705-106">accessReviewDecision resource type</span></span>

> <span data-ttu-id="a5705-107">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a5705-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a5705-108">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a5705-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a5705-109">No recurso de [acesso analisa](accessreviews-root.md) Azure AD, o `accessReviewDecision` representa uma decisão de revisão de acesso do Azure AD de acesso de uma entidade específica.</span><span class="sxs-lookup"><span data-stu-id="a5705-109">In the Azure AD [access reviews](accessreviews-root.md) feature, the `accessReviewDecision` represents an Azure AD access review decision of a particular entity's access.</span></span>  <span data-ttu-id="a5705-110">Dentro de uma revisão de acesso ou uma instância de uma análise mais acesso recorrentes, há um `accessReviewDecision` por usuário revisado.</span><span class="sxs-lookup"><span data-stu-id="a5705-110">Within an access review, or an instance of a recurring access review, there is one `accessReviewDecision` per reviewed user.</span></span>  <span data-ttu-id="a5705-111">Por exemplo, se um grupo tem dois convidados e um não-convidado como membros e uma revisão de acesso de convidados é executada para esse grupo, e em seguida, haverá dois objetos de decisão de revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="a5705-111">For example, if a group has two guests and one non-guest as members, and an access review of guests is performed for that group, then there will be two access review decision objects.</span></span>  <span data-ttu-id="a5705-112">Se um revisor altera sua decisão ou outro revisor substitui-los, em seguida, a `accessReviewDecision` é atualizado.</span><span class="sxs-lookup"><span data-stu-id="a5705-112">If a reviewer changes their decision, or another reviewer overrides them, then the `accessReviewDecision` is updated.</span></span>


## <a name="methods"></a><span data-ttu-id="a5705-113">Métodos</span><span class="sxs-lookup"><span data-stu-id="a5705-113">Methods</span></span>

<span data-ttu-id="a5705-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a5705-114">None.</span></span>  <span data-ttu-id="a5705-115">Objetos desse tipo são criados automaticamente pelo recurso quando um acesso Revise inicializa e não podem ser excluídas.</span><span class="sxs-lookup"><span data-stu-id="a5705-115">Objects of this type are automatically created by the feature when an access review initializes, and cannot be deleted.</span></span>  <span data-ttu-id="a5705-116">Eles podem ser recuperados de uma revisão de acesso usando as relações de [decisões](../api/accessreview-listdecisions.md) e [mydecisions](../api/accessreview-listmydecisions.md) .</span><span class="sxs-lookup"><span data-stu-id="a5705-116">They can be retrieved from an access review using the [decisions](../api/accessreview-listdecisions.md) and [mydecisions](../api/accessreview-listmydecisions.md) relationships.</span></span>

## <a name="properties"></a><span data-ttu-id="a5705-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a5705-117">Properties</span></span>

<span data-ttu-id="a5705-118">Esta tabela ilustra as propriedades de base dos objetos desse tipo.</span><span class="sxs-lookup"><span data-stu-id="a5705-118">This table illustrates the base properties of objects of this type.</span></span> 

| <span data-ttu-id="a5705-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a5705-119">Property</span></span>                        | <span data-ttu-id="a5705-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="a5705-120">Type</span></span>                         | <span data-ttu-id="a5705-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5705-121">Description</span></span>                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `id`                            |`String`                      | <span data-ttu-id="a5705-122">A identificação da decisão dentro da revisão do access.</span><span class="sxs-lookup"><span data-stu-id="a5705-122">The id of the decision within the access review.</span></span>                                                                                     |
| `accessReviewId`                |`String`                      | <span data-ttu-id="a5705-123">A id da revisão acesso gerados pelo recurso.</span><span class="sxs-lookup"><span data-stu-id="a5705-123">The feature-generated id of the access review.</span></span>                                                                                       |
| `reviewedBy`                    |[<span data-ttu-id="a5705-124">userIdentity</span><span class="sxs-lookup"><span data-stu-id="a5705-124">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="a5705-125">A identidade do revisor.</span><span class="sxs-lookup"><span data-stu-id="a5705-125">The identity of the reviewer.</span></span>                                                                                       |
| `reviewedDate`                  |`DateTimeOffset`              | <span data-ttu-id="a5705-126">A data e hora da revisão mais recente para que isso direito de acesso foi fornecido.</span><span class="sxs-lookup"><span data-stu-id="a5705-126">The date and time the most recent review for this access right was supplied.</span></span>                                                                         |
| `reviewResult`                  |`String`                      | <span data-ttu-id="a5705-127">O resultado da revisão.</span><span class="sxs-lookup"><span data-stu-id="a5705-127">The result of the review.</span></span>                                                                                    |
| `justification`                 |`String`                      | <span data-ttu-id="a5705-128">Justificativa do revisor comercial, se fornecido.</span><span class="sxs-lookup"><span data-stu-id="a5705-128">The reviewer's business justification, if supplied.</span></span>                                                                         |
| `appliedBy`                     |[<span data-ttu-id="a5705-129">userIdentity</span><span class="sxs-lookup"><span data-stu-id="a5705-129">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="a5705-130">Quando a revisão completa, se os resultados foram aplicados manualmente, a identidade do usuário do usuário que é aplicado a decisão.</span><span class="sxs-lookup"><span data-stu-id="a5705-130">When the review completes, if the results were manually applied, the user identity of the user who applied the decision.</span></span>                                                           |
| `appliedDateTime`               |`DateTimeOffset`              | <span data-ttu-id="a5705-131">A data e a hora quando a decisão de revisão foi aplicada.</span><span class="sxs-lookup"><span data-stu-id="a5705-131">The date and time when the review decision was applied.</span></span>                                                          |
| `applyResult`                   |`String`                      | <span data-ttu-id="a5705-132">O resultado da aplicação a decisão, uma das `NotApplied`, `Success`, `Failed`, `NotFound` ou `NotSupported`.</span><span class="sxs-lookup"><span data-stu-id="a5705-132">The outcome of applying the decision, one of `NotApplied`, `Success`, `Failed`, `NotFound` or `NotSupported`.</span></span>                      |
| `accessRecommendation`          |`String`                      | <span data-ttu-id="a5705-133">A recomendação recurso-gerado mostrada ao revisor, uma das `Approve`, `Deny` ou `NotAvailable`.</span><span class="sxs-lookup"><span data-stu-id="a5705-133">The feature- generated recommendation shown to the reviewer, one of `Approve`, `Deny` or `NotAvailable`.</span></span> |


<span data-ttu-id="a5705-134">Além disso, as propriedades adicionais podem estar presentes dependendo do tipo de objeto do objeto com o access que foi decidido.</span><span class="sxs-lookup"><span data-stu-id="a5705-134">In addition, additional properties may be present depending on the object type of the object possessing the access that was decided upon.</span></span>  <span data-ttu-id="a5705-135">Por exemplo, se a decisão de revisão de acesso é a associação de grupo de um usuário específico ou acesso de aplicativo, o usuário que será potencialmente ter seu acesso a ser removida é identificado através dessas propriedades:</span><span class="sxs-lookup"><span data-stu-id="a5705-135">For example, if the access review decision is a particular user's group membership or application access, the user who is potentially going to have their access be removed is identified through these properties:</span></span>

| <span data-ttu-id="a5705-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a5705-136">Property</span></span>                        | <span data-ttu-id="a5705-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="a5705-137">Type</span></span>                         | <span data-ttu-id="a5705-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5705-138">Description</span></span>                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `userId`                            |`String`                      | <span data-ttu-id="a5705-139">A id de usuário cujo acesso foi examinado.</span><span class="sxs-lookup"><span data-stu-id="a5705-139">The id of user whose access was reviewed.</span></span>                                                                                    |
| `userDisplayName`                            |`String`                      | <span data-ttu-id="a5705-140">O nome de exibição do usuário cujo acesso foi examinado.</span><span class="sxs-lookup"><span data-stu-id="a5705-140">The display name of the user whose access was reviewed.</span></span>                                                                                     |
| `userPrincipalName`                            |`String`                      | <span data-ttu-id="a5705-141">O nome principal de usuário do usuário cujo acesso foi examinado.</span><span class="sxs-lookup"><span data-stu-id="a5705-141">The user principal name of the user whose access was reviewed.</span></span>                                                                                     |



## <a name="relationships"></a><span data-ttu-id="a5705-142">Relações</span><span class="sxs-lookup"><span data-stu-id="a5705-142">Relationships</span></span>

<span data-ttu-id="a5705-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a5705-143">None.</span></span>  <span data-ttu-id="a5705-144">Objetos desse tipo podem ser recuperados de uma revisão de acesso usando as relações de [decisões](../api/accessreview-listdecisions.md) e [mydecisions](../api/accessreview-listmydecisions.md) do objeto [accessReview](accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="a5705-144">Objects of this type can be retrieved from an access review using the [decisions](../api/accessreview-listdecisions.md) and [mydecisions](../api/accessreview-listmydecisions.md) relationships of the [accessReview](accessreview.md) object.</span></span>

## <a name="see-also"></a><span data-ttu-id="a5705-145">Confira também</span><span class="sxs-lookup"><span data-stu-id="a5705-145">See also</span></span>

| <span data-ttu-id="a5705-146">Método</span><span class="sxs-lookup"><span data-stu-id="a5705-146">Method</span></span>           | <span data-ttu-id="a5705-147">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a5705-147">Return Type</span></span>    |<span data-ttu-id="a5705-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5705-148">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a5705-149">Lista accessReview decisões</span><span class="sxs-lookup"><span data-stu-id="a5705-149">List accessReview decisions</span></span>](../api/accessreview-listdecisions.md) |      <span data-ttu-id="a5705-150">coleção [accessReviewDecision](accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="a5705-150">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="a5705-151">Obtenha as decisões de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="a5705-151">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="a5705-152">Listar meus decisões accessReview</span><span class="sxs-lookup"><span data-stu-id="a5705-152">List my accessReview decisions</span></span>](../api/accessreview-listmydecisions.md) |     <span data-ttu-id="a5705-153">coleção [accessReviewDecision](accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="a5705-153">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="a5705-154">Como um revisor, obtenha Minhas decisões de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="a5705-154">As a reviewer, get my decisions of an accessReview.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a5705-155">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a5705-155">JSON representation</span></span>

<span data-ttu-id="a5705-156">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a5705-156">Here is a JSON representation of the resource.</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "accessReviewDecision resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
