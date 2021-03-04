---
title: 'accessReviewInstance: pendingAccessReviewInstances'
description: Recupere os objetos accessReviewInstance aguardando aprovação chamando o usuário.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 82ae31f82b9c9609403221bc7a0e82c0e220941d
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439151"
---
# <a name="accessreviewinstance-pendingaccessreviewinstances"></a><span data-ttu-id="f02d3-103">accessReviewInstance: pendingAccessReviewInstances</span><span class="sxs-lookup"><span data-stu-id="f02d3-103">accessReviewInstance: pendingAccessReviewInstances</span></span>

<span data-ttu-id="f02d3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f02d3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f02d3-105">Recupere os [objetos accessReviewInstance](../resources/accessreviewinstance.md) pendentes aprovação pelo usuário de chamada.</span><span class="sxs-lookup"><span data-stu-id="f02d3-105">Retrieve the [accessReviewInstance](../resources/accessreviewinstance.md) objects pending approval by the calling user.</span></span> <span data-ttu-id="f02d3-106">Uma lista de zero ou mais objetos accessReviewInstance são retornados, dos quais o usuário de chamada é um revisor atribuído.</span><span class="sxs-lookup"><span data-stu-id="f02d3-106">A list of zero or more accessReviewInstance objects are returned, of which the calling user is an assigned reviewer.</span></span>

>[!NOTE]
><span data-ttu-id="f02d3-107">Se muitos **accessReviewInstances são retornados,** para melhorar a eficiência e evitar tempos-extra, recupere o resultado definido em páginas, incluindo o parâmetro de consulta $top com um tamanho de página de no máximo 100 e o parâmetro de consulta $skip=0 na solicitação.</span><span class="sxs-lookup"><span data-stu-id="f02d3-107">If many **accessReviewInstances** are returned, to improve efficiency and avoid timeouts, retrieve the result set in pages, by including both the $top query parameter with a page size of at most 100, and the $skip=0 query parameter in the request.</span></span> <span data-ttu-id="f02d3-108">Quando um conjunto de resultados abrange várias páginas, o Microsoft Graph retorna essa página com uma propriedade @odata.nextLink na resposta que contém uma URL para a próxima página de resultados.</span><span class="sxs-lookup"><span data-stu-id="f02d3-108">When a result set spans multiple pages, Microsoft Graph returns that page with an @odata.nextLink property in the response that contains a URL to the next page of results.</span></span> <span data-ttu-id="f02d3-109">Se essa propriedade estiver presente, continue fazendo solicitações adicionais com a URL @odata.nextLink em cada resposta, até que todos os resultados sejam retornados, conforme descrito na paja de dados do Microsoft Graph em seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f02d3-109">If that property is present, continue making additional requests with the @odata.nextLink URL in each response, until all the results are returned, as described in paging Microsoft Graph data in your app.</span></span>
>
><span data-ttu-id="f02d3-110">Se nenhum parâmetro de consulta for fornecido e houver mais de 100 resultados, o Microsoft Graph paginará automaticamente os resultados em 100 resultados por página.</span><span class="sxs-lookup"><span data-stu-id="f02d3-110">If no query parameters are provided and there are more than 100 results, Microsoft Graph will automatically paginate results at 100 results per page.</span></span>

## <a name="permissions"></a><span data-ttu-id="f02d3-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="f02d3-111">Permissions</span></span>
<span data-ttu-id="f02d3-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f02d3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f02d3-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f02d3-114">Permission type</span></span>                        | <span data-ttu-id="f02d3-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f02d3-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f02d3-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f02d3-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="f02d3-117">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f02d3-117">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |

 <span data-ttu-id="f02d3-118">O usuário in-loco só vê instâncias das quais são atribuídas revisores no accessReviewScheduleDefinition da instância.</span><span class="sxs-lookup"><span data-stu-id="f02d3-118">The signed-in user only sees instances of which they are assigned reviewer in the accessReviewScheduleDefinition of the instance.</span></span>

## <a name="http-request"></a><span data-ttu-id="f02d3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f02d3-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/pendingAccessReviewInstances
```
## <a name="request-headers"></a><span data-ttu-id="f02d3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f02d3-120">Request headers</span></span>
<span data-ttu-id="f02d3-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f02d3-121">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="f02d3-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f02d3-122">Request body</span></span>
<span data-ttu-id="f02d3-123">Não fornecer um corpo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f02d3-123">Do not supply a request body.</span></span>

## <a name="response"></a><span data-ttu-id="f02d3-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="f02d3-124">Response</span></span>
<span data-ttu-id="f02d3-125">Se tiver êxito, este método retornará um código de resposta e uma matriz de `200 OK` [objetos accessReviewInstance](../resources/accessreviewinstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f02d3-125">If successful, this method returns a `200 OK` response code and an array of [accessReviewInstance](../resources/accessreviewinstance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f02d3-126">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f02d3-126">Examples</span></span>
### <a name="request"></a><span data-ttu-id="f02d3-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f02d3-127">Request</span></span>
<span data-ttu-id="f02d3-128">O exemplo a seguir mostra uma solicitação para recuperar todas as séries de revisão de acesso em um locatário.</span><span class="sxs-lookup"><span data-stu-id="f02d3-128">The following example shows a request to retrieve all the access review series in a tenant.</span></span>


# <a name="http"></a>[<span data-ttu-id="f02d3-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="f02d3-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessReviewInstance_pendingapproval"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/pendingAccessReviewInstances?$expand=definition&$top=100&$skip=0
```
# <a name="c"></a>[<span data-ttu-id="f02d3-130">C#</span><span class="sxs-lookup"><span data-stu-id="f02d3-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewinstance-pendingapproval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f02d3-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f02d3-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewinstance-pendingapproval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f02d3-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f02d3-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewinstance-pendingapproval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f02d3-133">Java</span><span class="sxs-lookup"><span data-stu-id="f02d3-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewinstance-pendingapproval-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f02d3-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f02d3-134">Response</span></span>
><span data-ttu-id="f02d3-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f02d3-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="f02d3-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="f02d3-137">See also</span></span>

- [<span data-ttu-id="f02d3-138">Obter accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="f02d3-138">Get accessReviewInstance</span></span>](accessreviewinstance-get.md)
- [<span data-ttu-id="f02d3-139">Obter a aprovação pendente accessReviewInstanceDecisionItems</span><span class="sxs-lookup"><span data-stu-id="f02d3-139">Get accessReviewInstanceDecisionItems pending approval</span></span>](accessreviewinstancedecisionitem-listpendingapproval.md)


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
