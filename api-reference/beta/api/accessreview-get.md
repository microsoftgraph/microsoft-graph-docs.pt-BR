---
title: Obter accessReview
description: No recurso de revisões do Azure AD Access, recupere um objeto accessReview.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f2050635bbe019be2673644f885f8ec87f9c3d22
ms.sourcegitcommit: 5f643d3b3f71a9711963c8953da2188539fc9b0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/14/2020
ms.locfileid: "41119536"
---
# <a name="get-accessreview"></a><span data-ttu-id="253fa-103">Obter accessReview</span><span class="sxs-lookup"><span data-stu-id="253fa-103">Get accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="253fa-104">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , recupere um objeto [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="253fa-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve an [accessReview](../resources/accessreview.md) object.</span></span>  

<span data-ttu-id="253fa-105">Para recuperar os revisores da revisão do Access, use a API [list accessReview reviewers](accessreview-listreviewers.md) .</span><span class="sxs-lookup"><span data-stu-id="253fa-105">To retrieve the reviewers of the access review, use the [list accessReview reviewers](accessreview-listreviewers.md) API.</span></span> <span data-ttu-id="253fa-106">Para recuperar as decisões da revisão de acesso, use a API de [accessReview decisions](accessreview-listdecisions.md) ou a API [list My accessReview decisions](accessreview-listmydecisions.md) .</span><span class="sxs-lookup"><span data-stu-id="253fa-106">To retrieve the decisions of the access review, use the [list accessReview decisions](accessreview-listdecisions.md) API, or the [list my accessReview decisions](accessreview-listmydecisions.md) API.</span></span>

<span data-ttu-id="253fa-107">Se esta for uma revisão de acesso recorrente, nenhuma decisão será associada à série de análise de acesso recorrente.</span><span class="sxs-lookup"><span data-stu-id="253fa-107">If this is a recurring access review, no decisions will be associated with the recurring access review series.</span></span> <span data-ttu-id="253fa-108">Em vez disso, `instances` use a relação dessa série para recuperar uma coleção [accessReview](../resources/accessreview.md) das instâncias passadas, atual e futuras da revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="253fa-108">Instead, use the `instances` relationship of that series to retrieve an [accessReview](../resources/accessreview.md) collection of the past, current, and future instances of the access review.</span></span> <span data-ttu-id="253fa-109">Cada instância passada e atual terá decisões.</span><span class="sxs-lookup"><span data-stu-id="253fa-109">Each past and current instance will have decisions.</span></span>

## <a name="permissions"></a><span data-ttu-id="253fa-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="253fa-110">Permissions</span></span>
<span data-ttu-id="253fa-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="253fa-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="253fa-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="253fa-113">Permission type</span></span>                        | <span data-ttu-id="253fa-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="253fa-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="253fa-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="253fa-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="253fa-116">AccessReview. Read. All, AccessReview. ReadWrite. Membership, AccessReview. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="253fa-116">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="253fa-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="253fa-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="253fa-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="253fa-118">Not supported.</span></span> |
|<span data-ttu-id="253fa-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="253fa-119">Application</span></span>                            | <span data-ttu-id="253fa-120">AccessReview. Read. All, AccessReview. ReadWrite. Membership</span><span class="sxs-lookup"><span data-stu-id="253fa-120">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span>  |

<span data-ttu-id="253fa-121">Para chamar essa API, o usuário conectado também deve estar em uma função de diretório que permite que ele leia uma revisão do Access ou que o usuário possa ser atribuído como um revisor na revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="253fa-121">In order to call this API, the signed in user must also be in a directory role that permits them to read an access review, or the user can be assigned as a reviewer on the access review.</span></span>  <span data-ttu-id="253fa-122">Para obter mais detalhes, consulte a função e os requisitos de permissão para [revisões do Access](../resources/accessreviews-root.md).</span><span class="sxs-lookup"><span data-stu-id="253fa-122">For more details, see the role and permission requirements for [access reviews](../resources/accessreviews-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="253fa-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="253fa-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews/{reviewId}
```
## <a name="request-headers"></a><span data-ttu-id="253fa-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="253fa-124">Request headers</span></span>
| <span data-ttu-id="253fa-125">Nome</span><span class="sxs-lookup"><span data-stu-id="253fa-125">Name</span></span>         | <span data-ttu-id="253fa-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="253fa-126">Type</span></span>        | <span data-ttu-id="253fa-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="253fa-127">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="253fa-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="253fa-128">Authorization</span></span> | <span data-ttu-id="253fa-129">string</span><span class="sxs-lookup"><span data-stu-id="253fa-129">string</span></span> | <span data-ttu-id="253fa-p105">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="253fa-p105">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="253fa-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="253fa-132">Request body</span></span>
<span data-ttu-id="253fa-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="253fa-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="253fa-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="253fa-134">Response</span></span>
<span data-ttu-id="253fa-135">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [accessReview](../resources/accessreview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="253fa-135">If successful, this method returns a `200 OK` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="253fa-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="253fa-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="253fa-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="253fa-137">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="253fa-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="253fa-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="253fa-139">C#</span><span class="sxs-lookup"><span data-stu-id="253fa-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="253fa-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="253fa-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="253fa-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="253fa-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="253fa-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="253fa-142">Response</span></span>
><span data-ttu-id="253fa-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="253fa-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="253fa-145">Confira também</span><span class="sxs-lookup"><span data-stu-id="253fa-145">See also</span></span>

- [<span data-ttu-id="253fa-146">Criar accessReview</span><span class="sxs-lookup"><span data-stu-id="253fa-146">Create accessReview</span></span>](accessreview-create.md)
- [<span data-ttu-id="253fa-147">Listar accessReviews</span><span class="sxs-lookup"><span data-stu-id="253fa-147">List accessReviews</span></span>](accessreview-list.md)
- [<span data-ttu-id="253fa-148">Listar programControls</span><span class="sxs-lookup"><span data-stu-id="253fa-148">List programControls</span></span>](programcontrol-list.md)
- [<span data-ttu-id="253fa-149">Listar revisores do accessReview</span><span class="sxs-lookup"><span data-stu-id="253fa-149">List accessReview reviewers</span></span>](accessreview-listreviewers.md)
- [<span data-ttu-id="253fa-150">Listar decisões accessReview</span><span class="sxs-lookup"><span data-stu-id="253fa-150">List accessReview decisions</span></span>](accessreview-listdecisions.md)
- [<span data-ttu-id="253fa-151">Listar minhas decisões do accessReview</span><span class="sxs-lookup"><span data-stu-id="253fa-151">List my accessReview decisions</span></span>](accessreview-listmydecisions.md)


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
