---
title: Acessar AccessReviewScheduleDefinition
description: Recupere um objeto accessReviewScheduleDefinition.
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bb8b22ecb9baf4e579223fcc490bf29fea4c6894
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981155"
---
# <a name="get-accessreviewscheduledefinition"></a><span data-ttu-id="93d4d-103">Acessar AccessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="93d4d-103">Get accessReviewScheduleDefinition</span></span>

<span data-ttu-id="93d4d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93d4d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93d4d-105">Recupere um [objeto accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) por ID.</span><span class="sxs-lookup"><span data-stu-id="93d4d-105">Retrieve an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object by ID.</span></span> <span data-ttu-id="93d4d-106">Isso retorna todas as propriedades da série de revisão de acesso agendada, exceto para o accessReviewInstances associado.</span><span class="sxs-lookup"><span data-stu-id="93d4d-106">This returns all properties of the scheduled access review series except for the associated accessReviewInstances.</span></span> <span data-ttu-id="93d4d-107">Cada accessReviewScheduleDefinition tem pelo menos uma instância.</span><span class="sxs-lookup"><span data-stu-id="93d4d-107">Each accessReviewScheduleDefinition has at least one instance.</span></span> <span data-ttu-id="93d4d-108">Uma instância representa uma revisão de um recurso específico (como os membros de um grupo específico), durante uma ocorrência (por exemplo, março de 2021) de uma revisão recorrente.</span><span class="sxs-lookup"><span data-stu-id="93d4d-108">An instance represents a review for a specific resource (such as a particular group's members), during one occurrence (e.g., March 2021) of a recurring review.</span></span>

<span data-ttu-id="93d4d-109">Para recuperar as instâncias da série de revisão de acesso, use a LISTA [accessReviewInstance](accessreviewinstance-list.md) API.</span><span class="sxs-lookup"><span data-stu-id="93d4d-109">To retrieve the instances of the access review series, use the [list accessReviewInstance](accessreviewinstance-list.md) API.</span></span>

## <a name="permissions"></a><span data-ttu-id="93d4d-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="93d4d-110">Permissions</span></span>
<span data-ttu-id="93d4d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93d4d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93d4d-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="93d4d-113">Permission type</span></span>                        | <span data-ttu-id="93d4d-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="93d4d-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="93d4d-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="93d4d-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="93d4d-116">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93d4d-116">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="93d4d-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="93d4d-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="93d4d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="93d4d-118">Not supported.</span></span>|
|<span data-ttu-id="93d4d-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="93d4d-119">Application</span></span>                            | <span data-ttu-id="93d4d-120">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93d4d-120">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span> |

<span data-ttu-id="93d4d-121">Para chamar essa API, o usuário deve estar também em uma função de diretório que permita ler uma revisão de acesso, ou o usuário pode ser atribuído como revistor na revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="93d4d-121">To call this API, the signed-in user must also be in a directory role that permits them to read an access review, or the user can be assigned as a reviewer on the access review.</span></span>  <span data-ttu-id="93d4d-122">Para obter mais detalhes, consulte os requisitos de função e permissão para [revisões de acesso.](../resources/accessreviewsv2-root.md)</span><span class="sxs-lookup"><span data-stu-id="93d4d-122">For more details, see the role and permission requirements for [access reviews](../resources/accessreviewsv2-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="93d4d-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="93d4d-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/accessReviews/definitions/{review-id}
```
## <a name="request-headers"></a><span data-ttu-id="93d4d-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="93d4d-124">Request headers</span></span>
<span data-ttu-id="93d4d-125">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="93d4d-125">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="93d4d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="93d4d-126">Request body</span></span>
<span data-ttu-id="93d4d-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="93d4d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="93d4d-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="93d4d-128">Response</span></span>
<span data-ttu-id="93d4d-129">Se bem-sucedido, este método retorna um código de resposta e um objeto `200 OK` [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="93d4d-129">If successful, this method returns a `200 OK` response code and an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="93d4d-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="93d4d-130">Examples</span></span>
### <a name="request"></a><span data-ttu-id="93d4d-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="93d4d-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="93d4d-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="93d4d-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReviewScheduleDefinition"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/2b83cc42-09db-46f6-8c6e-16fec466a82d
```
# <a name="c"></a>[<span data-ttu-id="93d4d-133">C#</span><span class="sxs-lookup"><span data-stu-id="93d4d-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreviewscheduledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="93d4d-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="93d4d-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreviewscheduledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="93d4d-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="93d4d-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreviewscheduledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="93d4d-136">Java</span><span class="sxs-lookup"><span data-stu-id="93d4d-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreviewscheduledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---

### <a name="response"></a><span data-ttu-id="93d4d-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="93d4d-137">Response</span></span>
><span data-ttu-id="93d4d-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="93d4d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewScheduleDefinition",
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "60860cdd-fb4d-4054-91ba-f7544443baa6",
    "displayName": "Test world",
    "createdDateTime": "2020-09-14T20:03:36.7391027Z",
    "lastModifiedDateTime": "2020-09-14T20:04:28Z",
    "status": "InProgress",
    "descriptionForAdmins": "",
    "descriptionForReviewers": "",
    "createdBy": {
        "id": "957f1027-c0ee-460d-4444-b8828e59e0fe",
        "displayName": "MOD Administrator",
        "userPrincipalName": "admin@contoso.com"
    },
    "scope": {
        "query": "/groups/b7a059cb-038a-4802-8fc9-b944440cf11f/transitiveMembers",
        "queryType": "MicrosoftGraph"
    },
    "instanceEnumerationScope": {
        "query": "/groups/b7a059cb-038a-4802-8fc9-b9d14444f11f",
        "queryType": "MicrosoftGraph"
    },
    "reviewers": [],
    "settings": {
        "mailNotificationsEnabled": true,
        "reminderNotificationsEnabled": true,
        "justificationRequiredOnApproval": true,
        "defaultDecisionEnabled": false,
        "defaultDecision": "None",
        "instanceDurationInDays": 0,
        "autoApplyDecisionsEnabled": false,
        "recommendationsEnabled": true,
        "recurrence": {
            "pattern": {
                "type": "weekly",
                "interval": 1,
                "month": 0,
                "dayOfMonth": 0,
                "daysOfWeek": [],
                "firstDayOfWeek": "sunday",
                "index": "first"
            },
            "range": {
                "type": "numbered",
                "numberOfOccurrences": 0,
                "recurrenceTimeZone": null,
                "startDate": "2020-09-15",
                "endDate": "9999-12-31"
            }
        }
    }
}
```

## <a name="see-also"></a><span data-ttu-id="93d4d-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="93d4d-140">See also</span></span>

- [<span data-ttu-id="93d4d-141">Criar accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="93d4d-141">Create accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-create.md)
- [<span data-ttu-id="93d4d-142">Listar accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="93d4d-142">List accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-list.md)
- [<span data-ttu-id="93d4d-143">Listar accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="93d4d-143">List accessReviewInstance</span></span>](accessreviewinstance-list.md)


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReviewScheduleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
