---
title: Obter accessReviewInstance
description: Leia as propriedades e as relações de um objeto accessReviewInstance.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 8a8e2ec2ec059201dabea44523bf45ef054a4f3f
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031017"
---
# <a name="get-accessreviewinstance"></a><span data-ttu-id="4f5d2-103">Obter accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="4f5d2-103">Get accessReviewInstance</span></span>
<span data-ttu-id="4f5d2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f5d2-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="4f5d2-105">Leia as propriedades e as relações de um [objeto accessReviewInstance.](../resources/accessreviewinstance.md)</span><span class="sxs-lookup"><span data-stu-id="4f5d2-105">Read the properties and relationships of an [accessReviewInstance](../resources/accessreviewinstance.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4f5d2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4f5d2-106">Permissions</span></span>
<span data-ttu-id="4f5d2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f5d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f5d2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4f5d2-109">Permission type</span></span>|<span data-ttu-id="4f5d2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4f5d2-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f5d2-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4f5d2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4f5d2-112">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f5d2-112">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="4f5d2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4f5d2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f5d2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f5d2-114">Not supported.</span></span>|
|<span data-ttu-id="4f5d2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4f5d2-115">Application</span></span>|<span data-ttu-id="4f5d2-116">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f5d2-116">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f5d2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4f5d2-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4f5d2-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4f5d2-118">Optional query parameters</span></span>
<span data-ttu-id="4f5d2-119">Este método dá suporte `$select` ao parâmetro de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4f5d2-119">This method supports `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="4f5d2-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="4f5d2-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="4f5d2-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4f5d2-121">Request headers</span></span>
|<span data-ttu-id="4f5d2-122">Nome</span><span class="sxs-lookup"><span data-stu-id="4f5d2-122">Name</span></span>|<span data-ttu-id="4f5d2-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f5d2-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4f5d2-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="4f5d2-124">Authorization</span></span>|<span data-ttu-id="4f5d2-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4f5d2-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f5d2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4f5d2-127">Request body</span></span>
<span data-ttu-id="4f5d2-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4f5d2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f5d2-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f5d2-129">Response</span></span>

<span data-ttu-id="4f5d2-130">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto accessReviewInstance](../resources/accessreviewinstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4f5d2-130">If successful, this method returns a `200 OK` response code and an [accessReviewInstance](../resources/accessreviewinstance.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4f5d2-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4f5d2-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4f5d2-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4f5d2-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_accessreviewinstance"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/e6cafba0-cbf0-4748-8868-0810c7f4cc06/instances/12345ba0-cbf0-5678-8868-4444c7f4cc06
```


### <a name="response"></a><span data-ttu-id="4f5d2-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f5d2-133">Response</span></span>
><span data-ttu-id="4f5d2-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4f5d2-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewInstance"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.accessReviewInstance",
    "id": "d7fbc019-c019-d7fb-19c0-fbd719c0fbd7",
    "startDateTime": "2021-03-11T16:44:59.337Z",
    "endDateTime": "2021-06-09T16:44:59.337Z",
    "status": "InProgress",
    "scope": {
        "@odata.type": "#microsoft.graph.accessReviewQueryScope",
        "query": "/v1.0/groups/97eebd44-61fd-4d42-8b2a-a4de41b6c572/transitiveMembers",
        "queryType": "MicrosoftGraph",
        "queryRoot": null
    }
  }
}
```
