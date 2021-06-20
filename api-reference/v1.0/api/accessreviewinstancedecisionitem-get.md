---
title: Obter accessReviewInstanceDecisionItem
description: Leia as propriedades e as relações de um objeto accessReviewInstanceDecisionItem.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 33a4ffa25cf02c81b3975647cb42dd74f2b6c669
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030995"
---
# <a name="get-accessreviewinstancedecisionitem"></a><span data-ttu-id="079ac-103">Obter accessReviewInstanceDecisionItem</span><span class="sxs-lookup"><span data-stu-id="079ac-103">Get accessReviewInstanceDecisionItem</span></span>
<span data-ttu-id="079ac-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="079ac-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="079ac-105">Leia as propriedades e as relações de um [objeto accessReviewInstanceDecisionItem.](../resources/accessreviewinstancedecisionitem.md)</span><span class="sxs-lookup"><span data-stu-id="079ac-105">Read the properties and relationships of an [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="079ac-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="079ac-106">Permissions</span></span>
<span data-ttu-id="079ac-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="079ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="079ac-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="079ac-109">Permission type</span></span>|<span data-ttu-id="079ac-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="079ac-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="079ac-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="079ac-111">Delegated (work or school account)</span></span>|<span data-ttu-id="079ac-112">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="079ac-112">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="079ac-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="079ac-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="079ac-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="079ac-114">Not supported.</span></span>|
|<span data-ttu-id="079ac-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="079ac-115">Application</span></span>|<span data-ttu-id="079ac-116">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="079ac-116">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="079ac-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="079ac-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/decisions/{accessReviewInstanceDecisionItemId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="079ac-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="079ac-118">Optional query parameters</span></span>
<span data-ttu-id="079ac-119">Este método dá suporte `$select` ao parâmetro de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="079ac-119">This method supports `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="079ac-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="079ac-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="079ac-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="079ac-121">Request headers</span></span>
|<span data-ttu-id="079ac-122">Nome</span><span class="sxs-lookup"><span data-stu-id="079ac-122">Name</span></span>|<span data-ttu-id="079ac-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="079ac-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="079ac-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="079ac-124">Authorization</span></span>|<span data-ttu-id="079ac-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="079ac-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="079ac-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="079ac-127">Request body</span></span>
<span data-ttu-id="079ac-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="079ac-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="079ac-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="079ac-129">Response</span></span>

<span data-ttu-id="079ac-130">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="079ac-130">If successful, this method returns a `200 OK` response code and an [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="079ac-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="079ac-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="079ac-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="079ac-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_accessreviewinstancedecisionitem"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/abadf3b6-8ea4-4dea-90a5-9eac8fe93fbd/instances/abadf3b6-8ea4-4dea-90a5-9eac8fe93fbd/decisions/9550e25b-f315-4454-9d87-16b885c35de4
```


### <a name="response"></a><span data-ttu-id="079ac-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="079ac-133">Response</span></span>
><span data-ttu-id="079ac-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="079ac-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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
