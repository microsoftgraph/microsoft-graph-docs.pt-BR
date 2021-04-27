---
title: Listar a aprovação pendente accessReviewInstanceDecisionItem
description: Recupere os objetos accessReviewInstanceDecisionItem aguardando aprovação do usuário chamador.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 2eabb7f646806d501dfacad8aa2b22e8cb5e95ee
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048383"
---
# <a name="list-accessreviewinstancedecisionitems-pending-approval"></a><span data-ttu-id="07b27-103">Listar accessReviewInstanceDecisionItems aguardando aprovação</span><span class="sxs-lookup"><span data-stu-id="07b27-103">List accessReviewInstanceDecisionItems pending approval</span></span>

<span data-ttu-id="07b27-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07b27-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07b27-105">Recupere os [objetos accessReviewInstanceDecisionItem](../resources/accessreviewinstance.md) para uma aprovação pendente [accessReviewInstance](../resources/accessreviewscheduledefinition.md) específica pelo usuário chamador.</span><span class="sxs-lookup"><span data-stu-id="07b27-105">Retrieve the [accessReviewInstanceDecisionItem](../resources/accessreviewinstance.md) objects for a specific [accessReviewInstance](../resources/accessreviewscheduledefinition.md) pending approval by the calling user.</span></span> <span data-ttu-id="07b27-106">Uma lista de zero ou mais objetos accessReviewInstanceDecisionItem é retornada, incluindo todas as suas propriedades aninhadas.</span><span class="sxs-lookup"><span data-stu-id="07b27-106">A list of zero or more accessReviewInstanceDecisionItem objects are returned, including all of their nested properties.</span></span>

>[!NOTE]
><span data-ttu-id="07b27-107">Se muitos **accessReviewInstanceDecisionItems são retornados,** para melhorar a eficiência e evitar tempos-de-tempo, recupere o conjunto de resultados definido em páginas, incluindo o parâmetro de consulta $top com um tamanho de página de no máximo 100 e o parâmetro de consulta $skip=0 na solicitação.</span><span class="sxs-lookup"><span data-stu-id="07b27-107">If many **accessReviewInstanceDecisionItems** are returned, to improve efficiency and avoid timeouts, retrieve the result set in pages, by including both the $top query parameter with a page size of at most 100, and the $skip=0 query parameter in the request.</span></span> <span data-ttu-id="07b27-108">Quando um conjunto de resultados abrange várias páginas, o Microsoft Graph retorna essa página com uma propriedade @odata.nextLink na resposta que contém uma URL para a próxima página de resultados.</span><span class="sxs-lookup"><span data-stu-id="07b27-108">When a result set spans multiple pages, Microsoft Graph returns that page with an @odata.nextLink property in the response that contains a URL to the next page of results.</span></span> <span data-ttu-id="07b27-109">Se essa propriedade estiver presente, continue fazendo solicitações adicionais com a URL @odata.nextLink em cada resposta, até que todos os resultados sejam retornados, conforme descrito na pa paja do Microsoft Graph dados em seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="07b27-109">If that property is present, continue making additional requests with the @odata.nextLink URL in each response, until all the results are returned, as described in paging Microsoft Graph data in your app.</span></span>
>
><span data-ttu-id="07b27-110">Se nenhum parâmetro de consulta for fornecido e houver mais de 100 resultados, o Microsoft Graph paginará automaticamente os resultados em 100 resultados por página.</span><span class="sxs-lookup"><span data-stu-id="07b27-110">If no query parameters are provided and there are more than 100 results, Microsoft Graph will automatically paginate results at 100 results per page.</span></span>

## <a name="permissions"></a><span data-ttu-id="07b27-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="07b27-111">Permissions</span></span>
<span data-ttu-id="07b27-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07b27-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07b27-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="07b27-114">Permission type</span></span>                        | <span data-ttu-id="07b27-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="07b27-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="07b27-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="07b27-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="07b27-117">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07b27-117">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="07b27-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="07b27-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07b27-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07b27-119">Not supported.</span></span>|

<span data-ttu-id="07b27-120">O usuário interno também verá apenas as decisões das quais o revisor é atribuído no accessReviewScheduleDefinition da instância dessa decisão.</span><span class="sxs-lookup"><span data-stu-id="07b27-120">The signed-in user will also only see decisions of which they are assigned reviewer in that decision's instance's accessReviewScheduleDefinition.</span></span>

## <a name="http-request"></a><span data-ttu-id="07b27-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="07b27-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/pendingAccessReviewInstances/{instance-id}/decisions
```
## <a name="request-headers"></a><span data-ttu-id="07b27-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="07b27-122">Request headers</span></span>
<span data-ttu-id="07b27-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="07b27-123">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="07b27-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="07b27-124">Request body</span></span>
<span data-ttu-id="07b27-125">Não fornecer um corpo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="07b27-125">Do not supply a request body.</span></span>

## <a name="response"></a><span data-ttu-id="07b27-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="07b27-126">Response</span></span>
<span data-ttu-id="07b27-127">Se tiver êxito, este método retornará um código de resposta e uma matriz de `200 OK` [objetos accessReviewInstanceDecisionItem](../resources/accessreviewinstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="07b27-127">If successful, this method returns a `200 OK` response code and an array of [accessReviewInstanceDecisionItem](../resources/accessreviewinstance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="07b27-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="07b27-128">Examples</span></span>
### <a name="request"></a><span data-ttu-id="07b27-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="07b27-129">Request</span></span>
<span data-ttu-id="07b27-130">O exemplo a seguir mostra uma solicitação para recuperar todas as decisões em uma instância de uma revisão de acesso aguardando a aprovação do usuário chamador.</span><span class="sxs-lookup"><span data-stu-id="07b27-130">The following example shows a request to retrieve all the decisions on an instance of an access review pending the calling user's approval.</span></span>


# <a name="http"></a>[<span data-ttu-id="07b27-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="07b27-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessReviewInstanceDecisionItem_pendingapproval"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/pendingAccessReviewInstances/70a68410-67f3-4d4c-b946-6989e050be19/decisions?$top=100&$skip=0
```
# <a name="c"></a>[<span data-ttu-id="07b27-132">C#</span><span class="sxs-lookup"><span data-stu-id="07b27-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewinstancedecisionitem-pendingapproval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="07b27-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="07b27-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewinstancedecisionitem-pendingapproval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="07b27-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="07b27-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewinstancedecisionitem-pendingapproval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="07b27-135">Java</span><span class="sxs-lookup"><span data-stu-id="07b27-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewinstancedecisionitem-pendingapproval-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a><span data-ttu-id="07b27-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="07b27-136">Response</span></span>
><span data-ttu-id="07b27-137">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="07b27-137">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.count": 2,
    "value": [
        {
            "id": "654b34e7-b48f-4772-a2d4-08f1d0dd014c",
            "accessReviewId": "70a68410-67f3-4d4c-b946-6989e050be19",
            "reviewedDateTime": null,
            "decision": "NotReviewed",
            "justification": "",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Approve",
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
                "userId": "7eae986b-d425-48b2-adf2-3c777f6256f3",
                "userDisplayName": "Adele Vance",
                "userPrincipalName": "AdeleV@contoso.com"
            }
        },
        {
            "id": "0311dba4-c60c-412e-ac77-14e1da23daf1",
            "accessReviewId": "70a68410-67f3-4d4c-b946-6989e050be19",
            "reviewedDateTime": null,
            "decision": "NotReviewed",
            "justification": "",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Approve",
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
                "userId": "957f1027-c0ee-460d-9269-b8828e59e0fe",
                "userDisplayName": "MOD Administrator",
                "userPrincipalName": "admin@contoso.com"
            }
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="07b27-138">Confira também</span><span class="sxs-lookup"><span data-stu-id="07b27-138">See also</span></span>

- [<span data-ttu-id="07b27-139">Obter accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="07b27-139">Get accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-get.md)
- [<span data-ttu-id="07b27-140">Obter accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="07b27-140">Get accessReviewInstance</span></span>](accessreviewinstance-get.md)


<!--
{
  "type": "#page.annotation",
  "description": "List accessReviewInstanceDecisionItem pendingApproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
