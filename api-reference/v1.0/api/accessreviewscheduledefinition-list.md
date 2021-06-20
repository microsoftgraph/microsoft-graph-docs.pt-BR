---
title: Listar accessReviewScheduleDefinitions
description: Obter uma lista dos objetos accessReviewScheduleDefinition e suas propriedades.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: dd60a89a7aeb43c4817fa9b67bcf3886425f166a
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030988"
---
# <a name="list-accessreviewscheduledefinitions"></a><span data-ttu-id="dddcd-103">Listar accessReviewScheduleDefinitions</span><span class="sxs-lookup"><span data-stu-id="dddcd-103">List accessReviewScheduleDefinitions</span></span>
<span data-ttu-id="dddcd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dddcd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dddcd-105">Obter uma lista dos [objetos accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="dddcd-105">Get a list of the [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) objects and their properties.</span></span>

>[!NOTE]
><span data-ttu-id="dddcd-106">O tamanho padrão da página para essa API é de 100 objetos accessReviewScheduleDefinition.</span><span class="sxs-lookup"><span data-stu-id="dddcd-106">The default page size for this API is 100 accessReviewScheduleDefinition objects.</span></span> <span data-ttu-id="dddcd-107">Para melhorar a eficiência e evitar tempos-de-tempo devido a grandes conjuntos de resultados, aplique paginação usando os `$skip` parâmetros e `$top` de consulta.</span><span class="sxs-lookup"><span data-stu-id="dddcd-107">To improve efficiency and avoid timeouts due to large result sets, apply pagination using the `$skip` and `$top` query parameters.</span></span> <span data-ttu-id="dddcd-108">Para mais informações, consulte [Paginação de dados do Microsoft Graph em seu aplicativo](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="dddcd-108">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="dddcd-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="dddcd-109">Permissions</span></span>
<span data-ttu-id="dddcd-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dddcd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dddcd-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dddcd-112">Permission type</span></span>|<span data-ttu-id="dddcd-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dddcd-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dddcd-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dddcd-114">Delegated (work or school account)</span></span>|<span data-ttu-id="dddcd-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dddcd-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="dddcd-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dddcd-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dddcd-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dddcd-117">Not supported.</span></span>|
|<span data-ttu-id="dddcd-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dddcd-118">Application</span></span>|<span data-ttu-id="dddcd-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dddcd-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|

 <span data-ttu-id="dddcd-120">O usuário interno também deve estar em uma função de diretório que permita que ele leia uma revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="dddcd-120">The signed-in user must also be in a directory role that permits them to read an access review.</span></span> <span data-ttu-id="dddcd-121">Consulte access review [role and application permission authorization checks](../resources/accessreviewsv2-root.md#role-and-application-permission-authorization-checks).</span><span class="sxs-lookup"><span data-stu-id="dddcd-121">See access review [role and application permission authorization checks](../resources/accessreviewsv2-root.md#role-and-application-permission-authorization-checks).</span></span>

## <a name="http-request"></a><span data-ttu-id="dddcd-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dddcd-122">HTTP request</span></span>

<span data-ttu-id="dddcd-123">Para listar todos os seus accessReviewScheduleDefinitions:</span><span class="sxs-lookup"><span data-stu-id="dddcd-123">To list all your accessReviewScheduleDefinitions:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/accessReviews/definitions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dddcd-124">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="dddcd-124">Optional query parameters</span></span>
<span data-ttu-id="dddcd-125">Este método dá suporte aos parâmetros de consulta , , , e OData para `$select` ajudar a personalizar a `$top` `$skip` `$orderBy` `$filter` resposta.</span><span class="sxs-lookup"><span data-stu-id="dddcd-125">This method supports the `$select`, `$top`, `$skip`,`$orderBy`, and `$filter` OData query parameters to help customize the response.</span></span> <span data-ttu-id="dddcd-126">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="dddcd-126">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="use-the-filter-query-parameter"></a><span data-ttu-id="dddcd-127">Usar o parâmetro $filter de consulta</span><span class="sxs-lookup"><span data-stu-id="dddcd-127">Use the $filter query parameter</span></span>
<span data-ttu-id="dddcd-128">O parâmetro de consulta com o operador é suportado na propriedade `$filter` `contains` **scope** accessReviewScheduleDefinition.</span><span class="sxs-lookup"><span data-stu-id="dddcd-128">The `$filter` query parameter with the `contains` operator is supported on the **scope** property of accessReviewScheduleDefinition.</span></span> <span data-ttu-id="dddcd-129">Use o seguinte formato para a solicitação:</span><span class="sxs-lookup"><span data-stu-id="dddcd-129">Use the following format for the request:</span></span>

```http
GET /identityGovernance/accessReviews/definitions?$filter=contains(scope/microsoft.graph.accessReviewQueryScope/query, '{object}')
```

<span data-ttu-id="dddcd-130">O valor de `{object}` pode ser um dos seguintes:</span><span class="sxs-lookup"><span data-stu-id="dddcd-130">The value of `{object}` can be one of the following:</span></span>

|<span data-ttu-id="dddcd-131">Valor</span><span class="sxs-lookup"><span data-stu-id="dddcd-131">Value</span></span>|<span data-ttu-id="dddcd-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="dddcd-132">Description</span></span>|
|:---     |:---       |
|`/groups`  |<span data-ttu-id="dddcd-133">Listar todos os accessReviewScheduleDefinition em grupos individuais (exclui definições com escopo para todos os grupos Microsoft 365 com usuários convidados).</span><span class="sxs-lookup"><span data-stu-id="dddcd-133">List every accessReviewScheduleDefinition on individual groups (excludes definitions scoped to all Microsoft 365 groups with guest users).</span></span>|
|`/groups/{group id}`  |<span data-ttu-id="dddcd-134">Listar todos os accessReviewScheduleDefinition em um grupo específico (exclui definições com escopo para todos os grupos Microsoft 365 com usuários convidados).</span><span class="sxs-lookup"><span data-stu-id="dddcd-134">List every accessReviewScheduleDefinition on a specific group (excludes definitions scoped to all Microsoft 365 groups with guest users).</span></span>|
|`./members`  |<span data-ttu-id="dddcd-135">Listar todos os accessReviewScheduleDefinition com escopo para todos os grupos Microsoft 365 com usuários convidados.</span><span class="sxs-lookup"><span data-stu-id="dddcd-135">List every accessReviewScheduleDefinition scoped to all Microsoft 365 groups with guest users.</span></span>|
|`accessPackageAssignments`  |<span data-ttu-id="dddcd-136">Listar todos os accessReviewScheduleDefinition em um pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="dddcd-136">List every accessReviewScheduleDefinition on an access package.</span></span>|
|`roleAssignmentScheduleInstances`  |<span data-ttu-id="dddcd-137">Listar todos os accessReviewScheduleDefinition para entidades de serviço atribuídas a uma função privilegiada.</span><span class="sxs-lookup"><span data-stu-id="dddcd-137">List every accessReviewScheduleDefinition for service principals assigned to a privileged role.</span></span>|

<span data-ttu-id="dddcd-138">O parâmetro de consulta não é suportado `$filter` em **accessReviewInactiveUserQueryScope** ou **principalResourceMembershipScope**.</span><span class="sxs-lookup"><span data-stu-id="dddcd-138">The `$filter` query parameter is not supported on **accessReviewInactiveUserQueryScope** or **principalResourceMembershipScope**.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dddcd-139">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dddcd-139">Request headers</span></span>
|<span data-ttu-id="dddcd-140">Nome</span><span class="sxs-lookup"><span data-stu-id="dddcd-140">Name</span></span>|<span data-ttu-id="dddcd-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="dddcd-141">Description</span></span>|
|:---|:---|
|<span data-ttu-id="dddcd-142">Autorização</span><span class="sxs-lookup"><span data-stu-id="dddcd-142">Authorization</span></span>|<span data-ttu-id="dddcd-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dddcd-p106">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dddcd-145">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dddcd-145">Request body</span></span>
<span data-ttu-id="dddcd-146">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dddcd-146">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dddcd-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="dddcd-147">Response</span></span>

<span data-ttu-id="dddcd-148">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dddcd-148">If successful, this method returns a `200 OK` response code and a collection of [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dddcd-149">Exemplos</span><span class="sxs-lookup"><span data-stu-id="dddcd-149">Examples</span></span>

### <a name="example-1-list-the-first-one-hundred-access-review-definitions"></a><span data-ttu-id="dddcd-150">Exemplo 1: listar as primeiras 100 definições de revisão de acesso</span><span class="sxs-lookup"><span data-stu-id="dddcd-150">Example 1: List the first one hundred access review definitions</span></span>

#### <a name="request"></a><span data-ttu-id="dddcd-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dddcd-151">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_accessReviewScheduleDefinition"
}-->
```
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions?$top=100&$skip=0
```

#### <a name="response"></a><span data-ttu-id="dddcd-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="dddcd-152">Response</span></span>
><span data-ttu-id="dddcd-153">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="dddcd-153">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/accessReviews/definitions",
    "@odata.count": 1,
    "value": [
        {
            "id": "98dcebed-c7f6-46f4-bcf3-4a3fccdb3e2a",
            "displayName": "Access Review",
            "scope": {
                "query": "/groups/119cc181-22f0-4e18-8537-264e7524ee0b/transitiveMembers",
                "queryType": "MicrosoftGraph"
            },
            "instanceEnumerationScope": {
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

### <a name="example-2-retrieve-all-access-review-definitions-scoped-to-all-microsoft-365-groups-in-a-tenant"></a><span data-ttu-id="dddcd-154">Exemplo 2: Recuperar todas as definições de revisão de acesso com escopo para todos os grupos Microsoft 365 em um locatário</span><span class="sxs-lookup"><span data-stu-id="dddcd-154">Example 2: Retrieve all access review definitions scoped to all Microsoft 365 groups in a tenant</span></span>

#### <a name="request"></a><span data-ttu-id="dddcd-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dddcd-155">Request</span></span>
<span data-ttu-id="dddcd-156">O exemplo a seguir mostra uma solicitação para recuperar todas as séries de revisão de acesso com escopo para todos os grupos Microsoft 365 em um locatário.</span><span class="sxs-lookup"><span data-stu-id="dddcd-156">The following example shows a request to retrieve all the access review series scoped to all Microsoft 365 groups in a tenant.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_accessReviewScheduleDefinition_allgroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions?$filter=contains(scope/microsoft.graph.accessReviewQueryScope/query, './members')
```

#### <a name="response"></a><span data-ttu-id="dddcd-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="dddcd-157">Response</span></span>
><span data-ttu-id="dddcd-158">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="dddcd-158">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/accessReviews/definitions",
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
            "instances@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/accessReviews/definitions('cc701697-762c-439a-81f5-f58d680fde76')/instances",
            "instances": []
        }
    ]
}

```
