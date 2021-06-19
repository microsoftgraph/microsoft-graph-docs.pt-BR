---
title: 'accessReviewInstance: pendingAccessReviewInstances'
description: Recupere os objetos accessReviewInstance aguardando aprovação chamando o usuário.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: c62f954ea7fe70d46ff4a46879b4d568d619226c
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030521"
---
# <a name="accessreviewinstance-pendingaccessreviewinstances-deprecated"></a><span data-ttu-id="9733b-103">accessReviewInstance: pendingAccessReviewInstances (preterido)</span><span class="sxs-lookup"><span data-stu-id="9733b-103">accessReviewInstance: pendingAccessReviewInstances (deprecated)</span></span>

<span data-ttu-id="9733b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9733b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
><span data-ttu-id="9733b-105">Esse método será preterido e interromperá o retorno de dados em 19 de maio de 2023.</span><span class="sxs-lookup"><span data-stu-id="9733b-105">This method will be deprecated and will stop returning data on May 19, 2023.</span></span> <span data-ttu-id="9733b-106">Ele foi substituído por [filterByCurrentUser](accessreviewinstance-filterbycurrentuser.md).</span><span class="sxs-lookup"><span data-stu-id="9733b-106">It has been replaced by [filterByCurrentUser](accessreviewinstance-filterbycurrentuser.md).</span></span>

>[!NOTE]
><span data-ttu-id="9733b-107">O tamanho padrão da página para essa API é de 100 objetos accessReviewInstance.</span><span class="sxs-lookup"><span data-stu-id="9733b-107">The default page size for this API is 100 accessReviewInstance objects.</span></span> <span data-ttu-id="9733b-108">Para melhorar a eficiência e evitar tempos-de-tempo devido a grandes conjuntos de resultados, aplique paginação usando os `$skip` parâmetros e `$top` de consulta.</span><span class="sxs-lookup"><span data-stu-id="9733b-108">To improve efficiency and avoid timeouts due to large result sets, apply pagination using the `$skip` and `$top` query parameters.</span></span> <span data-ttu-id="9733b-109">Para mais informações, consulte [Paginação de dados do Microsoft Graph em seu aplicativo](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="9733b-109">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

<span data-ttu-id="9733b-110">Recupere os [objetos accessReviewInstance](../resources/accessreviewinstance.md) pendentes aprovação pelo usuário de chamada.</span><span class="sxs-lookup"><span data-stu-id="9733b-110">Retrieve the [accessReviewInstance](../resources/accessreviewinstance.md) objects pending approval by the calling user.</span></span> <span data-ttu-id="9733b-111">Uma lista de zero ou mais objetos accessReviewInstance são retornados, dos quais o usuário de chamada é um revisor atribuído.</span><span class="sxs-lookup"><span data-stu-id="9733b-111">A list of zero or more accessReviewInstance objects are returned, of which the calling user is an assigned reviewer.</span></span>

## <a name="permissions"></a><span data-ttu-id="9733b-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="9733b-112">Permissions</span></span>
<span data-ttu-id="9733b-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9733b-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9733b-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9733b-115">Permission type</span></span>                        | <span data-ttu-id="9733b-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9733b-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="9733b-117">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9733b-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="9733b-118">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9733b-118">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |

 <span data-ttu-id="9733b-119">O usuário in-loco só vê instâncias das quais são atribuídas revisores no accessReviewScheduleDefinition da instância.</span><span class="sxs-lookup"><span data-stu-id="9733b-119">The signed-in user only sees instances of which they are assigned reviewer in the accessReviewScheduleDefinition of the instance.</span></span>

## <a name="http-request"></a><span data-ttu-id="9733b-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9733b-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/pendingAccessReviewInstances
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9733b-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9733b-121">Optional query parameters</span></span>
<span data-ttu-id="9733b-122">Este método oferece `$skip` suporte e `$top` parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9733b-122">This method supports `$skip` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="9733b-123">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="9733b-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9733b-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9733b-124">Request headers</span></span>
<span data-ttu-id="9733b-125">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9733b-125">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="9733b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9733b-126">Request body</span></span>
<span data-ttu-id="9733b-127">Não fornecer um corpo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9733b-127">Do not supply a request body.</span></span>

## <a name="response"></a><span data-ttu-id="9733b-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="9733b-128">Response</span></span>
<span data-ttu-id="9733b-129">Se tiver êxito, este método retornará um código de resposta e uma matriz de `200 OK` [objetos accessReviewInstance](../resources/accessreviewinstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9733b-129">If successful, this method returns a `200 OK` response code and an array of [accessReviewInstance](../resources/accessreviewinstance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9733b-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9733b-130">Examples</span></span>
### <a name="request"></a><span data-ttu-id="9733b-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9733b-131">Request</span></span>
<span data-ttu-id="9733b-132">O exemplo a seguir mostra uma solicitação para recuperar todas as séries de revisão de acesso em um locatário.</span><span class="sxs-lookup"><span data-stu-id="9733b-132">The following example shows a request to retrieve all the access review series in a tenant.</span></span>


# <a name="http"></a>[<span data-ttu-id="9733b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="9733b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessReviewInstance_pendingapproval"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/pendingAccessReviewInstances?$expand=definition&$top=100&$skip=0
```
# <a name="c"></a>[<span data-ttu-id="9733b-134">C#</span><span class="sxs-lookup"><span data-stu-id="9733b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewinstance-pendingapproval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9733b-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9733b-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewinstance-pendingapproval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9733b-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9733b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewinstance-pendingapproval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9733b-137">Java</span><span class="sxs-lookup"><span data-stu-id="9733b-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewinstance-pendingapproval-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9733b-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="9733b-138">Response</span></span>
><span data-ttu-id="9733b-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9733b-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewInstance",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.count": 1,
    "value": [
        {
            "id": "70a68410-67f3-4d4c-b946-6989e050be19",
            "startDateTime": "2020-09-09T15:57:56Z",
            "endDateTime": "2020-10-08T15:57:56Z",
            "status": "InProgress",
            "scope": {
                "query": "/groups/04b3d70b-c770-46cb-b751-d857d2beedff/transitiveMembers",
                "queryType": "MicrosoftGraph"
            },
            "definition": {
                "id": "70a68410-67f3-4d4c-b946-6989e050be19",
                "displayName": "review of leadership",
                "createdDateTime": "2020-09-08T15:59:06Z",
                "lastModifiedDateTime": "2020-09-09T15:58:24Z",
                "status": "InProgress",
                "descriptionForAdmins": "review of leadership",
                "descriptionForReviewers": "",
                "createdBy": {
                    "id": "957f1027-c0ee-460d-9269-b8828e59e0fe",
                    "displayName": "MOD Administrator",
                    "userPrincipalName": "admin@msft.com"
                },
                "scope": {
                    "query": "/groups/04b3d70b-c770-46cb-b751-d857d2beedff/transitiveMembers",
                    "queryType": "MicrosoftGraph"
                },
                "instanceEnumerationScope": {
                    "query": "/groups/04b3d70b-c770-46cb-b751-d857d2beedff",
                    "queryType": "MicrosoftGraph"
                },
                "reviewers": [
                    {
                        "query": "/users/957f1027-c0ee-460d-9269-b8828e59e0fe",
                        "queryType": "MicrosoftGraph",
                        "queryRoot": null
                    }
                ],
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
                        "pattern": null,
                        "range": {
                            "type": "numbered",
                            "numberOfOccurrences": 0,
                            "recurrenceTimeZone": null,
                            "startDate": "2020-09-09",
                            "endDate": "2020-10-08"
                        }
                    },
                    "applyActions": [
                        {
                            "@odata.type": "#microsoft.graph.removeAccessApplyAction"
                        }
                    ]
                }
            }
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="9733b-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="9733b-140">See also</span></span>

- [<span data-ttu-id="9733b-141">Obter accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="9733b-141">Get accessReviewInstance</span></span>](accessreviewinstance-get.md)
- [<span data-ttu-id="9733b-142">Obter a aprovação pendente accessReviewInstanceDecisionItems</span><span class="sxs-lookup"><span data-stu-id="9733b-142">Get accessReviewInstanceDecisionItems pending approval</span></span>](accessreviewinstancedecisionitem-listpendingapproval.md)


<!--
{
  "type": "#page.annotation",
  "description": "List accessReviewInstance pendingApproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
