---
title: Obter accessReviewScheduleDefinition
description: Leia as propriedades e as relações de um objeto accessReviewScheduleDefinition.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: b7eb33d56831e330883d833c3117187b7cc12b1c
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208645"
---
# <a name="get-accessreviewscheduledefinition"></a><span data-ttu-id="028e9-103">Obter accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="028e9-103">Get accessReviewScheduleDefinition</span></span>
<span data-ttu-id="028e9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="028e9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="028e9-105">Leia as propriedades e as relações de [um objeto accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="028e9-105">Read the properties and relationships of an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>

<span data-ttu-id="028e9-106">Para recuperar as instâncias da série de revisão de acesso, use a API [accessReviewInstance de](accessreviewinstance-list.md) lista.</span><span class="sxs-lookup"><span data-stu-id="028e9-106">To retrieve the instances of the access review series, use the [list accessReviewInstance](accessreviewinstance-list.md) API.</span></span>   

## <a name="permissions"></a><span data-ttu-id="028e9-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="028e9-107">Permissions</span></span>
<span data-ttu-id="028e9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="028e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="028e9-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="028e9-110">Permission type</span></span>|<span data-ttu-id="028e9-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="028e9-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="028e9-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="028e9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="028e9-113">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="028e9-113">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="028e9-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="028e9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="028e9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="028e9-115">Not supported.</span></span>|
|<span data-ttu-id="028e9-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="028e9-116">Application</span></span>|<span data-ttu-id="028e9-117">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="028e9-117">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|

<span data-ttu-id="028e9-118">Para chamar essa API, o usuário de entrada também deve estar em uma função de diretório que permita que ele leia uma revisão de acesso, ou o usuário pode ser atribuído como revistor na revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="028e9-118">To call this API, the signed-in user must also be in a directory role that permits them to read an access review, or the user can be assigned as a reviewer on the access review.</span></span>  <span data-ttu-id="028e9-119">Para obter mais detalhes, consulte os requisitos de função e permissão para [avaliações de acesso.](../resources/accessreviewsv2-root.md)</span><span class="sxs-lookup"><span data-stu-id="028e9-119">For more details, see the role and permission requirements for [access reviews](../resources/accessreviewsv2-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="028e9-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="028e9-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="028e9-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="028e9-121">Optional query parameters</span></span>
<span data-ttu-id="028e9-122">Este método dá suporte `$select` ao parâmetro de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="028e9-122">This method supports `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="028e9-123">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="028e9-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="028e9-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="028e9-124">Request headers</span></span>
|<span data-ttu-id="028e9-125">Nome</span><span class="sxs-lookup"><span data-stu-id="028e9-125">Name</span></span>|<span data-ttu-id="028e9-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="028e9-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="028e9-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="028e9-127">Authorization</span></span>|<span data-ttu-id="028e9-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="028e9-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="028e9-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="028e9-130">Request body</span></span>
<span data-ttu-id="028e9-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="028e9-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="028e9-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="028e9-132">Response</span></span>

<span data-ttu-id="028e9-133">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="028e9-133">If successful, this method returns a `200 OK` response code and an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="028e9-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="028e9-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="028e9-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="028e9-135">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="028e9-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="028e9-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessreviewscheduledefinition"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/3856fd6f-36e2-4152-97c9-76070d19f730
```
# <a name="c"></a>[<span data-ttu-id="028e9-137">C#</span><span class="sxs-lookup"><span data-stu-id="028e9-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreviewscheduledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="028e9-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="028e9-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreviewscheduledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="028e9-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="028e9-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreviewscheduledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="028e9-140">Java</span><span class="sxs-lookup"><span data-stu-id="028e9-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreviewscheduledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="028e9-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="028e9-141">Response</span></span>
><span data-ttu-id="028e9-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="028e9-142">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewScheduleDefinition"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "id": "d6bf2f6c-2f6c-d6bf-6c2f-bfd66c2fbfd6",
    "displayName": "Review example",
    "status": "Applying",
    "scope": {
        "@odata.type": "#microsoft.graph.accessReviewQueryScope",
        "query": "/v1.0/groups/4444d821-ca3b-45cc-98ee-54c00a04deef/transitiveMembers/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
        "queryType": "MicrosoftGraph",
        "queryRoot": null
    },
    "reviewers": [
        {
            "query": "/v1.0/users/5555556e-fce3-4e2d-b28e-4ac0c7d2fa10",
            "queryType": "MicrosoftGraph",
            "queryRoot": null
        }
    ],
    "fallbackReviewers": [],
    "instanceEnumerationScope": {
        "@odata.type": "#microsoft.graph.accessReviewQueryScope",
        "query": "/v1.0/groups/4444d821-ca3b-45cc-98ee-54c00a04deef",
        "queryType": "MicrosoftGraph",
        "queryRoot": null
    },
    "settings": {
        "mailNotificationsEnabled": true,
        "reminderNotificationsEnabled": true,
        "justificationRequiredOnApproval": false,
        "defaultDecisionEnabled": true,
        "defaultDecision": "Deny",
        "instanceDurationInDays": 10,
        "autoApplyDecisionsEnabled": false,
        "recommendationsEnabled": true,
        "recurrence": {
            "pattern": null,
            "range": {
                "type": "numbered",
                "numberOfOccurrences": 0,
                "recurrenceTimeZone": null,
                "startDate": "2021-04-28",
                "endDate": "2021-05-08"
            }
        },
        "applyActions": [
            {
                "@odata.type": "#microsoft.graph.disableAndDeleteUserApplyAction"
            }
        ]
    }
  }
}
```

## <a name="see-also"></a><span data-ttu-id="028e9-143">Confira também</span><span class="sxs-lookup"><span data-stu-id="028e9-143">See also</span></span>

- [<span data-ttu-id="028e9-144">Criar accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="028e9-144">Create accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-post.md)
- [<span data-ttu-id="028e9-145">Listar accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="028e9-145">List accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-list.md)
- [<span data-ttu-id="028e9-146">Listar accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="028e9-146">List accessReviewInstance</span></span>](accessreviewinstance-list.md)
