---
title: Obter accessReviewInstanceDecisionItem
description: Leia as propriedades e as relações de um objeto accessReviewInstanceDecisionItem.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 7354b9eba451c7ea19aac4def869fad4a31e4346
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207424"
---
# <a name="get-accessreviewinstancedecisionitem"></a><span data-ttu-id="f2332-103">Obter accessReviewInstanceDecisionItem</span><span class="sxs-lookup"><span data-stu-id="f2332-103">Get accessReviewInstanceDecisionItem</span></span>
<span data-ttu-id="f2332-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2332-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2332-105">Leia as propriedades e as relações de um [objeto accessReviewInstanceDecisionItem.](../resources/accessreviewinstancedecisionitem.md)</span><span class="sxs-lookup"><span data-stu-id="f2332-105">Read the properties and relationships of an [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f2332-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f2332-106">Permissions</span></span>
<span data-ttu-id="f2332-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2332-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2332-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f2332-109">Permission type</span></span>|<span data-ttu-id="f2332-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f2332-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2332-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f2332-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f2332-112">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2332-112">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="f2332-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f2332-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2332-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2332-114">Not supported.</span></span>|
|<span data-ttu-id="f2332-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2332-115">Application</span></span>|<span data-ttu-id="f2332-116">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2332-116">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2332-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f2332-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/decisions/{accessReviewInstanceDecisionItemId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f2332-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f2332-118">Optional query parameters</span></span>
<span data-ttu-id="f2332-119">Este método dá suporte `$select` ao parâmetro de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f2332-119">This method supports `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="f2332-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f2332-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f2332-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f2332-121">Request headers</span></span>
|<span data-ttu-id="f2332-122">Nome</span><span class="sxs-lookup"><span data-stu-id="f2332-122">Name</span></span>|<span data-ttu-id="f2332-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2332-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f2332-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f2332-124">Authorization</span></span>|<span data-ttu-id="f2332-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2332-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2332-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f2332-127">Request body</span></span>
<span data-ttu-id="f2332-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f2332-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2332-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2332-129">Response</span></span>

<span data-ttu-id="f2332-130">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f2332-130">If successful, this method returns a `200 OK` response code and an [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f2332-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f2332-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f2332-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2332-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f2332-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f2332-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessreviewinstancedecisionitem"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/5eac5a70-7cd7-4f20-92b0-f9dba70dd7f0/instances/6444d4fd-ab55-4608-8cf9-c6702d172bcc/decisions/e6cafba0-cbf0-4748-8868-0810c7f4cc06
```
# <a name="c"></a>[<span data-ttu-id="f2332-134">C#</span><span class="sxs-lookup"><span data-stu-id="f2332-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreviewinstancedecisionitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f2332-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f2332-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreviewinstancedecisionitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f2332-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f2332-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreviewinstancedecisionitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f2332-137">Java</span><span class="sxs-lookup"><span data-stu-id="f2332-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreviewinstancedecisionitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="f2332-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2332-138">Response</span></span>
><span data-ttu-id="f2332-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f2332-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions('5eac5a70-7cd7-4f20-92b0-f9dba70dd7f0')/instances('6444d4fd-ab55-4608-8cf9-c6702d172bcc')/decisions/$entity",
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
}
```
