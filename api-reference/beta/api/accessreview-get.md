---
title: Obter accessReview
description: 'No recurso de revisões do Azure AD Access, recupere um objeto accessReview.  '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b0c088f5c8f7a402282d1d205ff52b80e68fac75
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36719301"
---
# <a name="get-accessreview"></a><span data-ttu-id="49a72-103">Obter accessReview</span><span class="sxs-lookup"><span data-stu-id="49a72-103">Get accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49a72-104">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , recupere um objeto [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="49a72-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve an [accessReview](../resources/accessreview.md) object.</span></span>  

<span data-ttu-id="49a72-105">Para recuperar os revisores da revisão do Access, use a API [list accessReview](accessreview-listreviewers.md) reviewers.</span><span class="sxs-lookup"><span data-stu-id="49a72-105">To retrieve the reviewers of the access review, use the [list accessReview reviewers](accessreview-listreviewers.md) API.</span></span> <span data-ttu-id="49a72-106">Para recuperar as decisões da revisão de acesso, use a API de [accessReview decisions](accessreview-listdecisions.md) ou a API [list My accessReview decisions](accessreview-listmydecisions.md) .</span><span class="sxs-lookup"><span data-stu-id="49a72-106">To retrieve the decisions of the access review, use the [list accessReview decisions](accessreview-listdecisions.md) API, or the [list my accessReview decisions](accessreview-listmydecisions.md) API.</span></span>

<span data-ttu-id="49a72-107">Se esta for uma revisão de acesso recorrente, use a `instances` relação para recuperar uma coleção [accessReview](../resources/accessreview.md) das instâncias passadas, atual e futura da revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="49a72-107">If this is a recurring access review, then use the `instances` relationship to retrieve an [accessReview](../resources/accessreview.md) collection of the past, current, and future instances of the access review.</span></span>

## <a name="permissions"></a><span data-ttu-id="49a72-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="49a72-108">Permissions</span></span>
<span data-ttu-id="49a72-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49a72-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49a72-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="49a72-111">Permission type</span></span>                        | <span data-ttu-id="49a72-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="49a72-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="49a72-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="49a72-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="49a72-114">AccessReview. Read. All, AccessReview. ReadWrite. Membership, AccessReview. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="49a72-114">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="49a72-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="49a72-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49a72-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="49a72-116">Not supported.</span></span> |
|<span data-ttu-id="49a72-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="49a72-117">Application</span></span>                            | <span data-ttu-id="49a72-118">AccessReview. Read. All, AccessReview. ReadWrite. Membership</span><span class="sxs-lookup"><span data-stu-id="49a72-118">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span>  |

<span data-ttu-id="49a72-119">Para chamar essa API, o usuário conectado também deve estar em uma função de diretório que permite que ele leia uma revisão do Access ou que o usuário possa ser atribuído como um revisor na revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="49a72-119">In order to call this API, the signed in user must also be in a directory role that permits them to read an access review, or the user can be assigned as a reviewer on the access review.</span></span>  <span data-ttu-id="49a72-120">Para obter mais detalhes, consulte a função e os requisitos de permissão para [revisões do Access](../resources/accessreviews-root.md).</span><span class="sxs-lookup"><span data-stu-id="49a72-120">For more details, see the role and permission requirements for [access reviews](../resources/accessreviews-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="49a72-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="49a72-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews/{reviewId}
```
## <a name="request-headers"></a><span data-ttu-id="49a72-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="49a72-122">Request headers</span></span>
| <span data-ttu-id="49a72-123">Nome</span><span class="sxs-lookup"><span data-stu-id="49a72-123">Name</span></span>         | <span data-ttu-id="49a72-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="49a72-124">Type</span></span>        | <span data-ttu-id="49a72-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="49a72-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="49a72-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="49a72-126">Authorization</span></span> | <span data-ttu-id="49a72-127">string</span><span class="sxs-lookup"><span data-stu-id="49a72-127">string</span></span> | <span data-ttu-id="49a72-p104">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="49a72-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="49a72-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="49a72-130">Request body</span></span>
<span data-ttu-id="49a72-131">Nenhum corpo de solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="49a72-131">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="49a72-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="49a72-132">Response</span></span>
<span data-ttu-id="49a72-133">Se tiver êxito, este método retornará `200, OK` um código de resposta e um objeto [accessReview](../resources/accessreview.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="49a72-133">If successful, this method returns a `200, OK` response code and an [accessReview](../resources/accessreview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49a72-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="49a72-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="49a72-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="49a72-135">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="49a72-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="49a72-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="49a72-137">C#</span><span class="sxs-lookup"><span data-stu-id="49a72-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="49a72-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49a72-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="49a72-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="49a72-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="49a72-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="49a72-140">Response</span></span>
><span data-ttu-id="49a72-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="49a72-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="49a72-143">Confira também</span><span class="sxs-lookup"><span data-stu-id="49a72-143">See also</span></span>

- [<span data-ttu-id="49a72-144">Criar accessReview</span><span class="sxs-lookup"><span data-stu-id="49a72-144">Create accessReview</span></span>](accessreview-create.md)
- [<span data-ttu-id="49a72-145">Listar accessReviews</span><span class="sxs-lookup"><span data-stu-id="49a72-145">List accessReviews</span></span>](accessreview-list.md)
- [<span data-ttu-id="49a72-146">Listar programControls</span><span class="sxs-lookup"><span data-stu-id="49a72-146">List programControls</span></span>](programcontrol-list.md)
- [<span data-ttu-id="49a72-147">Listar revisores do accessReview</span><span class="sxs-lookup"><span data-stu-id="49a72-147">List accessReview reviewers</span></span>](accessreview-listreviewers.md)
- [<span data-ttu-id="49a72-148">Listar decisões accessReview</span><span class="sxs-lookup"><span data-stu-id="49a72-148">List accessReview decisions</span></span>](accessreview-listdecisions.md)
- [<span data-ttu-id="49a72-149">Listar minhas decisões do accessReview</span><span class="sxs-lookup"><span data-stu-id="49a72-149">List my accessReview decisions</span></span>](accessreview-listmydecisions.md)


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
