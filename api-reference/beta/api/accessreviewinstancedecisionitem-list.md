---
title: Listar accessReviewInstanceDecisionItem
description: Recupere objetos accessReviewInstanceDecisionItem.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: a89f6a1bc91f2449a280fe3bfcfaab918cd92e16
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030429"
---
# <a name="list-accessreviewinstancedecisionitem"></a><span data-ttu-id="1deff-103">Listar accessReviewInstanceDecisionItem</span><span class="sxs-lookup"><span data-stu-id="1deff-103">List accessReviewInstanceDecisionItem</span></span>

<span data-ttu-id="1deff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1deff-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1deff-105">Recupere os [objetos accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) para um [accessReviewInstance específico.](../resources/accessreviewinstance.md)</span><span class="sxs-lookup"><span data-stu-id="1deff-105">Retrieve the [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects for a specific [accessReviewInstance](../resources/accessreviewinstance.md).</span></span> <span data-ttu-id="1deff-106">Uma lista de zero ou mais objetos accessReviewInstanceDecisionItem é retornada, incluindo todas as suas propriedades aninhadas.</span><span class="sxs-lookup"><span data-stu-id="1deff-106">A list of zero or more accessReviewInstanceDecisionItem objects are returned, including all of their nested properties.</span></span>

>[!NOTE]
><span data-ttu-id="1deff-107">O tamanho padrão da página para essa API é de 100 objetos accessReviewInstanceDecisionItem.</span><span class="sxs-lookup"><span data-stu-id="1deff-107">The default page size for this API is 100 accessReviewInstanceDecisionItem objects.</span></span> <span data-ttu-id="1deff-108">Para melhorar a eficiência e evitar tempos-de-tempo devido a grandes conjuntos de resultados, aplique paginação usando os `$skip` parâmetros e `$top` de consulta.</span><span class="sxs-lookup"><span data-stu-id="1deff-108">To improve efficiency and avoid timeouts due to large result sets, apply pagination using the `$skip` and `$top` query parameters.</span></span> <span data-ttu-id="1deff-109">Para mais informações, consulte [Paginação de dados do Microsoft Graph em seu aplicativo](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="1deff-109">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="1deff-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="1deff-110">Permissions</span></span>
<span data-ttu-id="1deff-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1deff-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1deff-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1deff-113">Permission type</span></span>                        | <span data-ttu-id="1deff-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1deff-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="1deff-115">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1deff-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="1deff-116">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1deff-116">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="1deff-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1deff-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1deff-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1deff-118">Not supported.</span></span>|
|<span data-ttu-id="1deff-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1deff-119">Application</span></span>                            | <span data-ttu-id="1deff-120">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1deff-120">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span> |

 <span data-ttu-id="1deff-121">O usuário interno também deve estar em uma função de diretório que permita que ele leia uma revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="1deff-121">The signed-in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="1deff-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1deff-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/accessReviews/definitions/{definition-id}/instances/{instance-id}/decisions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1deff-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1deff-123">Optional query parameters</span></span>
<span data-ttu-id="1deff-124">Este método dá suporte a parâmetros de consulta `$select` , , , e `$filter` `$orderBy` `$skip` `$top` OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1deff-124">This method supports `$select`, `$filter`, `$orderBy`, `$skip`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="1deff-125">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1deff-125">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1deff-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1deff-126">Request headers</span></span>
<span data-ttu-id="1deff-127">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="1deff-127">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="1deff-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1deff-128">Request body</span></span>
<span data-ttu-id="1deff-129">Não fornecer um corpo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1deff-129">Do not supply a request body.</span></span>

## <a name="response"></a><span data-ttu-id="1deff-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="1deff-130">Response</span></span>
<span data-ttu-id="1deff-131">Se tiver êxito, este método retornará um código de resposta e uma matriz de `200 OK` [objetos accessReviewInstanceDecisionItem](../resources/accessreviewinstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1deff-131">If successful, this method returns a `200 OK` response code and an array of [accessReviewInstanceDecisionItem](../resources/accessreviewinstance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1deff-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1deff-132">Examples</span></span>
### <a name="request"></a><span data-ttu-id="1deff-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1deff-133">Request</span></span>
<span data-ttu-id="1deff-134">O exemplo a seguir mostra uma solicitação para recuperar todas as decisões em uma instância de uma revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="1deff-134">The following example shows a request to retrieve all the decisions on an instance of an access review.</span></span>


# <a name="http"></a>[<span data-ttu-id="1deff-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="1deff-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessReviewInstanceDecisionItem"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/60860cdd-fb4d-4054-91ba-444404f3baa6/instances/14444cdb-6a18-4c08-ba2c-48c02f0a0138/decisions?$top=100&$skip=0
```
# <a name="c"></a>[<span data-ttu-id="1deff-136">C#</span><span class="sxs-lookup"><span data-stu-id="1deff-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewinstancedecisionitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1deff-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1deff-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewinstancedecisionitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1deff-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1deff-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewinstancedecisionitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1deff-139">Java</span><span class="sxs-lookup"><span data-stu-id="1deff-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewinstancedecisionitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="1deff-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="1deff-140">Response</span></span>
><span data-ttu-id="1deff-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1deff-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItem",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions('5eac5a70-7cd7-4f20-92b0-f9dba70dd7f0')/instances('6444d4fd-ab55-4608-8cf9-c6702d172bcc')/decisions",
    "@odata.count": 2,
    "value": [
        {
            "id": "e6cafba0-cbf0-4748-8868-0810c7f4cc06",
            "accessReviewId": "6444d4fd-ab55-4608-8cf9-c6702d172bcc",
            "reviewedDateTime": null,
            "decision": "NotReviewed",
            "justification": "",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Approve",
            "principalLink": "https://graph.microsoft.com/v1.0/users/04777c4b-4d43-4d32-a2e7-1eba5d03f8cf",
            "resourceLink": null,
            "resource": null,
            "reviewedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "target": {
                "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
                "userId": "04777c4b-4d43-4d32-a2e7-1eba5d03f8cf",
                "userDisplayName": "Diego Siciliani",
                "userPrincipalName": "DiegoS@contoso.com"
            },
            "principal": {
                "@odata.type": "#microsoft.graph.userIdentity",
                "id": "04777c4b-4d43-4d32-a2e7-1eba5d03f8cf",
                "displayName": "Diego Siciliani",
                "userPrincipalName": "DiegoS@contoso.com"
            }
        },
        {
            "id": "4bde8d40-9224-4aa3-936b-08d73e1baf47",
            "accessReviewId": "6444d4fd-ab55-4608-8cf9-c6702d172bcc",
            "reviewedDateTime": null,
            "decision": "NotReviewed",
            "justification": "",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Approve",
            "principalLink": "https://graph.microsoft.com/v1.0/users/11feb738-0039-4a6c-a045-dcb91a47969a",
            "resourceLink": null,
            "resource": null,
            "reviewedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "target": {
                "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
                "userId": "11feb738-0039-4a6c-a045-dcb91a47969a",
                "userDisplayName": "Johanna Lorenz",
                "userPrincipalName": "JohannaL@contoso.com"
            },
            "principal": {
                "@odata.type": "#microsoft.graph.userIdentity",
                "id": "11feb738-0039-4a6c-a045-dcb91a47969a",
                "displayName": "Johanna Lorenz",
                "userPrincipalName": "JohannaL@contoso.com"
            }
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="1deff-142">Confira também</span><span class="sxs-lookup"><span data-stu-id="1deff-142">See also</span></span>

- [<span data-ttu-id="1deff-143">Obter accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="1deff-143">Get accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-get.md)
- [<span data-ttu-id="1deff-144">Obter accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="1deff-144">Get accessReviewInstance</span></span>](accessreviewinstance-get.md)


<!--
{
  "type": "#page.annotation",
  "description": "List accessReviewInstanceDecisionItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
