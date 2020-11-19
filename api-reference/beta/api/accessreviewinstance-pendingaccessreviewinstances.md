---
title: 'accessReviewInstance: pendingAccessReviewInstances'
description: Recupere objetos accessReviewInstance com aprovação pendente chamando o usuário.
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 793192a647865d524754f20be7d1deb664821d44
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49221997"
---
# <a name="accessreviewinstance-pendingaccessreviewinstances"></a><span data-ttu-id="576e6-103">accessReviewInstance: pendingAccessReviewInstances</span><span class="sxs-lookup"><span data-stu-id="576e6-103">accessReviewInstance: pendingAccessReviewInstances</span></span>

<span data-ttu-id="576e6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="576e6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="576e6-105">Recupere os objetos [accessReviewInstance](../resources/accessreviewinstance.md) com aprovação pendente pelo usuário de chamada.</span><span class="sxs-lookup"><span data-stu-id="576e6-105">Retrieve the [accessReviewInstance](../resources/accessreviewinstance.md) objects pending approval by the calling user.</span></span> <span data-ttu-id="576e6-106">Uma lista de zero ou mais objetos accessReviewInstance é retornada, da qual o usuário de chamada é um revisor atribuído.</span><span class="sxs-lookup"><span data-stu-id="576e6-106">A list of zero or more accessReviewInstance objects are returned, of which the calling user is an assigned reviewer.</span></span>

>[!NOTE]
><span data-ttu-id="576e6-107">Se muitos **accessReviewInstances** forem retornados, para melhorar a eficiência e evitar tempos limite, recupere o conjunto de resultados nas páginas, incluindo o parâmetro de consulta $Top com um tamanho de página de no máximo 100, e o parâmetro de consulta $Skip = 0 na solicitação.</span><span class="sxs-lookup"><span data-stu-id="576e6-107">If many **accessReviewInstances** are returned, to improve efficiency and avoid timeouts, retrieve the result set in pages, by including both the $top query parameter with a page size of at most 100, and the $skip=0 query parameter in the request.</span></span> <span data-ttu-id="576e6-108">Quando um conjunto de resultados abrange várias páginas, o Microsoft Graph retorna essa página com uma propriedade @odata. nextLink na resposta que contém uma URL para a próxima página de resultados.</span><span class="sxs-lookup"><span data-stu-id="576e6-108">When a result set spans multiple pages, Microsoft Graph returns that page with an @odata.nextLink property in the response that contains a URL to the next page of results.</span></span> <span data-ttu-id="576e6-109">Se essa propriedade estiver presente, continue fazendo solicitações adicionais com a URL @odata. nextLink em cada resposta, até que todos os resultados sejam retornados, conforme descrito em paginação de dados do Microsoft Graph em seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="576e6-109">If that property is present, continue making additional requests with the @odata.nextLink URL in each response, until all the results are returned, as described in paging Microsoft Graph data in your app.</span></span>
>
><span data-ttu-id="576e6-110">Se nenhum parâmetro de consulta for fornecido e houver mais de 100 resultados, o Microsoft Graph pausará automaticamente os resultados a 100 resultados por página.</span><span class="sxs-lookup"><span data-stu-id="576e6-110">If no query parameters are provided and there are more than 100 results, Microsoft Graph will automatically paginate results at 100 results per page.</span></span>

## <a name="permissions"></a><span data-ttu-id="576e6-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="576e6-111">Permissions</span></span>
<span data-ttu-id="576e6-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="576e6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="576e6-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="576e6-114">Permission type</span></span>                        | <span data-ttu-id="576e6-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="576e6-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="576e6-116">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="576e6-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="576e6-117">AccessReview. Read. All, AccessReview. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="576e6-117">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |

 <span data-ttu-id="576e6-118">O usuário conectado só vê instâncias das quais eles estão atribuídos revisor no accessReviewScheduleDefinition da instância.</span><span class="sxs-lookup"><span data-stu-id="576e6-118">The signed-in user only sees instances of which they are assigned reviewer in the accessReviewScheduleDefinition of the instance.</span></span>

## <a name="http-request"></a><span data-ttu-id="576e6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="576e6-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/pendingAccessReviewInstances
```
## <a name="request-headers"></a><span data-ttu-id="576e6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="576e6-120">Request headers</span></span>
<span data-ttu-id="576e6-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="576e6-121">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="576e6-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="576e6-122">Request body</span></span>
<span data-ttu-id="576e6-123">Não forneça um corpo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="576e6-123">Do not supply a request body.</span></span>

## <a name="response"></a><span data-ttu-id="576e6-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="576e6-124">Response</span></span>
<span data-ttu-id="576e6-125">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma matriz de objetos [accessReviewInstance](../resources/accessreviewinstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="576e6-125">If successful, this method returns a `200 OK` response code and an array of [accessReviewInstance](../resources/accessreviewinstance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="576e6-126">Exemplos</span><span class="sxs-lookup"><span data-stu-id="576e6-126">Examples</span></span>
### <a name="request"></a><span data-ttu-id="576e6-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="576e6-127">Request</span></span>
<span data-ttu-id="576e6-128">O exemplo a seguir mostra uma solicitação para recuperar todas as séries de revisão do Access em um locatário.</span><span class="sxs-lookup"><span data-stu-id="576e6-128">The following example shows a request to retrieve all the access review series in a tenant.</span></span>


# <a name="http"></a>[<span data-ttu-id="576e6-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="576e6-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessReviewInstance_pendingapproval"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/pendingAccessReviewInstances?$expand=definition&$top=100&$skip=0
```
# <a name="c"></a>[<span data-ttu-id="576e6-130">C#</span><span class="sxs-lookup"><span data-stu-id="576e6-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewinstance-pendingapproval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="576e6-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="576e6-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewinstance-pendingapproval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="576e6-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="576e6-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewinstance-pendingapproval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="576e6-133">Java</span><span class="sxs-lookup"><span data-stu-id="576e6-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewinstance-pendingapproval-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="576e6-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="576e6-134">Response</span></span>
><span data-ttu-id="576e6-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="576e6-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="576e6-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="576e6-137">See also</span></span>

- [<span data-ttu-id="576e6-138">Obter accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="576e6-138">Get accessReviewInstance</span></span>](accessreviewinstance-get.md)
- [<span data-ttu-id="576e6-139">Obter aprovação pendente accessReviewInstanceDecisionItems</span><span class="sxs-lookup"><span data-stu-id="576e6-139">Get accessReviewInstanceDecisionItems pending approval</span></span>](accessreviewinstancedecisionitem-listpendingapproval.md)


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
