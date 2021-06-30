---
title: 'accessReviewScheduleDefinition: filterByCurrentUser'
description: Retorna os objetos accessReviewScheduleDefinition onde o usuário de chamada é o revisor.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: b30bb5464e0373f65c3f200aa33936d08d94ad56
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207389"
---
# <a name="accessreviewscheduledefinition-filterbycurrentuser"></a><span data-ttu-id="b327f-103">accessReviewScheduleDefinition: filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="b327f-103">accessReviewScheduleDefinition: filterByCurrentUser</span></span>
<span data-ttu-id="b327f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b327f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b327f-105">Retorna [os objetos accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) onde o usuário de chamada é um revisor em um ou mais [objetos accessReviewInstance.](../resources/accessreviewinstance.md)</span><span class="sxs-lookup"><span data-stu-id="b327f-105">Returns [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) objects where the calling user is a reviewer on one or more [accessReviewInstance](../resources/accessreviewinstance.md) objects.</span></span>

>[!NOTE]
><span data-ttu-id="b327f-106">O tamanho padrão da página para essa API é de 100 objetos accessReviewScheduleDefinition.</span><span class="sxs-lookup"><span data-stu-id="b327f-106">The default page size for this API is 100 accessReviewScheduleDefinition objects.</span></span> <span data-ttu-id="b327f-107">Para melhorar a eficiência e evitar tempos-de-tempo devido a grandes conjuntos de resultados, aplique paginação usando os `$skip` parâmetros e `$top` de consulta.</span><span class="sxs-lookup"><span data-stu-id="b327f-107">To improve efficiency and avoid timeouts due to large result sets, apply pagination using the `$skip` and `$top` query parameters.</span></span> <span data-ttu-id="b327f-108">Para mais informações, consulte [Paginação de dados do Microsoft Graph em seu aplicativo](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="b327f-108">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="permissions"></a><span data-ttu-id="b327f-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="b327f-109">Permissions</span></span>
<span data-ttu-id="b327f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b327f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b327f-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b327f-112">Permission type</span></span>|<span data-ttu-id="b327f-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b327f-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b327f-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b327f-114">Delegated (work or school account)</span></span>|<span data-ttu-id="b327f-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b327f-115">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="b327f-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b327f-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b327f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b327f-117">Not supported.</span></span>|
|<span data-ttu-id="b327f-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b327f-118">Application</span></span>|<span data-ttu-id="b327f-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b327f-119">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b327f-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b327f-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/filterByCurrentUser(on='reviewer')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b327f-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b327f-121">Optional query parameters</span></span>
<span data-ttu-id="b327f-122">Este método dá suporte a parâmetros de consulta `$select` , , , e `$filter` `$orderBy` `$skip` `$top` OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b327f-122">This method supports `$select`, `$filter`, `$orderBy`, `$skip`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="b327f-123">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b327f-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b327f-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b327f-124">Request headers</span></span>
|<span data-ttu-id="b327f-125">Nome</span><span class="sxs-lookup"><span data-stu-id="b327f-125">Name</span></span>|<span data-ttu-id="b327f-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="b327f-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b327f-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="b327f-127">Authorization</span></span>|<span data-ttu-id="b327f-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b327f-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b327f-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b327f-130">Request body</span></span>
<span data-ttu-id="b327f-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b327f-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b327f-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="b327f-132">Response</span></span>

<span data-ttu-id="b327f-133">Se tiver êxito, essa função retornará um código de resposta e uma `200 OK` [coleção accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b327f-133">If successful, this function returns a `200 OK` response code and a [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b327f-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b327f-134">Examples</span></span>
<span data-ttu-id="b327f-135">Retorna todas as definições de revisão em que o usuário de chamada é um revistor.</span><span class="sxs-lookup"><span data-stu-id="b327f-135">Returns all review definitions where the calling user is a reviewer.</span></span>

### <a name="request"></a><span data-ttu-id="b327f-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b327f-136">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b327f-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="b327f-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accessreviewscheduledefinition_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/filterByCurrentUser(on='reviewer')
```
# <a name="c"></a>[<span data-ttu-id="b327f-138">C#</span><span class="sxs-lookup"><span data-stu-id="b327f-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accessreviewscheduledefinition-filterbycurrentuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b327f-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b327f-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accessreviewscheduledefinition-filterbycurrentuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b327f-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b327f-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accessreviewscheduledefinition-filterbycurrentuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b327f-141">Java</span><span class="sxs-lookup"><span data-stu-id="b327f-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accessreviewscheduledefinition-filterbycurrentuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="b327f-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="b327f-142">Response</span></span>
><span data-ttu-id="b327f-143">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b327f-143">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessReviewScheduleDefinition)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(accessReviewScheduleDefinition)",
    "@odata.count": 1,
    "value": [
        {
            "@odata.type": "#microsoft.graph.accessReviewScheduleDefinition",
            "id": "ad0ec492-c1b6-49f0-9025-ea15ca471ea9",
            "displayName": "Test",
            "createdDateTime": "2021-04-29T20:01:18.1084432Z",
            "lastModifiedDateTime": "2021-04-29T20:01:52.3233462Z",
            "status": "Completed",
            "descriptionForAdmins": "Test",
            "descriptionForReviewers": "Test",
            "createdBy": {
                "id": "36c4c56e-fce3-4e2d-b28e-4ac0c7d2fa10",
                "displayName": "MOD Administrator",
                "userPrincipalName": "admin@contoso.com"
            },
            "scope": {
                "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
                "query": "./members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
                "queryType": "MicrosoftGraph",
                "queryRoot": null,
                "inactiveDuration": "P30D"
            },
            "instanceEnumerationScope": {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/v1.0/groups?$filter=(groupTypes/any(c:c+eq+'Unified'))&$count=true",
                "queryType": "MicrosoftGraph",
                "queryRoot": null
            },
            "reviewers": [
                {
                    "query": "./owners",
                    "queryType": "MicrosoftGraph",
                    "queryRoot": null
                }
            ],
            "backupReviewers": [],
            "fallbackReviewers": [],
            "settings": {
                "mailNotificationsEnabled": true,
                "reminderNotificationsEnabled": true,
                "justificationRequiredOnApproval": true,
                "defaultDecisionEnabled": true,
                "defaultDecision": "Approve",
                "instanceDurationInDays": 3,
                "autoApplyDecisionsEnabled": true,
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
                        "startDate": "2021-04-30",
                        "endDate": "2021-04-30"
                    }
                },
                "applyActions": [
                    {
                        "@odata.type": "#microsoft.graph.removeAccessApplyAction"
                    }
                ]
            },
            "instances": []
        }
    ]
}
```
