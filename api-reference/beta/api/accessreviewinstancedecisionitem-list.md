---
title: Listar accessReviewInstanceDecisionItem
description: Recupere objetos accessReviewInstanceDecisionItem.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 7674a129b118c2c9d8c3487623cf039b2ceca603
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048397"
---
# <a name="list-accessreviewinstancedecisionitem"></a><span data-ttu-id="1a8ac-103">Listar accessReviewInstanceDecisionItem</span><span class="sxs-lookup"><span data-stu-id="1a8ac-103">List accessReviewInstanceDecisionItem</span></span>

<span data-ttu-id="1a8ac-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a8ac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a8ac-105">Recupere os [objetos accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) para um [accessReviewInstance específico.](../resources/accessreviewinstance.md)</span><span class="sxs-lookup"><span data-stu-id="1a8ac-105">Retrieve the [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects for a specific [accessReviewInstance](../resources/accessreviewinstance.md).</span></span> <span data-ttu-id="1a8ac-106">Uma lista de zero ou mais objetos accessReviewInstanceDecisionItem é retornada, incluindo todas as suas propriedades aninhadas.</span><span class="sxs-lookup"><span data-stu-id="1a8ac-106">A list of zero or more accessReviewInstanceDecisionItem objects are returned, including all of their nested properties.</span></span>

>[!NOTE]
><span data-ttu-id="1a8ac-107">Se muitos **accessReviewInstanceDecisionItems são retornados,** para melhorar a eficiência e evitar tempos-de-tempo, recupere o conjunto de resultados definido em páginas, incluindo o parâmetro de consulta $top com um tamanho de página de no máximo 100 e o parâmetro de consulta $skip=0 na solicitação.</span><span class="sxs-lookup"><span data-stu-id="1a8ac-107">If many **accessReviewInstanceDecisionItems** are returned, to improve efficiency and avoid timeouts, retrieve the result set in pages, by including both the $top query parameter with a page size of at most 100, and the $skip=0 query parameter in the request.</span></span> <span data-ttu-id="1a8ac-108">Quando um conjunto de resultados abrange várias páginas, o Microsoft Graph retorna essa página com uma propriedade @odata.nextLink na resposta que contém uma URL para a próxima página de resultados.</span><span class="sxs-lookup"><span data-stu-id="1a8ac-108">When a result set spans multiple pages, Microsoft Graph returns that page with an @odata.nextLink property in the response that contains a URL to the next page of results.</span></span> <span data-ttu-id="1a8ac-109">Se essa propriedade estiver presente, continue fazendo solicitações adicionais com a URL @odata.nextLink em cada resposta, até que todos os resultados sejam retornados, conforme descrito na pa paja do Microsoft Graph dados em seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1a8ac-109">If that property is present, continue making additional requests with the @odata.nextLink URL in each response, until all the results are returned, as described in paging Microsoft Graph data in your app.</span></span>
>
><span data-ttu-id="1a8ac-110">Se nenhum parâmetro de consulta for fornecido e houver mais de 100 resultados, o Microsoft Graph paginará automaticamente os resultados em 100 resultados por página.</span><span class="sxs-lookup"><span data-stu-id="1a8ac-110">If no query parameters are provided and there are more than 100 results, Microsoft Graph will automatically paginate results at 100 results per page.</span></span>

## <a name="permissions"></a><span data-ttu-id="1a8ac-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="1a8ac-111">Permissions</span></span>
<span data-ttu-id="1a8ac-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a8ac-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a8ac-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1a8ac-114">Permission type</span></span>                        | <span data-ttu-id="1a8ac-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1a8ac-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a8ac-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1a8ac-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="1a8ac-117">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a8ac-117">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="1a8ac-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1a8ac-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a8ac-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1a8ac-119">Not supported.</span></span>|
|<span data-ttu-id="1a8ac-120">Application</span><span class="sxs-lookup"><span data-stu-id="1a8ac-120">Application</span></span>                            | <span data-ttu-id="1a8ac-121">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a8ac-121">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span> |

 <span data-ttu-id="1a8ac-122">O usuário interno também deve estar em uma função de diretório que permita que ele leia uma revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="1a8ac-122">The signed-in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="1a8ac-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1a8ac-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/accessReviews/definitions/{definition-id}/instances/{instance-id}/decisions
```
## <a name="request-headers"></a><span data-ttu-id="1a8ac-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1a8ac-124">Request headers</span></span>
<span data-ttu-id="1a8ac-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1a8ac-125">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="1a8ac-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1a8ac-126">Request body</span></span>
<span data-ttu-id="1a8ac-127">Não fornecer um corpo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1a8ac-127">Do not supply a request body.</span></span>

## <a name="response"></a><span data-ttu-id="1a8ac-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a8ac-128">Response</span></span>
<span data-ttu-id="1a8ac-129">Se tiver êxito, este método retornará um código de resposta e uma matriz de `200 OK` [objetos accessReviewInstanceDecisionItem](../resources/accessreviewinstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1a8ac-129">If successful, this method returns a `200 OK` response code and an array of [accessReviewInstanceDecisionItem](../resources/accessreviewinstance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1a8ac-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1a8ac-130">Examples</span></span>
### <a name="request"></a><span data-ttu-id="1a8ac-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1a8ac-131">Request</span></span>
<span data-ttu-id="1a8ac-132">O exemplo a seguir mostra uma solicitação para recuperar todas as decisões em uma instância de uma revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="1a8ac-132">The following example shows a request to retrieve all the decisions on an instance of an access review.</span></span>


# <a name="http"></a>[<span data-ttu-id="1a8ac-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="1a8ac-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessReviewInstanceDecisionItem"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/60860cdd-fb4d-4054-91ba-444404f3baa6/instances/14444cdb-6a18-4c08-ba2c-48c02f0a0138/decisions?$top=100&$skip=0
```
# <a name="c"></a>[<span data-ttu-id="1a8ac-134">C#</span><span class="sxs-lookup"><span data-stu-id="1a8ac-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewinstancedecisionitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1a8ac-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1a8ac-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewinstancedecisionitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1a8ac-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1a8ac-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewinstancedecisionitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1a8ac-137">Java</span><span class="sxs-lookup"><span data-stu-id="1a8ac-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewinstancedecisionitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="1a8ac-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a8ac-138">Response</span></span>
><span data-ttu-id="1a8ac-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1a8ac-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.count": 4,
    "value": [
        {
            "id": "77a61af9-3bef-4bbf-b00b-04734d6d5eae",
            "accessReviewId": "70463350-742e-4909-bfa5-bc23447bd002",
            "reviewedDateTime": null,
            "decision": "NotReviewed",
            "justification": "",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Deny",
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
                "userId": "3736c87b-dc21-4290-8802-d6fef5fa3a08",
                "userDisplayName": "Irvin Sayers",
                "userPrincipalName": "IrvinS@M365x471116.OnMicrosoft.com"
            }
        },
        {
            "id": "f30b68ef-b843-4479-86b8-0a3a2f4bb209",
            "accessReviewId": "70463350-742e-4909-bfa5-bc23447bd002",
            "reviewedDateTime": "2020-09-18T16:56:08.377Z",
            "decision": "Approve",
            "justification": "This employee needs access for reason X",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Deny",
            "reviewedBy": {
                "id": "957f1027-c0ee-460d-9269-b8828e59e0fe",
                "displayName": "MOD Administrator",
                "userPrincipalName": "MOD Administrator"
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "target": {
                "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
                "userId": "ecd78419-3f1e-4f07-9bd9-7c77137af4f1",
                "userDisplayName": "Bianca Pisani",
                "userPrincipalName": "BiancaP@M365x471116.OnMicrosoft.com"
            }
        },
        {
            "id": "037b737f-e8ca-4507-b126-5a0620ba2c18",
            "accessReviewId": "70463350-742e-4909-bfa5-bc23447bd002",
            "reviewedDateTime": "2020-09-18T16:56:28.473Z",
            "decision": "Deny",
            "justification": "This employee changed roles and no longer needs access",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Deny",
            "reviewedBy": {
                "id": "957f1027-c0ee-460d-9269-b8828e59e0fe",
                "displayName": "MOD Administrator",
                "userPrincipalName": "MOD Administrator"
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "target": {
                "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
                "userId": "5f16b75b-031c-4944-9691-070f03273079",
                "userDisplayName": "Delia Dennis",
                "userPrincipalName": "DeliaD@M365x471116.OnMicrosoft.com"
            }
        },
        {
            "id": "7032f455-10a3-4d04-bf02-66fb65d26d10",
            "accessReviewId": "70463350-742e-4909-bfa5-bc23447bd002",
            "reviewedDateTime": "2020-09-18T16:56:44.38Z",
            "decision": "DontKnow",
            "justification": "I do not know what this employee needs",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Deny",
            "reviewedBy": {
                "id": "957f1027-c0ee-460d-9269-b8828e59e0fe",
                "displayName": "MOD Administrator",
                "userPrincipalName": "MOD Administrator"
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "target": {
                "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
                "userId": "4169762e-895f-4350-a13d-e5b09b1efcfa",
                "userDisplayName": "Isaiah Langer",
                "userPrincipalName": "IsaiahL@M365x471116.OnMicrosoft.com"
            }
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="1a8ac-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="1a8ac-140">See also</span></span>

- [<span data-ttu-id="1a8ac-141">Obter accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="1a8ac-141">Get accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-get.md)
- [<span data-ttu-id="1a8ac-142">Obter accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="1a8ac-142">Get accessReviewInstance</span></span>](accessreviewinstance-get.md)


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
