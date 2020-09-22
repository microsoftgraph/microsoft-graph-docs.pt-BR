---
title: Obter accessReview
description: No recurso de revisões do Azure AD Access, recupere um objeto accessReview.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3af27792d66328085eb0a48a38935a33ec2b2607
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47983589"
---
# <a name="get-accessreview"></a><span data-ttu-id="3595e-103">Obter accessReview</span><span class="sxs-lookup"><span data-stu-id="3595e-103">Get accessReview</span></span>

<span data-ttu-id="3595e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3595e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3595e-105">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , recupere um objeto [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="3595e-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve an [accessReview](../resources/accessreview.md) object.</span></span>  

<span data-ttu-id="3595e-106">Para recuperar os revisores da revisão do Access, use a API [list accessReview reviewers](accessreview-listreviewers.md) .</span><span class="sxs-lookup"><span data-stu-id="3595e-106">To retrieve the reviewers of the access review, use the [list accessReview reviewers](accessreview-listreviewers.md) API.</span></span> <span data-ttu-id="3595e-107">Para recuperar as decisões da revisão de acesso, use a API de [accessReview decisions](accessreview-listdecisions.md) ou a API [list My accessReview decisions](accessreview-listmydecisions.md) .</span><span class="sxs-lookup"><span data-stu-id="3595e-107">To retrieve the decisions of the access review, use the [list accessReview decisions](accessreview-listdecisions.md) API, or the [list my accessReview decisions](accessreview-listmydecisions.md) API.</span></span>

<span data-ttu-id="3595e-108">Se esta for uma revisão de acesso recorrente, nenhuma decisão será associada à série de análise de acesso recorrente.</span><span class="sxs-lookup"><span data-stu-id="3595e-108">If this is a recurring access review, no decisions will be associated with the recurring access review series.</span></span> <span data-ttu-id="3595e-109">Em vez disso, use a `instances` relação dessa série para recuperar uma coleção [accessReview](../resources/accessreview.md) das instâncias passadas, atual e futuras da revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="3595e-109">Instead, use the `instances` relationship of that series to retrieve an [accessReview](../resources/accessreview.md) collection of the past, current, and future instances of the access review.</span></span> <span data-ttu-id="3595e-110">Cada instância passada e atual terá decisões.</span><span class="sxs-lookup"><span data-stu-id="3595e-110">Each past and current instance will have decisions.</span></span>

## <a name="permissions"></a><span data-ttu-id="3595e-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="3595e-111">Permissions</span></span>
<span data-ttu-id="3595e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3595e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3595e-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3595e-114">Permission type</span></span>                        | <span data-ttu-id="3595e-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3595e-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="3595e-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3595e-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="3595e-117">AccessReview. Read. All, AccessReview. ReadWrite. Membership, AccessReview. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="3595e-117">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="3595e-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3595e-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3595e-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3595e-119">Not supported.</span></span> |
|<span data-ttu-id="3595e-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3595e-120">Application</span></span>                            | <span data-ttu-id="3595e-121">AccessReview. Read. All, AccessReview. ReadWrite. Membership</span><span class="sxs-lookup"><span data-stu-id="3595e-121">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span>  |

<span data-ttu-id="3595e-122">Para chamar essa API, o usuário conectado também deve estar em uma função de diretório que permite que ele leia uma revisão do Access ou que o usuário possa ser atribuído como um revisor na revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="3595e-122">In order to call this API, the signed in user must also be in a directory role that permits them to read an access review, or the user can be assigned as a reviewer on the access review.</span></span>  <span data-ttu-id="3595e-123">Para obter mais detalhes, consulte a função e os requisitos de permissão para [revisões do Access](../resources/accessreviews-root.md).</span><span class="sxs-lookup"><span data-stu-id="3595e-123">For more details, see the role and permission requirements for [access reviews](../resources/accessreviews-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="3595e-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3595e-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews/{reviewId}
```
## <a name="request-headers"></a><span data-ttu-id="3595e-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3595e-125">Request headers</span></span>
| <span data-ttu-id="3595e-126">Nome</span><span class="sxs-lookup"><span data-stu-id="3595e-126">Name</span></span>         | <span data-ttu-id="3595e-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="3595e-127">Type</span></span>        | <span data-ttu-id="3595e-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="3595e-128">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="3595e-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="3595e-129">Authorization</span></span> | <span data-ttu-id="3595e-130">string</span><span class="sxs-lookup"><span data-stu-id="3595e-130">string</span></span> | <span data-ttu-id="3595e-p105">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3595e-p105">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3595e-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3595e-133">Request body</span></span>
<span data-ttu-id="3595e-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3595e-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3595e-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="3595e-135">Response</span></span>
<span data-ttu-id="3595e-136">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [accessReview](../resources/accessreview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3595e-136">If successful, this method returns a `200 OK` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3595e-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3595e-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3595e-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3595e-138">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="3595e-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="3595e-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d
```
# <a name="c"></a>[<span data-ttu-id="3595e-140">C#</span><span class="sxs-lookup"><span data-stu-id="3595e-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3595e-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3595e-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3595e-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3595e-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3595e-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="3595e-143">Response</span></span>
><span data-ttu-id="3595e-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3595e-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="3595e-146">Confira também</span><span class="sxs-lookup"><span data-stu-id="3595e-146">See also</span></span>

- [<span data-ttu-id="3595e-147">Criar accessReview</span><span class="sxs-lookup"><span data-stu-id="3595e-147">Create accessReview</span></span>](accessreview-create.md)
- [<span data-ttu-id="3595e-148">Listar accessReviews</span><span class="sxs-lookup"><span data-stu-id="3595e-148">List accessReviews</span></span>](accessreview-list.md)
- [<span data-ttu-id="3595e-149">Listar programControls</span><span class="sxs-lookup"><span data-stu-id="3595e-149">List programControls</span></span>](programcontrol-list.md)
- [<span data-ttu-id="3595e-150">Listar revisores do accessReview</span><span class="sxs-lookup"><span data-stu-id="3595e-150">List accessReview reviewers</span></span>](accessreview-listreviewers.md)
- [<span data-ttu-id="3595e-151">Listar decisões accessReview</span><span class="sxs-lookup"><span data-stu-id="3595e-151">List accessReview decisions</span></span>](accessreview-listdecisions.md)
- [<span data-ttu-id="3595e-152">Listar minhas decisões do accessReview</span><span class="sxs-lookup"><span data-stu-id="3595e-152">List my accessReview decisions</span></span>](accessreview-listmydecisions.md)


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


