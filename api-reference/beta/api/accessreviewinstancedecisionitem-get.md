---
title: Obter accessReviewInstanceDecisionItem
description: Leia as propriedades e as relações de um objeto accessReviewInstanceDecisionItem.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 22dea5e8d96a1aa356bb4ae7e984262ef09c4d4f
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031423"
---
# <a name="get-accessreviewinstancedecisionitem"></a><span data-ttu-id="fbff9-103">Obter accessReviewInstanceDecisionItem</span><span class="sxs-lookup"><span data-stu-id="fbff9-103">Get accessReviewInstanceDecisionItem</span></span>
<span data-ttu-id="fbff9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fbff9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fbff9-105">Leia as propriedades e as relações de um [objeto accessReviewInstanceDecisionItem.](../resources/accessreviewinstancedecisionitem.md)</span><span class="sxs-lookup"><span data-stu-id="fbff9-105">Read the properties and relationships of an [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fbff9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fbff9-106">Permissions</span></span>
<span data-ttu-id="fbff9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fbff9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbff9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fbff9-109">Permission type</span></span>|<span data-ttu-id="fbff9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fbff9-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fbff9-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fbff9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fbff9-112">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbff9-112">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="fbff9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fbff9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fbff9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fbff9-114">Not supported.</span></span>|
|<span data-ttu-id="fbff9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fbff9-115">Application</span></span>|<span data-ttu-id="fbff9-116">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbff9-116">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fbff9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fbff9-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/decisions/{accessReviewInstanceDecisionItemId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fbff9-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fbff9-118">Optional query parameters</span></span>
<span data-ttu-id="fbff9-119">Este método dá suporte `$select` ao parâmetro de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fbff9-119">This method supports `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="fbff9-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="fbff9-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="fbff9-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fbff9-121">Request headers</span></span>
|<span data-ttu-id="fbff9-122">Nome</span><span class="sxs-lookup"><span data-stu-id="fbff9-122">Name</span></span>|<span data-ttu-id="fbff9-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="fbff9-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fbff9-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="fbff9-124">Authorization</span></span>|<span data-ttu-id="fbff9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fbff9-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fbff9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fbff9-127">Request body</span></span>
<span data-ttu-id="fbff9-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fbff9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fbff9-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="fbff9-129">Response</span></span>

<span data-ttu-id="fbff9-130">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fbff9-130">If successful, this method returns a `200 OK` response code and an [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fbff9-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fbff9-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fbff9-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fbff9-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_accessreviewinstancedecisionitem"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/5eac5a70-7cd7-4f20-92b0-f9dba70dd7f0/instances/6444d4fd-ab55-4608-8cf9-c6702d172bcc/decisions/e6cafba0-cbf0-4748-8868-0810c7f4cc06
```


### <a name="response"></a><span data-ttu-id="fbff9-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="fbff9-133">Response</span></span>
><span data-ttu-id="fbff9-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="fbff9-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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
