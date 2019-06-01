---
title: Obter accessReview
description: 'No recurso de revisões do Azure AD Access, recupere um objeto accessReview.  '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3953efad278fed3eb3010da38d18f3aae8286b45
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2019
ms.locfileid: "34655492"
---
# <a name="get-accessreview"></a><span data-ttu-id="3e6a0-103">Obter accessReview</span><span class="sxs-lookup"><span data-stu-id="3e6a0-103">Get accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e6a0-104">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , recupere um objeto [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="3e6a0-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve an [accessReview](../resources/accessreview.md) object.</span></span>  

<span data-ttu-id="3e6a0-105">Para recuperar os revisores da revisão do Access, use a API [list accessReview](accessreview-listreviewers.md) reviewers.</span><span class="sxs-lookup"><span data-stu-id="3e6a0-105">To retrieve the reviewers of the access review, use the [list accessReview reviewers](accessreview-listreviewers.md) API.</span></span> <span data-ttu-id="3e6a0-106">Para recuperar as decisões da revisão de acesso, use a API de [accessReview decisions](accessreview-listdecisions.md) ou a API [list My accessReview decisions](accessreview-listmydecisions.md) .</span><span class="sxs-lookup"><span data-stu-id="3e6a0-106">To retrieve the decisions of the access review, use the [list accessReview decisions](accessreview-listdecisions.md) API, or the [list my accessReview decisions](accessreview-listmydecisions.md) API.</span></span>

<span data-ttu-id="3e6a0-107">Se esta for uma revisão de acesso recorrente, use a `instances` relação para recuperar uma coleção [accessReview](../resources/accessreview.md) das instâncias passadas, atual e futura da revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="3e6a0-107">If this is a recurring access review, then use the `instances` relationship to retrieve an [accessReview](../resources/accessreview.md) collection of the past, current, and future instances of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="3e6a0-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="3e6a0-108">Permissions</span></span>
<span data-ttu-id="3e6a0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e6a0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e6a0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3e6a0-111">Permission type</span></span>                        | <span data-ttu-id="3e6a0-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3e6a0-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e6a0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3e6a0-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="3e6a0-114">AccessReview.Read.All</span><span class="sxs-lookup"><span data-stu-id="3e6a0-114">AccessReview.Read.All</span></span>  |
|<span data-ttu-id="3e6a0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3e6a0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e6a0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3e6a0-116">Not supported.</span></span> |
|<span data-ttu-id="3e6a0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3e6a0-117">Application</span></span>                            | <span data-ttu-id="3e6a0-118">AccessReview.Read.All</span><span class="sxs-lookup"><span data-stu-id="3e6a0-118">AccessReview.Read.All</span></span>  |

<span data-ttu-id="3e6a0-119">Para chamar essa API, o usuário conectado também deve estar em uma função de diretório que permite que ele leia uma revisão do Access ou que o usuário possa ser atribuído como um revisor na revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="3e6a0-119">In order to call this API, the signed in user must also be in a directory role that permits them to read an access review, or the user can be assigned as a reviewer on the access review.</span></span>  <span data-ttu-id="3e6a0-120">Para obter mais detalhes, consulte a função e os requisitos de permissão para [revisões do Access](../resources/accessreviews-root.md).</span><span class="sxs-lookup"><span data-stu-id="3e6a0-120">For more details, see the role and permission requirements for [access reviews](../resources/accessreviews-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="3e6a0-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3e6a0-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')
```
## <a name="request-headers"></a><span data-ttu-id="3e6a0-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3e6a0-122">Request headers</span></span>
| <span data-ttu-id="3e6a0-123">Nome</span><span class="sxs-lookup"><span data-stu-id="3e6a0-123">Name</span></span>         | <span data-ttu-id="3e6a0-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="3e6a0-124">Type</span></span>        | <span data-ttu-id="3e6a0-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e6a0-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="3e6a0-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="3e6a0-126">Authorization</span></span> | <span data-ttu-id="3e6a0-127">string</span><span class="sxs-lookup"><span data-stu-id="3e6a0-127">string</span></span> | <span data-ttu-id="3e6a0-p104">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3e6a0-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3e6a0-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3e6a0-130">Request body</span></span>
<span data-ttu-id="3e6a0-131">Nenhum corpo de solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="3e6a0-131">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="3e6a0-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e6a0-132">Response</span></span>
<span data-ttu-id="3e6a0-133">Se tiver êxito, este método retornará `200, OK` um código de resposta e um objeto [accessReview](../resources/accessreview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3e6a0-133">If successful, this method returns a `200, OK` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e6a0-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3e6a0-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3e6a0-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3e6a0-135">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d
```

##### <a name="response"></a><span data-ttu-id="3e6a0-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e6a0-136">Response</span></span>
><span data-ttu-id="3e6a0-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3e6a0-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="3e6a0-139">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="3e6a0-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3e6a0-140">C#</span><span class="sxs-lookup"><span data-stu-id="3e6a0-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_accessReview-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3e6a0-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="3e6a0-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_accessReview-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="3e6a0-142">Confira também</span><span class="sxs-lookup"><span data-stu-id="3e6a0-142">See also</span></span>

| <span data-ttu-id="3e6a0-143">Método</span><span class="sxs-lookup"><span data-stu-id="3e6a0-143">Method</span></span>           | <span data-ttu-id="3e6a0-144">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3e6a0-144">Return Type</span></span>    |<span data-ttu-id="3e6a0-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e6a0-145">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3e6a0-146">Criar accessReview</span><span class="sxs-lookup"><span data-stu-id="3e6a0-146">Create accessReview</span></span>](accessreview-create.md) |    [<span data-ttu-id="3e6a0-147">accessReview</span><span class="sxs-lookup"><span data-stu-id="3e6a0-147">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="3e6a0-148">Criar um novo accessReview.</span><span class="sxs-lookup"><span data-stu-id="3e6a0-148">Create a new accessReview.</span></span> |
|[<span data-ttu-id="3e6a0-149">Listar programControls</span><span class="sxs-lookup"><span data-stu-id="3e6a0-149">List programControls</span></span>](programcontrol-list.md) | <span data-ttu-id="3e6a0-150">coleção [programControl](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="3e6a0-150">[programControl](../resources/programcontrol.md) collection</span></span> | <span data-ttu-id="3e6a0-151">Listar programControls em um locatário.</span><span class="sxs-lookup"><span data-stu-id="3e6a0-151">List programControls in a tenant.</span></span> |
|[<span data-ttu-id="3e6a0-152">Listar revisores do accessReview</span><span class="sxs-lookup"><span data-stu-id="3e6a0-152">List accessReview reviewers</span></span>](accessreview-listreviewers.md) |     <span data-ttu-id="3e6a0-153">[](../resources/useridentity.md) coleção UserIdentity</span><span class="sxs-lookup"><span data-stu-id="3e6a0-153">[userIdentity](../resources/useridentity.md) collection</span></span>|    <span data-ttu-id="3e6a0-154">Obter os revisores de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="3e6a0-154">Get the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="3e6a0-155">Listar decisões accessReview</span><span class="sxs-lookup"><span data-stu-id="3e6a0-155">List accessReview decisions</span></span>](accessreview-listdecisions.md) |     <span data-ttu-id="3e6a0-156">coleção [accessReviewDecision](../resources/accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="3e6a0-156">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="3e6a0-157">Obtenha as decisões de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="3e6a0-157">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="3e6a0-158">Listar minhas decisões do accessReview</span><span class="sxs-lookup"><span data-stu-id="3e6a0-158">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="3e6a0-159">coleção [accessReviewDecision](../resources/accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="3e6a0-159">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="3e6a0-160">Como revisor, obtenha as minhas decisões de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="3e6a0-160">As a reviewer, get my decisions of an accessReview.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/accessreview-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
