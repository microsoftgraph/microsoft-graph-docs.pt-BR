---
title: Obter accessReview
description: No recurso de revisões de acesso do Azure AD, recupere um objeto accessReview.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 01bf052e6e77377c5ec07eddfc005b1a05394106
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048495"
---
# <a name="get-accessreview"></a><span data-ttu-id="5056b-103">Obter accessReview</span><span class="sxs-lookup"><span data-stu-id="5056b-103">Get accessReview</span></span>

<span data-ttu-id="5056b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5056b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5056b-105">No recurso de revisões de acesso do Azure [AD,](../resources/accessreviews-root.md) recupere um [objeto accessReview.](../resources/accessreview.md)</span><span class="sxs-lookup"><span data-stu-id="5056b-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve an [accessReview](../resources/accessreview.md) object.</span></span>  

<span data-ttu-id="5056b-106">Para recuperar os revisores da revisão de acesso, use a API de revisores [de acesso à](accessreview-listreviewers.md) lista.</span><span class="sxs-lookup"><span data-stu-id="5056b-106">To retrieve the reviewers of the access review, use the [list accessReview reviewers](accessreview-listreviewers.md) API.</span></span> <span data-ttu-id="5056b-107">Para recuperar as decisões da revisão de acesso, use a API de decisões do [accessReview](accessreview-listdecisions.md) de lista ou a API de decisões [do meu accessReview.](accessreview-listmydecisions.md)</span><span class="sxs-lookup"><span data-stu-id="5056b-107">To retrieve the decisions of the access review, use the [list accessReview decisions](accessreview-listdecisions.md) API, or the [list my accessReview decisions](accessreview-listmydecisions.md) API.</span></span>

<span data-ttu-id="5056b-108">Se for uma revisão de acesso recorrente, nenhuma decisão será associada à série de revisão de acesso recorrente.</span><span class="sxs-lookup"><span data-stu-id="5056b-108">If this is a recurring access review, no decisions will be associated with the recurring access review series.</span></span> <span data-ttu-id="5056b-109">Em vez disso, use a relação dessa série para recuperar uma coleção `instances` [accessReview](../resources/accessreview.md) das instâncias passadas, atuais e futuras da revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="5056b-109">Instead, use the `instances` relationship of that series to retrieve an [accessReview](../resources/accessreview.md) collection of the past, current, and future instances of the access review.</span></span> <span data-ttu-id="5056b-110">Cada instância passada e atual terá decisões.</span><span class="sxs-lookup"><span data-stu-id="5056b-110">Each past and current instance will have decisions.</span></span>

## <a name="permissions"></a><span data-ttu-id="5056b-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="5056b-111">Permissions</span></span>
<span data-ttu-id="5056b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5056b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5056b-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5056b-114">Permission type</span></span>                        | <span data-ttu-id="5056b-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5056b-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="5056b-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5056b-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="5056b-117">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5056b-117">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="5056b-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5056b-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5056b-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5056b-119">Not supported.</span></span> |
|<span data-ttu-id="5056b-120">Application</span><span class="sxs-lookup"><span data-stu-id="5056b-120">Application</span></span>                            | <span data-ttu-id="5056b-121">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="5056b-121">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span>  |

<span data-ttu-id="5056b-122">Para chamar essa API, o usuário inscreveu também deve estar em uma função de diretório que permita que ele leia uma revisão de acesso, ou o usuário pode ser atribuído como revistor na revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="5056b-122">In order to call this API, the signed in user must also be in a directory role that permits them to read an access review, or the user can be assigned as a reviewer on the access review.</span></span>  <span data-ttu-id="5056b-123">Para obter mais detalhes, consulte os requisitos de função e permissão para [avaliações de acesso.](../resources/accessreviews-root.md)</span><span class="sxs-lookup"><span data-stu-id="5056b-123">For more details, see the role and permission requirements for [access reviews](../resources/accessreviews-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="5056b-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5056b-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews/{reviewId}
```
## <a name="request-headers"></a><span data-ttu-id="5056b-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5056b-125">Request headers</span></span>
| <span data-ttu-id="5056b-126">Nome</span><span class="sxs-lookup"><span data-stu-id="5056b-126">Name</span></span>         | <span data-ttu-id="5056b-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="5056b-127">Type</span></span>        | <span data-ttu-id="5056b-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="5056b-128">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="5056b-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="5056b-129">Authorization</span></span> | <span data-ttu-id="5056b-130">string</span><span class="sxs-lookup"><span data-stu-id="5056b-130">string</span></span> | <span data-ttu-id="5056b-p105">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5056b-p105">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5056b-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5056b-133">Request body</span></span>
<span data-ttu-id="5056b-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5056b-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5056b-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="5056b-135">Response</span></span>
<span data-ttu-id="5056b-136">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto accessReview](../resources/accessreview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5056b-136">If successful, this method returns a `200 OK` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5056b-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5056b-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5056b-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5056b-138">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="5056b-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="5056b-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d
```
# <a name="c"></a>[<span data-ttu-id="5056b-140">C#</span><span class="sxs-lookup"><span data-stu-id="5056b-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5056b-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5056b-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5056b-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5056b-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5056b-143">Java</span><span class="sxs-lookup"><span data-stu-id="5056b-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5056b-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="5056b-144">Response</span></span>
><span data-ttu-id="5056b-145">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5056b-145">**Note:** The response object shown here might be shortened for readability.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="5056b-146">Confira também</span><span class="sxs-lookup"><span data-stu-id="5056b-146">See also</span></span>

- [<span data-ttu-id="5056b-147">Criar accessReview</span><span class="sxs-lookup"><span data-stu-id="5056b-147">Create accessReview</span></span>](accessreview-create.md)
- [<span data-ttu-id="5056b-148">Listar accessReviews</span><span class="sxs-lookup"><span data-stu-id="5056b-148">List accessReviews</span></span>](accessreview-list.md)
- [<span data-ttu-id="5056b-149">Listar programControls</span><span class="sxs-lookup"><span data-stu-id="5056b-149">List programControls</span></span>](programcontrol-list.md)
- [<span data-ttu-id="5056b-150">Listar revisores do accessReview</span><span class="sxs-lookup"><span data-stu-id="5056b-150">List accessReview reviewers</span></span>](accessreview-listreviewers.md)
- [<span data-ttu-id="5056b-151">Listar decisões do accessReview</span><span class="sxs-lookup"><span data-stu-id="5056b-151">List accessReview decisions</span></span>](accessreview-listdecisions.md)
- [<span data-ttu-id="5056b-152">Listar minhas decisões do accessReview</span><span class="sxs-lookup"><span data-stu-id="5056b-152">List my accessReview decisions</span></span>](accessreview-listmydecisions.md)


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


