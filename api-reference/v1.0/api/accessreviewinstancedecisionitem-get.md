---
title: Obter accessReviewInstanceDecisionItem
description: Leia as propriedades e as relações de um objeto accessReviewInstanceDecisionItem.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 2f72596f4f89fe71f6d7cee310e721dd230357ee
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209720"
---
# <a name="get-accessreviewinstancedecisionitem"></a><span data-ttu-id="8c7eb-103">Obter accessReviewInstanceDecisionItem</span><span class="sxs-lookup"><span data-stu-id="8c7eb-103">Get accessReviewInstanceDecisionItem</span></span>
<span data-ttu-id="8c7eb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c7eb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8c7eb-105">Leia as propriedades e as relações de um [objeto accessReviewInstanceDecisionItem.](../resources/accessreviewinstancedecisionitem.md)</span><span class="sxs-lookup"><span data-stu-id="8c7eb-105">Read the properties and relationships of an [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8c7eb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8c7eb-106">Permissions</span></span>
<span data-ttu-id="8c7eb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c7eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c7eb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8c7eb-109">Permission type</span></span>|<span data-ttu-id="8c7eb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8c7eb-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c7eb-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8c7eb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8c7eb-112">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c7eb-112">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="8c7eb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8c7eb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c7eb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8c7eb-114">Not supported.</span></span>|
|<span data-ttu-id="8c7eb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8c7eb-115">Application</span></span>|<span data-ttu-id="8c7eb-116">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c7eb-116">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c7eb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8c7eb-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/decisions/{accessReviewInstanceDecisionItemId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8c7eb-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8c7eb-118">Optional query parameters</span></span>
<span data-ttu-id="8c7eb-119">Este método dá suporte `$select` ao parâmetro de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8c7eb-119">This method supports `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="8c7eb-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="8c7eb-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="8c7eb-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8c7eb-121">Request headers</span></span>
|<span data-ttu-id="8c7eb-122">Nome</span><span class="sxs-lookup"><span data-stu-id="8c7eb-122">Name</span></span>|<span data-ttu-id="8c7eb-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c7eb-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8c7eb-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8c7eb-124">Authorization</span></span>|<span data-ttu-id="8c7eb-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8c7eb-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c7eb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8c7eb-127">Request body</span></span>
<span data-ttu-id="8c7eb-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8c7eb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c7eb-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c7eb-129">Response</span></span>

<span data-ttu-id="8c7eb-130">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8c7eb-130">If successful, this method returns a `200 OK` response code and an [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8c7eb-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8c7eb-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8c7eb-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8c7eb-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8c7eb-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="8c7eb-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessreviewinstancedecisionitem"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/abadf3b6-8ea4-4dea-90a5-9eac8fe93fbd/instances/abadf3b6-8ea4-4dea-90a5-9eac8fe93fbd/decisions/9550e25b-f315-4454-9d87-16b885c35de4
```
# <a name="c"></a>[<span data-ttu-id="8c7eb-134">C#</span><span class="sxs-lookup"><span data-stu-id="8c7eb-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreviewinstancedecisionitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8c7eb-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8c7eb-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreviewinstancedecisionitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8c7eb-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8c7eb-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreviewinstancedecisionitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8c7eb-137">Java</span><span class="sxs-lookup"><span data-stu-id="8c7eb-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreviewinstancedecisionitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="8c7eb-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c7eb-138">Response</span></span>
><span data-ttu-id="8c7eb-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8c7eb-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItem"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions('abadf3b6-8ea4-4dea-90a5-9eac8fe93fbd')/instances('7070ea1c-8d12-457b-bd35-a37dc59e54e0')/decisions/$entity",
    "id": "9550e25b-f315-4454-9d87-16b885c35de4",
    "accessReviewId": "7070ea1c-8d12-457b-bd35-a37dc59e54e0",
    "reviewedDateTime": null,
    "decision": "NotReviewed",
    "justification": "",
    "appliedDateTime": null,
    "applyResult": "New",
    "recommendation": "Deny",
    "principalLink": "https://graph.microsoft.com/v1.0/users/1800bb2c-955d-4205-8471-3a6c3116435d",
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
        "userId": "1800bb2c-955d-4205-8471-3a6c3116435d",
        "userDisplayName": "guest example",
        "userPrincipalName": "guest@guest.com"
    },
    "principal": {
        "@odata.type": "#microsoft.graph.userIdentity",
        "id": "1800bb2c-955d-4205-8471-3a6c3116435d",
        "displayName": "guest example",
        "userPrincipalName": "guest@guest.com"
    }
}
```
