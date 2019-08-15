---
title: Obter accessReview
description: 'No recurso de revisões do Azure AD Access, recupere um objeto accessReview.  '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f8e628c2ba8835d42f00116e46b4dfa0527765fe
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36408830"
---
# <a name="get-accessreview"></a><span data-ttu-id="dbcfc-103">Obter accessReview</span><span class="sxs-lookup"><span data-stu-id="dbcfc-103">Get accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dbcfc-104">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , recupere um objeto [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="dbcfc-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve an [accessReview](../resources/accessreview.md) object.</span></span>  

<span data-ttu-id="dbcfc-105">Para recuperar os revisores da revisão do Access, use a API [list accessReview](accessreview-listreviewers.md) reviewers.</span><span class="sxs-lookup"><span data-stu-id="dbcfc-105">To retrieve the reviewers of the access review, use the [list accessReview reviewers](accessreview-listreviewers.md) API.</span></span> <span data-ttu-id="dbcfc-106">Para recuperar as decisões da revisão de acesso, use a API de [accessReview decisions](accessreview-listdecisions.md) ou a API [list My accessReview decisions](accessreview-listmydecisions.md) .</span><span class="sxs-lookup"><span data-stu-id="dbcfc-106">To retrieve the decisions of the access review, use the [list accessReview decisions](accessreview-listdecisions.md) API, or the [list my accessReview decisions](accessreview-listmydecisions.md) API.</span></span>

<span data-ttu-id="dbcfc-107">Se esta for uma revisão de acesso recorrente, use a `instances` relação para recuperar uma coleção [accessReview](../resources/accessreview.md) das instâncias passadas, atual e futura da revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="dbcfc-107">If this is a recurring access review, then use the `instances` relationship to retrieve an [accessReview](../resources/accessreview.md) collection of the past, current, and future instances of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="dbcfc-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="dbcfc-108">Permissions</span></span>
<span data-ttu-id="dbcfc-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dbcfc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dbcfc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dbcfc-111">Permission type</span></span>                        | <span data-ttu-id="dbcfc-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dbcfc-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="dbcfc-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dbcfc-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="dbcfc-114">AccessReview. Read. All, AccessReview. ReadWrite. Membership, AccessReview. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="dbcfc-114">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="dbcfc-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dbcfc-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dbcfc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dbcfc-116">Not supported.</span></span> |
|<span data-ttu-id="dbcfc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dbcfc-117">Application</span></span>                            | <span data-ttu-id="dbcfc-118">AccessReview. Read. All, AccessReview. ReadWrite. Membership</span><span class="sxs-lookup"><span data-stu-id="dbcfc-118">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span>  |

<span data-ttu-id="dbcfc-119">Para chamar essa API, o usuário conectado também deve estar em uma função de diretório que permite que ele leia uma revisão do Access ou que o usuário possa ser atribuído como um revisor na revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="dbcfc-119">In order to call this API, the signed in user must also be in a directory role that permits them to read an access review, or the user can be assigned as a reviewer on the access review.</span></span>  <span data-ttu-id="dbcfc-120">Para obter mais detalhes, consulte a função e os requisitos de permissão para [revisões do Access](../resources/accessreviews-root.md).</span><span class="sxs-lookup"><span data-stu-id="dbcfc-120">For more details, see the role and permission requirements for [access reviews](../resources/accessreviews-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="dbcfc-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dbcfc-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews/{reviewId}
```
## <a name="request-headers"></a><span data-ttu-id="dbcfc-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dbcfc-122">Request headers</span></span>
| <span data-ttu-id="dbcfc-123">Nome</span><span class="sxs-lookup"><span data-stu-id="dbcfc-123">Name</span></span>         | <span data-ttu-id="dbcfc-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="dbcfc-124">Type</span></span>        | <span data-ttu-id="dbcfc-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="dbcfc-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="dbcfc-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="dbcfc-126">Authorization</span></span> | <span data-ttu-id="dbcfc-127">string</span><span class="sxs-lookup"><span data-stu-id="dbcfc-127">string</span></span> | <span data-ttu-id="dbcfc-p104">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dbcfc-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dbcfc-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dbcfc-130">Request body</span></span>
<span data-ttu-id="dbcfc-131">Nenhum corpo de solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="dbcfc-131">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="dbcfc-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbcfc-132">Response</span></span>
<span data-ttu-id="dbcfc-133">Se tiver êxito, este método retornará `200, OK` um código de resposta e um objeto [accessReview](../resources/accessreview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dbcfc-133">If successful, this method returns a `200, OK` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dbcfc-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dbcfc-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dbcfc-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dbcfc-135">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="dbcfc-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="dbcfc-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReview"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dbcfc-137">C#</span><span class="sxs-lookup"><span data-stu-id="dbcfc-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dbcfc-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dbcfc-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dbcfc-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="dbcfc-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="dbcfc-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbcfc-140">Response</span></span>
><span data-ttu-id="dbcfc-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dbcfc-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReview",
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "2b83cc42-09db-46f6-8c6e-16fec466a82d",
    "displayName": "review",
    "startDateTime": "2017-11-14T01:14:54.89Z",
    "endDateTime": "2017-12-14T01:14:54.89Z",
    "status": "InProgress",
    "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "reviewerType": "self",
    "description": "",
    "reviewedEntity":{"id":"3b4f7e74-eb82-4120-9ff5-ba429c1ea6df","displayName":"Salesforce"},
    "settings": {
        "mailNotificationsEnabled": true,
        "remindersEnabled": true,
        "justificationRequiredOnApproval": true,
        "autoReviewEnabled": false,
        "activityDurationInDays": 30,
        "autoApplyReviewResultsEnabled": false,
        "accessRecommendationsEnabled": false,
        "recurrenceSettings": {
            "recurrenceType": "onetime",
            "recurrenceEndType": "endBy",
            "durationInDays": 0,
            "recurrenceCount": 0
        },
        "autoReviewSettings": {
            "notReviewedResult": "Deny"
        }
    }
}
```

## <a name="see-also"></a><span data-ttu-id="dbcfc-143">Confira também</span><span class="sxs-lookup"><span data-stu-id="dbcfc-143">See also</span></span>

| <span data-ttu-id="dbcfc-144">Método</span><span class="sxs-lookup"><span data-stu-id="dbcfc-144">Method</span></span>           | <span data-ttu-id="dbcfc-145">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="dbcfc-145">Return Type</span></span>    |<span data-ttu-id="dbcfc-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="dbcfc-146">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="dbcfc-147">Criar accessReview</span><span class="sxs-lookup"><span data-stu-id="dbcfc-147">Create accessReview</span></span>](accessreview-create.md) |    [<span data-ttu-id="dbcfc-148">accessReview</span><span class="sxs-lookup"><span data-stu-id="dbcfc-148">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="dbcfc-149">Criar um novo accessReview.</span><span class="sxs-lookup"><span data-stu-id="dbcfc-149">Create a new accessReview.</span></span> |
|[<span data-ttu-id="dbcfc-150">Listar programControls</span><span class="sxs-lookup"><span data-stu-id="dbcfc-150">List programControls</span></span>](programcontrol-list.md) | <span data-ttu-id="dbcfc-151">coleção [programControl](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="dbcfc-151">[programControl](../resources/programcontrol.md) collection</span></span> | <span data-ttu-id="dbcfc-152">Listar programControls em um locatário.</span><span class="sxs-lookup"><span data-stu-id="dbcfc-152">List programControls in a tenant.</span></span> |
|[<span data-ttu-id="dbcfc-153">Listar revisores do accessReview</span><span class="sxs-lookup"><span data-stu-id="dbcfc-153">List accessReview reviewers</span></span>](accessreview-listreviewers.md) |     <span data-ttu-id="dbcfc-154">[](../resources/useridentity.md) coleção UserIdentity</span><span class="sxs-lookup"><span data-stu-id="dbcfc-154">[userIdentity](../resources/useridentity.md) collection</span></span>|    <span data-ttu-id="dbcfc-155">Obter os revisores de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="dbcfc-155">Get the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="dbcfc-156">Listar decisões accessReview</span><span class="sxs-lookup"><span data-stu-id="dbcfc-156">List accessReview decisions</span></span>](accessreview-listdecisions.md) |     <span data-ttu-id="dbcfc-157">coleção [accessReviewDecision](../resources/accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="dbcfc-157">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="dbcfc-158">Obtenha as decisões de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="dbcfc-158">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="dbcfc-159">Listar minhas decisões do accessReview</span><span class="sxs-lookup"><span data-stu-id="dbcfc-159">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="dbcfc-160">coleção [accessReviewDecision](../resources/accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="dbcfc-160">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="dbcfc-161">Como revisor, obtenha as minhas decisões de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="dbcfc-161">As a reviewer, get my decisions of an accessReview.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
