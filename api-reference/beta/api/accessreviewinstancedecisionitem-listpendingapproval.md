---
title: Listar a aprovação pendente accessReviewInstanceDecisionItem
description: Recupere os objetos accessReviewInstanceDecisionItem aguardando aprovação do usuário chamador.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: d1ce0293510f2f9a6ca526216b3fc2ad024b6285
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030471"
---
# <a name="list-accessreviewinstancedecisionitems-pending-approval-deprecated"></a><span data-ttu-id="a8a73-103">Listar accessReviewInstanceDecisionItems pendente aprovação (preterida)</span><span class="sxs-lookup"><span data-stu-id="a8a73-103">List accessReviewInstanceDecisionItems pending approval (deprecated)</span></span>

<span data-ttu-id="a8a73-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8a73-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
><span data-ttu-id="a8a73-105">Esse método será preterido e interromperá o retorno de dados em 19 de maio de 2023.</span><span class="sxs-lookup"><span data-stu-id="a8a73-105">This method will be deprecated and will stop returning data on May 19, 2023.</span></span> <span data-ttu-id="a8a73-106">Ele foi substituído por [filterByCurrentUser](accessreviewinstancedecisionitem-filterbycurrentuser.md).</span><span class="sxs-lookup"><span data-stu-id="a8a73-106">It has been replaced by [filterByCurrentUser](accessreviewinstancedecisionitem-filterbycurrentuser.md).</span></span>

<span data-ttu-id="a8a73-107">Recupere os [objetos accessReviewInstanceDecisionItem](../resources/accessreviewinstance.md) para uma aprovação pendente [accessReviewInstance](../resources/accessreviewscheduledefinition.md) específica pelo usuário chamador.</span><span class="sxs-lookup"><span data-stu-id="a8a73-107">Retrieve the [accessReviewInstanceDecisionItem](../resources/accessreviewinstance.md) objects for a specific [accessReviewInstance](../resources/accessreviewscheduledefinition.md) pending approval by the calling user.</span></span> <span data-ttu-id="a8a73-108">Uma lista de zero ou mais objetos accessReviewInstanceDecisionItem é retornada, incluindo todas as suas propriedades aninhadas.</span><span class="sxs-lookup"><span data-stu-id="a8a73-108">A list of zero or more accessReviewInstanceDecisionItem objects are returned, including all of their nested properties.</span></span>

>[!NOTE]
><span data-ttu-id="a8a73-109">O tamanho padrão da página para essa API é de 100 objetos accessReviewInstanceDecisionItem.</span><span class="sxs-lookup"><span data-stu-id="a8a73-109">The default page size for this API is 100 accessReviewInstanceDecisionItem objects.</span></span> <span data-ttu-id="a8a73-110">Para melhorar a eficiência e evitar tempos-de-tempo devido a grandes conjuntos de resultados, aplique paginação usando os `$skip` parâmetros e `$top` de consulta.</span><span class="sxs-lookup"><span data-stu-id="a8a73-110">To improve efficiency and avoid timeouts due to large result sets, apply pagination using the `$skip` and `$top` query parameters.</span></span> <span data-ttu-id="a8a73-111">Para mais informações, consulte [Paginação de dados do Microsoft Graph em seu aplicativo](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="a8a73-111">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="a8a73-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="a8a73-112">Permissions</span></span>
<span data-ttu-id="a8a73-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8a73-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8a73-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a8a73-115">Permission type</span></span>                        | <span data-ttu-id="a8a73-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a8a73-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a8a73-117">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a8a73-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="a8a73-118">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8a73-118">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="a8a73-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a8a73-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8a73-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a8a73-120">Not supported.</span></span>|

<span data-ttu-id="a8a73-121">O usuário interno também verá apenas as decisões das quais o revisor é atribuído no accessReviewScheduleDefinition da instância dessa decisão.</span><span class="sxs-lookup"><span data-stu-id="a8a73-121">The signed-in user will also only see decisions of which they are assigned reviewer in that decision's instance's accessReviewScheduleDefinition.</span></span>

## <a name="http-request"></a><span data-ttu-id="a8a73-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a8a73-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/pendingAccessReviewInstances/{instance-id}/decisions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a8a73-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a8a73-123">Optional query parameters</span></span>
<span data-ttu-id="a8a73-124">Este método oferece `$skip` suporte e `$top` parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a8a73-124">This method supports `$skip` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="a8a73-125">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a8a73-125">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a8a73-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a8a73-126">Request headers</span></span>
<span data-ttu-id="a8a73-127">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a8a73-127">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="a8a73-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a8a73-128">Request body</span></span>
<span data-ttu-id="a8a73-129">Não fornecer um corpo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a8a73-129">Do not supply a request body.</span></span>

## <a name="response"></a><span data-ttu-id="a8a73-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8a73-130">Response</span></span>
<span data-ttu-id="a8a73-131">Se tiver êxito, este método retornará um código de resposta e uma matriz de `200 OK` [objetos accessReviewInstanceDecisionItem](../resources/accessreviewinstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a8a73-131">If successful, this method returns a `200 OK` response code and an array of [accessReviewInstanceDecisionItem](../resources/accessreviewinstance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a8a73-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a8a73-132">Examples</span></span>
### <a name="request"></a><span data-ttu-id="a8a73-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a8a73-133">Request</span></span>
<span data-ttu-id="a8a73-134">O exemplo a seguir mostra uma solicitação para recuperar todas as decisões em uma instância de uma revisão de acesso aguardando a aprovação do usuário chamador.</span><span class="sxs-lookup"><span data-stu-id="a8a73-134">The following example shows a request to retrieve all the decisions on an instance of an access review pending the calling user's approval.</span></span>


# <a name="http"></a>[<span data-ttu-id="a8a73-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="a8a73-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessReviewInstanceDecisionItem_pendingapproval"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/pendingAccessReviewInstances/70a68410-67f3-4d4c-b946-6989e050be19/decisions?$top=100&$skip=0
```
# <a name="c"></a>[<span data-ttu-id="a8a73-136">C#</span><span class="sxs-lookup"><span data-stu-id="a8a73-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewinstancedecisionitem-pendingapproval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a8a73-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a8a73-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewinstancedecisionitem-pendingapproval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a8a73-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a8a73-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewinstancedecisionitem-pendingapproval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a8a73-139">Java</span><span class="sxs-lookup"><span data-stu-id="a8a73-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewinstancedecisionitem-pendingapproval-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a><span data-ttu-id="a8a73-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8a73-140">Response</span></span>
><span data-ttu-id="a8a73-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a8a73-141">**Note:** The response object shown here might be shortened for readability.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="a8a73-142">Confira também</span><span class="sxs-lookup"><span data-stu-id="a8a73-142">See also</span></span>

- [<span data-ttu-id="a8a73-143">Obter accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="a8a73-143">Get accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-get.md)
- [<span data-ttu-id="a8a73-144">Obter accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="a8a73-144">Get accessReviewInstance</span></span>](accessreviewinstance-get.md)


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
