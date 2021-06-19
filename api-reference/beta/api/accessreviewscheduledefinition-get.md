---
title: Obter accessReviewScheduleDefinition
description: Recupere um objeto accessReviewScheduleDefinition.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: b29e9790fc9a6a43dd7f36b0f91fcd94b903bd60
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030447"
---
# <a name="get-accessreviewscheduledefinition"></a><span data-ttu-id="b5112-103">Obter accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="b5112-103">Get accessReviewScheduleDefinition</span></span>

<span data-ttu-id="b5112-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5112-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5112-105">Recupere um [objeto accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) por ID.</span><span class="sxs-lookup"><span data-stu-id="b5112-105">Retrieve an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object by ID.</span></span> <span data-ttu-id="b5112-106">Isso retorna todas as propriedades da série de revisão de acesso agendada, exceto para o accessReviewInstances associado.</span><span class="sxs-lookup"><span data-stu-id="b5112-106">This returns all properties of the scheduled access review series except for the associated accessReviewInstances.</span></span> <span data-ttu-id="b5112-107">Cada accessReviewScheduleDefinition tem pelo menos uma instância.</span><span class="sxs-lookup"><span data-stu-id="b5112-107">Each accessReviewScheduleDefinition has at least one instance.</span></span> <span data-ttu-id="b5112-108">Uma instância representa uma revisão de um recurso específico (como membros de um grupo específico), durante uma ocorrência (por exemplo, março de 2021) de uma revisão recorrente.</span><span class="sxs-lookup"><span data-stu-id="b5112-108">An instance represents a review for a specific resource (such as a particular group's members), during one occurrence (e.g., March 2021) of a recurring review.</span></span>

<span data-ttu-id="b5112-109">Para recuperar as instâncias da série de revisão de acesso, use a API [accessReviewInstance de](accessreviewinstance-list.md) lista.</span><span class="sxs-lookup"><span data-stu-id="b5112-109">To retrieve the instances of the access review series, use the [list accessReviewInstance](accessreviewinstance-list.md) API.</span></span>

## <a name="permissions"></a><span data-ttu-id="b5112-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="b5112-110">Permissions</span></span>
<span data-ttu-id="b5112-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5112-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5112-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b5112-113">Permission type</span></span>                        | <span data-ttu-id="b5112-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b5112-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5112-115">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b5112-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="b5112-116">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5112-116">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="b5112-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b5112-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5112-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b5112-118">Not supported.</span></span>|
|<span data-ttu-id="b5112-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b5112-119">Application</span></span>                            | <span data-ttu-id="b5112-120">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5112-120">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span> |

<span data-ttu-id="b5112-121">Para chamar essa API, o usuário de entrada também deve estar em uma função de diretório que permita que ele leia uma revisão de acesso, ou o usuário pode ser atribuído como revistor na revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="b5112-121">To call this API, the signed-in user must also be in a directory role that permits them to read an access review, or the user can be assigned as a reviewer on the access review.</span></span>  <span data-ttu-id="b5112-122">Para obter mais detalhes, consulte os requisitos de função e permissão para [avaliações de acesso.](../resources/accessreviewsv2-root.md)</span><span class="sxs-lookup"><span data-stu-id="b5112-122">For more details, see the role and permission requirements for [access reviews](../resources/accessreviewsv2-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="b5112-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b5112-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/accessReviews/definitions/{review-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b5112-124">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b5112-124">Optional query parameters</span></span>
<span data-ttu-id="b5112-125">Este método dá suporte a parâmetros de consulta `$select` OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b5112-125">This method supports `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="b5112-126">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b5112-126">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b5112-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b5112-127">Request headers</span></span>
<span data-ttu-id="b5112-128">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b5112-128">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="b5112-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b5112-129">Request body</span></span>
<span data-ttu-id="b5112-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b5112-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5112-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5112-131">Response</span></span>
<span data-ttu-id="b5112-132">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b5112-132">If successful, this method returns a `200 OK` response code and an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b5112-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b5112-133">Examples</span></span>
### <a name="request"></a><span data-ttu-id="b5112-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b5112-134">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b5112-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="b5112-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReviewScheduleDefinition"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/2b83cc42-09db-46f6-8c6e-16fec466a82d
```
# <a name="c"></a>[<span data-ttu-id="b5112-136">C#</span><span class="sxs-lookup"><span data-stu-id="b5112-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreviewscheduledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b5112-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b5112-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreviewscheduledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b5112-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b5112-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreviewscheduledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b5112-139">Java</span><span class="sxs-lookup"><span data-stu-id="b5112-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreviewscheduledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---

### <a name="response"></a><span data-ttu-id="b5112-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5112-140">Response</span></span>
><span data-ttu-id="b5112-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b5112-141">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "status": "InProgress",
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

## <a name="see-also"></a><span data-ttu-id="b5112-142">Confira também</span><span class="sxs-lookup"><span data-stu-id="b5112-142">See also</span></span>

- [<span data-ttu-id="b5112-143">Criar accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="b5112-143">Create accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-post.md)
- [<span data-ttu-id="b5112-144">Listar accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="b5112-144">List accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-list.md)
- [<span data-ttu-id="b5112-145">Listar accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="b5112-145">List accessReviewInstance</span></span>](accessreviewinstance-list.md)


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
