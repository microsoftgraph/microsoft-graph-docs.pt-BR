---
title: Obter accessReview
description: 'No recurso de revisões do Azure AD Access, recupere um objeto accessReview.  '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a274766eb51b2b4fde1cfa35fe3a88188a586ef4
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36316112"
---
# <a name="get-accessreview"></a><span data-ttu-id="367ee-103">Obter accessReview</span><span class="sxs-lookup"><span data-stu-id="367ee-103">Get accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="367ee-104">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , recupere um objeto [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="367ee-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve an [accessReview](../resources/accessreview.md) object.</span></span>  

<span data-ttu-id="367ee-105">Para recuperar os revisores da revisão do Access, use a API [list accessReview](accessreview-listreviewers.md) reviewers.</span><span class="sxs-lookup"><span data-stu-id="367ee-105">To retrieve the reviewers of the access review, use the [list accessReview reviewers](accessreview-listreviewers.md) API.</span></span> <span data-ttu-id="367ee-106">Para recuperar as decisões da revisão de acesso, use a API de [accessReview decisions](accessreview-listdecisions.md) ou a API [list My accessReview decisions](accessreview-listmydecisions.md) .</span><span class="sxs-lookup"><span data-stu-id="367ee-106">To retrieve the decisions of the access review, use the [list accessReview decisions](accessreview-listdecisions.md) API, or the [list my accessReview decisions](accessreview-listmydecisions.md) API.</span></span>

<span data-ttu-id="367ee-107">Se esta for uma revisão de acesso recorrente, use a `instances` relação para recuperar uma coleção [accessReview](../resources/accessreview.md) das instâncias passadas, atual e futura da revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="367ee-107">If this is a recurring access review, then use the `instances` relationship to retrieve an [accessReview](../resources/accessreview.md) collection of the past, current, and future instances of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="367ee-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="367ee-108">Permissions</span></span>
<span data-ttu-id="367ee-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="367ee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="367ee-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="367ee-111">Permission type</span></span>                        | <span data-ttu-id="367ee-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="367ee-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="367ee-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="367ee-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="367ee-114">AccessReview. Read. All, AccessReview. ReadWrite. Membership, AccessReview. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="367ee-114">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="367ee-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="367ee-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="367ee-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="367ee-116">Not supported.</span></span> |
|<span data-ttu-id="367ee-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="367ee-117">Application</span></span>                            | <span data-ttu-id="367ee-118">AccessReview. Read. All, AccessReview. ReadWrite. Membership</span><span class="sxs-lookup"><span data-stu-id="367ee-118">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span>  |

<span data-ttu-id="367ee-119">Para chamar essa API, o usuário conectado também deve estar em uma função de diretório que permite que ele leia uma revisão do Access ou que o usuário possa ser atribuído como um revisor na revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="367ee-119">In order to call this API, the signed in user must also be in a directory role that permits them to read an access review, or the user can be assigned as a reviewer on the access review.</span></span>  <span data-ttu-id="367ee-120">Para obter mais detalhes, consulte a função e os requisitos de permissão para [revisões do Access](../resources/accessreviews-root.md).</span><span class="sxs-lookup"><span data-stu-id="367ee-120">For more details, see the role and permission requirements for [access reviews](../resources/accessreviews-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="367ee-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="367ee-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')
```
## <a name="request-headers"></a><span data-ttu-id="367ee-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="367ee-122">Request headers</span></span>
| <span data-ttu-id="367ee-123">Nome</span><span class="sxs-lookup"><span data-stu-id="367ee-123">Name</span></span>         | <span data-ttu-id="367ee-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="367ee-124">Type</span></span>        | <span data-ttu-id="367ee-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="367ee-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="367ee-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="367ee-126">Authorization</span></span> | <span data-ttu-id="367ee-127">string</span><span class="sxs-lookup"><span data-stu-id="367ee-127">string</span></span> | <span data-ttu-id="367ee-p104">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="367ee-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="367ee-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="367ee-130">Request body</span></span>
<span data-ttu-id="367ee-131">Nenhum corpo de solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="367ee-131">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="367ee-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="367ee-132">Response</span></span>
<span data-ttu-id="367ee-133">Se tiver êxito, este método retornará `200, OK` um código de resposta e um objeto [accessReview](../resources/accessreview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="367ee-133">If successful, this method returns a `200, OK` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="367ee-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="367ee-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="367ee-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="367ee-135">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="367ee-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="367ee-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReview"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="367ee-137">C#</span><span class="sxs-lookup"><span data-stu-id="367ee-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="367ee-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="367ee-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="367ee-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="367ee-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="367ee-140">Java</span><span class="sxs-lookup"><span data-stu-id="367ee-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="367ee-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="367ee-141">Response</span></span>
><span data-ttu-id="367ee-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="367ee-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="367ee-144">Confira também</span><span class="sxs-lookup"><span data-stu-id="367ee-144">See also</span></span>

| <span data-ttu-id="367ee-145">Método</span><span class="sxs-lookup"><span data-stu-id="367ee-145">Method</span></span>           | <span data-ttu-id="367ee-146">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="367ee-146">Return Type</span></span>    |<span data-ttu-id="367ee-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="367ee-147">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="367ee-148">Criar accessReview</span><span class="sxs-lookup"><span data-stu-id="367ee-148">Create accessReview</span></span>](accessreview-create.md) |    [<span data-ttu-id="367ee-149">accessReview</span><span class="sxs-lookup"><span data-stu-id="367ee-149">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="367ee-150">Criar um novo accessReview.</span><span class="sxs-lookup"><span data-stu-id="367ee-150">Create a new accessReview.</span></span> |
|[<span data-ttu-id="367ee-151">Listar programControls</span><span class="sxs-lookup"><span data-stu-id="367ee-151">List programControls</span></span>](programcontrol-list.md) | <span data-ttu-id="367ee-152">coleção [programControl](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="367ee-152">[programControl](../resources/programcontrol.md) collection</span></span> | <span data-ttu-id="367ee-153">Listar programControls em um locatário.</span><span class="sxs-lookup"><span data-stu-id="367ee-153">List programControls in a tenant.</span></span> |
|[<span data-ttu-id="367ee-154">Listar revisores do accessReview</span><span class="sxs-lookup"><span data-stu-id="367ee-154">List accessReview reviewers</span></span>](accessreview-listreviewers.md) |     <span data-ttu-id="367ee-155">[](../resources/useridentity.md) coleção UserIdentity</span><span class="sxs-lookup"><span data-stu-id="367ee-155">[userIdentity](../resources/useridentity.md) collection</span></span>|    <span data-ttu-id="367ee-156">Obter os revisores de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="367ee-156">Get the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="367ee-157">Listar decisões accessReview</span><span class="sxs-lookup"><span data-stu-id="367ee-157">List accessReview decisions</span></span>](accessreview-listdecisions.md) |     <span data-ttu-id="367ee-158">coleção [accessReviewDecision](../resources/accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="367ee-158">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="367ee-159">Obtenha as decisões de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="367ee-159">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="367ee-160">Listar minhas decisões do accessReview</span><span class="sxs-lookup"><span data-stu-id="367ee-160">List my accessReview decisions</span></span>](accessreview-listmydecisions.md) |        <span data-ttu-id="367ee-161">coleção [accessReviewDecision](../resources/accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="367ee-161">[accessReviewDecision](../resources/accessreviewdecision.md) collection</span></span>|    <span data-ttu-id="367ee-162">Como revisor, obtenha as minhas decisões de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="367ee-162">As a reviewer, get my decisions of an accessReview.</span></span>|


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
