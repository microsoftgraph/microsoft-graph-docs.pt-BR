---
title: Listar accessReviewInstance
description: Recupere objetos accessReviewInstance.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 59795800be0bf7146262ec82c01265b969e194e1
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51468937"
---
# <a name="list-accessreviewinstance"></a><span data-ttu-id="77225-103">Listar accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="77225-103">List accessReviewInstance</span></span>

<span data-ttu-id="77225-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77225-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77225-105">Recupere os [objetos accessReviewInstance](../resources/accessreviewinstance.md) para um [accessReviewScheduleDefinition específico.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="77225-105">Retrieve the [accessReviewInstance](../resources/accessreviewinstance.md) objects for a specific [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="77225-106">Uma lista de zero ou mais **objetos accessReviewInstance** são retornados, incluindo todas as propriedades aninhadas.</span><span class="sxs-lookup"><span data-stu-id="77225-106">A list of zero or more **accessReviewInstance** objects are returned, including all of their nested properties.</span></span> <span data-ttu-id="77225-107">Os objetos retornados não incluem accessReviewInstanceDecisionItems associados.</span><span class="sxs-lookup"><span data-stu-id="77225-107">Returned objects do not include associated accessReviewInstanceDecisionItems.</span></span> <span data-ttu-id="77225-108">Para recuperar as decisões na instância, use [List accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem-list.md).</span><span class="sxs-lookup"><span data-stu-id="77225-108">To retrieve the decisions on the instance, use [List accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem-list.md).</span></span>

>[!NOTE]
><span data-ttu-id="77225-109">Se muitos **accessReviewInstances são retornados,** para melhorar a eficiência e evitar tempos-extra, recupere o resultado definido em páginas, incluindo o parâmetro de consulta $top com um tamanho de página de no máximo 100 e o parâmetro de consulta $skip=0 na solicitação.</span><span class="sxs-lookup"><span data-stu-id="77225-109">If many **accessReviewInstances** are returned, to improve efficiency and avoid timeouts, retrieve the result set in pages, by including both the $top query parameter with a page size of at most 100, and the $skip=0 query parameter in the request.</span></span> <span data-ttu-id="77225-110">Quando um conjunto de resultados abrange várias páginas, o Microsoft Graph retorna essa página com uma propriedade @odata.nextLink na resposta que contém uma URL para a próxima página de resultados.</span><span class="sxs-lookup"><span data-stu-id="77225-110">When a result set spans multiple pages, Microsoft Graph returns that page with an @odata.nextLink property in the response that contains a URL to the next page of results.</span></span> <span data-ttu-id="77225-111">Se essa propriedade estiver presente, continue fazendo solicitações adicionais com a URL @odata.nextLink em cada resposta, até que todos os resultados sejam retornados, conforme descrito na paja de dados do Microsoft Graph em seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="77225-111">If that property is present, continue making additional requests with the @odata.nextLink URL in each response, until all the results are returned, as described in paging Microsoft Graph data in your app.</span></span>
>
><span data-ttu-id="77225-112">Se nenhum parâmetro de consulta for fornecido e houver mais de 100 resultados, o Microsoft Graph paginará automaticamente os resultados em 100 resultados por página.</span><span class="sxs-lookup"><span data-stu-id="77225-112">If no query parameters are provided and there are more than 100 results, Microsoft Graph will automatically paginate results at 100 results per page.</span></span>

## <a name="permissions"></a><span data-ttu-id="77225-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="77225-113">Permissions</span></span>
<span data-ttu-id="77225-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77225-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77225-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="77225-116">Permission type</span></span>                        | <span data-ttu-id="77225-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="77225-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="77225-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="77225-118">Delegated (work or school account)</span></span>     | <span data-ttu-id="77225-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77225-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="77225-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="77225-120">Application</span></span>                            | <span data-ttu-id="77225-121">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77225-121">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span> |

<span data-ttu-id="77225-122">O usuário interno também deve estar em uma função de diretório que permita que ele leia uma revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="77225-122">The signed-in user must also be in a directory role that permits them to read an access review.</span></span> <span data-ttu-id="77225-123">Para exibir apenas as instâncias em que o usuário interno recebe o revistor, consulte [Listar instâncias de](accessreviewinstance-pendingaccessreviewinstances.md) revisão de acesso pendentes</span><span class="sxs-lookup"><span data-stu-id="77225-123">To view just the instances that the signed-in user is assigned the reviewer on, see [List pending access review instances](accessreviewinstance-pendingaccessreviewinstances.md)</span></span>

## <a name="http-request"></a><span data-ttu-id="77225-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="77225-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/accessReviews/definitions/{definition-id}/instances
```
## <a name="request-headers"></a><span data-ttu-id="77225-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="77225-125">Request headers</span></span>
<span data-ttu-id="77225-126">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="77225-126">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="77225-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="77225-127">Request body</span></span>
<span data-ttu-id="77225-128">Não fornecer um corpo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="77225-128">Do not supply a request body.</span></span>

## <a name="response"></a><span data-ttu-id="77225-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="77225-129">Response</span></span>
<span data-ttu-id="77225-130">Se tiver êxito, este método retornará um código de resposta e uma matriz de `200 OK` [objetos accessReviewInstance](../resources/accessreviewinstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="77225-130">If successful, this method returns a `200 OK` response code and an array of [accessReviewInstance](../resources/accessreviewinstance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="77225-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="77225-131">Examples</span></span>
### <a name="request"></a><span data-ttu-id="77225-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="77225-132">Request</span></span>
<span data-ttu-id="77225-133">O exemplo a seguir mostra uma solicitação para recuperar todas as instâncias de revisão de acesso para uma definição.</span><span class="sxs-lookup"><span data-stu-id="77225-133">The following example shows a request to retrieve all the access review instances for a definition.</span></span>


# <a name="http"></a>[<span data-ttu-id="77225-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="77225-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessReviewInstance"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/8564a649-4f67-4e09-88e7-55def6530e88/instances?$top=100&$skip=0
```
# <a name="c"></a>[<span data-ttu-id="77225-135">C#</span><span class="sxs-lookup"><span data-stu-id="77225-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewinstance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="77225-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="77225-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewinstance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="77225-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="77225-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewinstance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="77225-138">Java</span><span class="sxs-lookup"><span data-stu-id="77225-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewinstance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="77225-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="77225-139">Response</span></span>
><span data-ttu-id="77225-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="77225-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions('8564a649-4f67-4e09-88e7-55def6530e88')/instances",
    "@odata.count": 2,
    "value": [
        {
            "id": "7bc18cf4-3d70-4009-bc8e-a7c5adb30849",
            "startDateTime": "2021-03-09T23:10:28.83Z",
            "endDateTime": "2021-03-09T23:10:28.83Z",
            "status": "Applied",
            "scope": {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/v1.0/groups/f661fdd0-f0f7-42c0-8281-e89c6527ac63/members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
                "queryType": "MicrosoftGraph",
                "queryRoot": null
            }
        },
        {
            "id": "f1f35945-3f42-4941-9f7b-465e545f6f99",
            "startDateTime": "2021-03-09T23:10:28.83Z",
            "endDateTime": "2021-03-09T23:10:28.83Z",
            "status": "Applied",
            "scope": {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/v1.0/groups/f4ac55b3-3b3c-417e-85bd-183bbda3ccf2/members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
                "queryType": "MicrosoftGraph",
                "queryRoot": null
            }
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="77225-142">Confira também</span><span class="sxs-lookup"><span data-stu-id="77225-142">See also</span></span>

- [<span data-ttu-id="77225-143">Listar accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="77225-143">List accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-list.md)
- [<span data-ttu-id="77225-144">Obter accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="77225-144">Get accessReviewInstance</span></span>](accessreviewinstance-get.md)


<!--
{
  "type": "#page.annotation",
  "description": "List accessReviewInstance",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
