---
title: Listar accessReviewInstance
description: Recupere objetos accessReviewInstance.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 52844146764ffb85be50a9c8d8609b466a88ba2e
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030520"
---
# <a name="list-accessreviewinstance"></a><span data-ttu-id="0fb77-103">Listar accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="0fb77-103">List accessReviewInstance</span></span>

<span data-ttu-id="0fb77-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0fb77-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0fb77-105">Recupere os [objetos accessReviewInstance](../resources/accessreviewinstance.md) para um [accessReviewScheduleDefinition específico.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0fb77-105">Retrieve the [accessReviewInstance](../resources/accessreviewinstance.md) objects for a specific [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="0fb77-106">Uma lista de zero ou mais **objetos accessReviewInstance** são retornados, incluindo todas as propriedades aninhadas.</span><span class="sxs-lookup"><span data-stu-id="0fb77-106">A list of zero or more **accessReviewInstance** objects are returned, including all of their nested properties.</span></span> <span data-ttu-id="0fb77-107">Os objetos retornados não incluem accessReviewInstanceDecisionItems associados.</span><span class="sxs-lookup"><span data-stu-id="0fb77-107">Returned objects do not include associated accessReviewInstanceDecisionItems.</span></span> <span data-ttu-id="0fb77-108">Para recuperar as decisões na instância, use [List accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem-list.md).</span><span class="sxs-lookup"><span data-stu-id="0fb77-108">To retrieve the decisions on the instance, use [List accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem-list.md).</span></span>

>[!NOTE]
><span data-ttu-id="0fb77-109">O tamanho padrão da página para essa API é de 100 objetos accessReviewInstance.</span><span class="sxs-lookup"><span data-stu-id="0fb77-109">The default page size for this API is 100 accessReviewInstance objects.</span></span> <span data-ttu-id="0fb77-110">Para melhorar a eficiência e evitar tempos-de-tempo devido a grandes conjuntos de resultados, aplique paginação usando os `$skip` parâmetros e `$top` de consulta.</span><span class="sxs-lookup"><span data-stu-id="0fb77-110">To improve efficiency and avoid timeouts due to large result sets, apply pagination using the `$skip` and `$top` query parameters.</span></span> <span data-ttu-id="0fb77-111">Para mais informações, consulte [Paginação de dados do Microsoft Graph em seu aplicativo](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="0fb77-111">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="0fb77-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="0fb77-112">Permissions</span></span>
<span data-ttu-id="0fb77-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0fb77-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0fb77-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0fb77-115">Permission type</span></span>                        | <span data-ttu-id="0fb77-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0fb77-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0fb77-117">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0fb77-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="0fb77-118">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fb77-118">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="0fb77-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0fb77-119">Application</span></span>                            | <span data-ttu-id="0fb77-120">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fb77-120">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span> |

<span data-ttu-id="0fb77-121">O usuário interno também deve estar em uma função de diretório que permita que ele leia uma revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="0fb77-121">The signed-in user must also be in a directory role that permits them to read an access review.</span></span> <span data-ttu-id="0fb77-122">Para exibir apenas as instâncias em que o usuário interno recebe o revistor, consulte [Listar instâncias de](accessreviewinstance-pendingaccessreviewinstances.md) revisão de acesso pendentes</span><span class="sxs-lookup"><span data-stu-id="0fb77-122">To view just the instances that the signed-in user is assigned the reviewer on, see [List pending access review instances](accessreviewinstance-pendingaccessreviewinstances.md)</span></span>

## <a name="http-request"></a><span data-ttu-id="0fb77-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0fb77-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/accessReviews/definitions/{definition-id}/instances
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0fb77-124">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0fb77-124">Optional query parameters</span></span>
<span data-ttu-id="0fb77-125">Este método dá suporte a parâmetros de consulta `$select` , , , e `$filter` `$orderBy` `$skip` `$top` OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0fb77-125">This method supports `$select`, `$filter`, `$orderBy`, `$skip`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="0fb77-126">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="0fb77-126">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0fb77-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0fb77-127">Request headers</span></span>
<span data-ttu-id="0fb77-128">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0fb77-128">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="0fb77-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0fb77-129">Request body</span></span>
<span data-ttu-id="0fb77-130">Não fornecer um corpo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0fb77-130">Do not supply a request body.</span></span>

## <a name="response"></a><span data-ttu-id="0fb77-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fb77-131">Response</span></span>
<span data-ttu-id="0fb77-132">Se tiver êxito, este método retornará um código de resposta e uma matriz de `200 OK` [objetos accessReviewInstance](../resources/accessreviewinstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0fb77-132">If successful, this method returns a `200 OK` response code and an array of [accessReviewInstance](../resources/accessreviewinstance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0fb77-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0fb77-133">Examples</span></span>
### <a name="request"></a><span data-ttu-id="0fb77-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0fb77-134">Request</span></span>
<span data-ttu-id="0fb77-135">O exemplo a seguir mostra uma solicitação para recuperar todas as instâncias de revisão de acesso para uma definição.</span><span class="sxs-lookup"><span data-stu-id="0fb77-135">The following example shows a request to retrieve all the access review instances for a definition.</span></span>


# <a name="http"></a>[<span data-ttu-id="0fb77-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="0fb77-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessReviewInstance"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/8564a649-4f67-4e09-88e7-55def6530e88/instances?$top=100&$skip=0
```
# <a name="c"></a>[<span data-ttu-id="0fb77-137">C#</span><span class="sxs-lookup"><span data-stu-id="0fb77-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewinstance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0fb77-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0fb77-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewinstance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0fb77-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0fb77-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewinstance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0fb77-140">Java</span><span class="sxs-lookup"><span data-stu-id="0fb77-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewinstance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0fb77-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="0fb77-141">Response</span></span>
><span data-ttu-id="0fb77-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0fb77-142">**Note:** The response object shown here might be shortened for readability.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="0fb77-143">Confira também</span><span class="sxs-lookup"><span data-stu-id="0fb77-143">See also</span></span>

- [<span data-ttu-id="0fb77-144">Listar accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="0fb77-144">List accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-list.md)
- [<span data-ttu-id="0fb77-145">Obter accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="0fb77-145">Get accessReviewInstance</span></span>](accessreviewinstance-get.md)


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
