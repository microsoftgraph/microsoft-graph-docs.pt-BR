---
title: Obter accessReviewInstance
description: Leia as propriedades e as relações de um objeto accessReviewInstance.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 62d18407a457de2c335656800c12d2b311ea90b6
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210987"
---
# <a name="get-accessreviewinstance"></a><span data-ttu-id="a6dec-103">Obter accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="a6dec-103">Get accessReviewInstance</span></span>
<span data-ttu-id="a6dec-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6dec-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="a6dec-105">Leia as propriedades e as relações de um [objeto accessReviewInstance.](../resources/accessreviewinstance.md)</span><span class="sxs-lookup"><span data-stu-id="a6dec-105">Read the properties and relationships of an [accessReviewInstance](../resources/accessreviewinstance.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a6dec-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a6dec-106">Permissions</span></span>
<span data-ttu-id="a6dec-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6dec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6dec-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a6dec-109">Permission type</span></span>|<span data-ttu-id="a6dec-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a6dec-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6dec-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a6dec-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a6dec-112">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6dec-112">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="a6dec-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a6dec-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6dec-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6dec-114">Not supported.</span></span>|
|<span data-ttu-id="a6dec-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a6dec-115">Application</span></span>|<span data-ttu-id="a6dec-116">AccessReview.Read.All, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6dec-116">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6dec-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a6dec-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a6dec-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a6dec-118">Optional query parameters</span></span>
<span data-ttu-id="a6dec-119">Este método dá suporte `$select` ao parâmetro de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a6dec-119">This method supports `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="a6dec-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a6dec-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a6dec-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a6dec-121">Request headers</span></span>
|<span data-ttu-id="a6dec-122">Nome</span><span class="sxs-lookup"><span data-stu-id="a6dec-122">Name</span></span>|<span data-ttu-id="a6dec-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6dec-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a6dec-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a6dec-124">Authorization</span></span>|<span data-ttu-id="a6dec-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6dec-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6dec-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a6dec-127">Request body</span></span>
<span data-ttu-id="a6dec-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a6dec-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6dec-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6dec-129">Response</span></span>

<span data-ttu-id="a6dec-130">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto accessReviewInstance](../resources/accessreviewinstance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a6dec-130">If successful, this method returns a `200 OK` response code and an [accessReviewInstance](../resources/accessreviewinstance.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a6dec-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a6dec-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a6dec-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a6dec-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a6dec-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a6dec-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessreviewinstance"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/e6cafba0-cbf0-4748-8868-0810c7f4cc06/instances/12345ba0-cbf0-5678-8868-4444c7f4cc06
```
# <a name="c"></a>[<span data-ttu-id="a6dec-134">C#</span><span class="sxs-lookup"><span data-stu-id="a6dec-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreviewinstance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a6dec-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a6dec-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreviewinstance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a6dec-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a6dec-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreviewinstance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a6dec-137">Java</span><span class="sxs-lookup"><span data-stu-id="a6dec-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreviewinstance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="a6dec-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6dec-138">Response</span></span>
><span data-ttu-id="a6dec-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a6dec-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
