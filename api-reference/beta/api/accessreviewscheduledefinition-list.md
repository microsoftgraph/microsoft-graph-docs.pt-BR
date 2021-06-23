---
title: Listar accessReviewScheduleDefinitions
description: Recupere objetos accessReviewScheduleDefinition.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: a2d29f6e1f3aa848b60351ed4972ab5b4f06cfd2
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/22/2021
ms.locfileid: "53059991"
---
# <a name="list-accessreviewscheduledefinition"></a><span data-ttu-id="7a07f-103">Listar accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="7a07f-103">List accessReviewScheduleDefinition</span></span>

<span data-ttu-id="7a07f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a07f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a07f-105">Recupere os [objetos accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7a07f-105">Retrieve the [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) objects.</span></span> <span data-ttu-id="7a07f-106">Uma lista de zero ou mais objetos accessReviewScheduleDefinition são retornados, incluindo todas as suas propriedades aninhadas, para cada série de revisão de acesso criada.</span><span class="sxs-lookup"><span data-stu-id="7a07f-106">A list of zero or more accessReviewScheduleDefinition objects are returned, including all of their nested properties, for each access review series created.</span></span> <span data-ttu-id="7a07f-107">Isso não inclui os objetos accessReviewInstance associados.</span><span class="sxs-lookup"><span data-stu-id="7a07f-107">This does not include the associated accessReviewInstance objects.</span></span>

>[!NOTE]
><span data-ttu-id="7a07f-108">O tamanho padrão da página para essa API é de 100 objetos accessReviewScheduleDefinition.</span><span class="sxs-lookup"><span data-stu-id="7a07f-108">The default page size for this API is 100 accessReviewScheduleDefinition objects.</span></span> <span data-ttu-id="7a07f-109">Para melhorar a eficiência e evitar tempos-de-tempo devido a grandes conjuntos de resultados, aplique paginação usando os `$skip` parâmetros e `$top` de consulta.</span><span class="sxs-lookup"><span data-stu-id="7a07f-109">To improve efficiency and avoid timeouts due to large result sets, apply pagination using the `$skip` and `$top` query parameters.</span></span> <span data-ttu-id="7a07f-110">Para mais informações, consulte [Paginação de dados do Microsoft Graph em seu aplicativo](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="7a07f-110">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="7a07f-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="7a07f-111">Permissions</span></span>
<span data-ttu-id="7a07f-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a07f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a07f-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7a07f-114">Permission type</span></span>                        | <span data-ttu-id="7a07f-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7a07f-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="7a07f-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7a07f-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="7a07f-117">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a07f-117">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="7a07f-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7a07f-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a07f-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7a07f-119">Not supported.</span></span>|
|<span data-ttu-id="7a07f-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7a07f-120">Application</span></span>                            | <span data-ttu-id="7a07f-121">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a07f-121">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span> |

 <span data-ttu-id="7a07f-122">O usuário interno também deve estar em uma função de diretório que permita que ele leia uma revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="7a07f-122">The signed-in user must also be in a directory role that permits them to read an access review.</span></span> <span data-ttu-id="7a07f-123">Consulte access review [role and application permission authorization checks](../resources/accessreviewsv2-root.md#role-and-application-permission-authorization-checks).</span><span class="sxs-lookup"><span data-stu-id="7a07f-123">See access review [role and application permission authorization checks](../resources/accessreviewsv2-root.md#role-and-application-permission-authorization-checks).</span></span>

## <a name="http-request"></a><span data-ttu-id="7a07f-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7a07f-124">HTTP request</span></span>

<span data-ttu-id="7a07f-125">Para listar todos os seus accessReviewScheduleDefinitions:</span><span class="sxs-lookup"><span data-stu-id="7a07f-125">To list all your accessReviewScheduleDefinitions:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/accessReviews/definitions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7a07f-126">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7a07f-126">Optional query parameters</span></span>
<span data-ttu-id="7a07f-127">Este método dá suporte `$select` aos `$top` parâmetros de consulta , , e OData para ajudar a `$skip` personalizar a `$filter` resposta.</span><span class="sxs-lookup"><span data-stu-id="7a07f-127">This method supports the `$select`, `$top`, `$skip`, and `$filter` OData query parameters to help customize the response.</span></span> <span data-ttu-id="7a07f-128">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="7a07f-128">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="use-the-filter-query-parameter"></a><span data-ttu-id="7a07f-129">Usar o parâmetro $filter de consulta</span><span class="sxs-lookup"><span data-stu-id="7a07f-129">Use the $filter query parameter</span></span>
<span data-ttu-id="7a07f-130">O parâmetro de consulta com o operador é suportado na propriedade `$filter` `contains` **scope** accessReviewScheduleDefinition.</span><span class="sxs-lookup"><span data-stu-id="7a07f-130">The `$filter` query parameter with the `contains` operator is supported on the **scope** property of accessReviewScheduleDefinition.</span></span> <span data-ttu-id="7a07f-131">Use o seguinte formato para a solicitação:</span><span class="sxs-lookup"><span data-stu-id="7a07f-131">Use the following format for the request:</span></span>

```http
GET /identityGovernance/accessReviews/definitions?$filter=contains(scope/microsoft.graph.accessReviewQueryScope/query, '{object}')
```

<span data-ttu-id="7a07f-132">O valor de `{object}` pode ser um dos seguintes:</span><span class="sxs-lookup"><span data-stu-id="7a07f-132">The value of `{object}` can be one of the following:</span></span>

|<span data-ttu-id="7a07f-133">Valor</span><span class="sxs-lookup"><span data-stu-id="7a07f-133">Value</span></span>|<span data-ttu-id="7a07f-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a07f-134">Description</span></span>|
|:---     |:---       |
|<span data-ttu-id="7a07f-135">/groups</span><span class="sxs-lookup"><span data-stu-id="7a07f-135">/groups</span></span>  |<span data-ttu-id="7a07f-136">Listar todos os accessReviewScheduleDefinition em grupos individuais (exclui definições com escopo para todos os grupos Microsoft 365 com usuários convidados).</span><span class="sxs-lookup"><span data-stu-id="7a07f-136">List every accessReviewScheduleDefinition on individual groups (excludes definitions scoped to all Microsoft 365 groups with guest users).</span></span>|
|<span data-ttu-id="7a07f-137">/groups/{group id}</span><span class="sxs-lookup"><span data-stu-id="7a07f-137">/groups/{group id}</span></span>  |<span data-ttu-id="7a07f-138">Listar todos os accessReviewScheduleDefinition em um grupo específico (exclui definições com escopo para todos os grupos Microsoft 365 com usuários convidados).</span><span class="sxs-lookup"><span data-stu-id="7a07f-138">List every accessReviewScheduleDefinition on a specific group (excludes definitions scoped to all Microsoft 365 groups with guest users).</span></span>|
|<span data-ttu-id="7a07f-139">./members</span><span class="sxs-lookup"><span data-stu-id="7a07f-139">./members</span></span>  |<span data-ttu-id="7a07f-140">Listar todos os accessReviewScheduleDefinition com escopo para todos os grupos Microsoft 365 com usuários convidados.</span><span class="sxs-lookup"><span data-stu-id="7a07f-140">List every accessReviewScheduleDefinition scoped to all Microsoft 365 groups with guest users.</span></span>|
|<span data-ttu-id="7a07f-141">accessPackageAssignments</span><span class="sxs-lookup"><span data-stu-id="7a07f-141">accessPackageAssignments</span></span>  |<span data-ttu-id="7a07f-142">Listar todos os accessReviewScheduleDefinition em um pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="7a07f-142">List every accessReviewScheduleDefinition on an access package.</span></span>|
|<span data-ttu-id="7a07f-143">roleAssignmentScheduleInstances</span><span class="sxs-lookup"><span data-stu-id="7a07f-143">roleAssignmentScheduleInstances</span></span>  |<span data-ttu-id="7a07f-144">Listar todos os accessReviewScheduleDefinition para entidades de serviço atribuídas a uma função privilegiada.</span><span class="sxs-lookup"><span data-stu-id="7a07f-144">List every accessReviewScheduleDefinition for service principals assigned to a privileged role.</span></span>|

<span data-ttu-id="7a07f-145">O parâmetro de consulta não é suportado `$filter` em **accessReviewInactiveUserQueryScope** ou **principalResourceMembershipScope**.</span><span class="sxs-lookup"><span data-stu-id="7a07f-145">The `$filter` query parameter is not supported on **accessReviewInactiveUserQueryScope** or **principalResourceMembershipScope**.</span></span>


## <a name="request-headers"></a><span data-ttu-id="7a07f-146">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7a07f-146">Request headers</span></span>
<span data-ttu-id="7a07f-147">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7a07f-147">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="7a07f-148">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7a07f-148">Request body</span></span>
<span data-ttu-id="7a07f-149">Não fornecer um corpo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7a07f-149">Do not supply a request body.</span></span>

## <a name="response"></a><span data-ttu-id="7a07f-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a07f-150">Response</span></span>
<span data-ttu-id="7a07f-151">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` matriz [de objetos accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7a07f-151">If successful, this method returns a `200 OK` response code and an array of [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7a07f-152">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7a07f-152">Examples</span></span>

### <a name="example-1-list-the-first-one-hundred-access-review-definitions"></a><span data-ttu-id="7a07f-153">Exemplo 1: listar as primeiras 100 definições de revisão de acesso</span><span class="sxs-lookup"><span data-stu-id="7a07f-153">Example 1: List the first one hundred access review definitions</span></span>

#### <a name="request"></a><span data-ttu-id="7a07f-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7a07f-154">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7a07f-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="7a07f-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessReviewScheduleDefinition"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions?$top=100&$skip=0
```
# <a name="c"></a>[<span data-ttu-id="7a07f-156">C#</span><span class="sxs-lookup"><span data-stu-id="7a07f-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewscheduledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7a07f-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7a07f-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewscheduledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7a07f-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7a07f-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewscheduledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7a07f-159">Java</span><span class="sxs-lookup"><span data-stu-id="7a07f-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewscheduledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="7a07f-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a07f-160">Response</span></span>
><span data-ttu-id="7a07f-161">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7a07f-161">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewScheduleDefinition",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions",
    "@odata.count": 1,
    "value": [
        {
            "id": "98dcebed-c7f6-46f4-bcf3-4a3fccdb3e2a",
            "displayName": "Access Review",
            "scope": {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/groups/119cc181-22f0-4e18-8537-264e7524ee0b/transitiveMembers",
                "queryType": "MicrosoftGraph"
            },
            "instanceEnumerationScope": {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/groups/119cc181-22f0-4e18-8537-264e7524ee0b",
                "queryType": "MicrosoftGraph"
            },
            "reviewers": [
                {
                    "query": "./manager",
                    "queryType": "MicrosoftGraph",
                    "queryRoot": "decisions"
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
                    "pattern": {
                        "type": "weekly",
                        "interval": 1,
                        "month": 0,
                        "dayOfMonth": 0,
                        "daysOfWeek": [],
                        "firstDayOfWeek": "sunday",
                        "index": "first"
                    },
                    "range": {
                        "type": "numbered",
                        "numberOfOccurrences": 0,
                        "recurrenceTimeZone": null,
                        "startDate": "2020-09-11",
                        "endDate": "9999-12-31"
                    }
                }
            }
        }
    ]
}
```


### <a name="example-2-retrieve-all-access-review-definitions-scoped-to-all-microsoft-365-groups-in-a-tenant"></a><span data-ttu-id="7a07f-162">Exemplo 2: Recuperar todas as definições de revisão de acesso com escopo para todos os grupos Microsoft 365 em um locatário</span><span class="sxs-lookup"><span data-stu-id="7a07f-162">Example 2: Retrieve all access review definitions scoped to all Microsoft 365 groups in a tenant</span></span>

#### <a name="request"></a><span data-ttu-id="7a07f-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7a07f-163">Request</span></span>
<span data-ttu-id="7a07f-164">O exemplo a seguir mostra uma solicitação para recuperar todas as séries de revisão de acesso com escopo para todos os grupos Microsoft 365 em um locatário.</span><span class="sxs-lookup"><span data-stu-id="7a07f-164">The following example shows a request to retrieve all the access review series scoped to all Microsoft 365 groups in a tenant.</span></span>


# <a name="http"></a>[<span data-ttu-id="7a07f-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="7a07f-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessReviewScheduleDefinition_allgroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions?$filter=contains(scope/microsoft.graph.accessReviewQueryScope/query, './members')
```
# <a name="c"></a>[<span data-ttu-id="7a07f-166">C#</span><span class="sxs-lookup"><span data-stu-id="7a07f-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewscheduledefinition-allgroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7a07f-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7a07f-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewscheduledefinition-allgroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7a07f-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7a07f-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewscheduledefinition-allgroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7a07f-169">Java</span><span class="sxs-lookup"><span data-stu-id="7a07f-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewscheduledefinition-allgroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7a07f-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a07f-170">Response</span></span>
><span data-ttu-id="7a07f-171">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7a07f-171">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewScheduleDefinition",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions",
    "@odata.count": 1,
    "value": [
        {
            "id": "cc701697-762c-439a-81f5-f58d680fde76",
            "displayName": "Review guest access across Microsoft 365 groups",
            "status": "InProgress",
            "scope": {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "./members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
                "queryType": "MicrosoftGraph"
            },
            "instanceEnumerationScope": {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/groups?$filter=(groupTypes/any(c:c+eq+'Unified'))&$count=true",
                "queryType": "MicrosoftGraph"
            },
            "reviewers": [
                {
                    "query": "./manager",
                    "queryType": "MicrosoftGraph",
                    "queryRoot": "decisions"
                }
            ],
            "settings": {
                "mailNotificationsEnabled": true,
                "reminderNotificationsEnabled": true,
                "justificationRequiredOnApproval": true,
                "defaultDecisionEnabled": true,
                "defaultDecision": "Recommendation",
                "instanceDurationInDays": 25,
                "autoApplyDecisionsEnabled": true,
                "recommendationsEnabled": true,
                "recurrence": {
                    "pattern": {
                        "type": "absoluteMonthly",
                        "interval": 3,
                        "month": 0,
                        "dayOfMonth": 0,
                        "daysOfWeek": [],
                        "firstDayOfWeek": "sunday",
                        "index": "first"
                    },
                    "range": {
                        "type": "numbered",
                        "numberOfOccurrences": 0,
                        "recurrenceTimeZone": null,
                        "startDate": "2021-04-27",
                        "endDate": "9999-12-31"
                    }
                },
                "applyActions": [
                    {
                        "@odata.type": "#microsoft.graph.removeAccessApplyAction"
                    }
                ]
            },
            "instances@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions('cc701697-762c-439a-81f5-f58d680fde76')/instances",
            "instances": []
        }
    ]
}

```


## <a name="see-also"></a><span data-ttu-id="7a07f-172">Confira também</span><span class="sxs-lookup"><span data-stu-id="7a07f-172">See also</span></span>

- [<span data-ttu-id="7a07f-173">Obter accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="7a07f-173">Get accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition-get.md)


<!--
{
  "type": "#page.annotation",
  "description": "List accessReviewScheduleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
