---
title: Obter ipNamedLocation
description: Recupere as propriedades e as relações de um objeto ipnamedlocation.
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: fbbf9d56ac73a997159b62e1483dde2d562e2ac5
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448043"
---
# <a name="get-ipnamedlocation"></a><span data-ttu-id="06a15-103">Obter ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="06a15-103">Get ipNamedLocation</span></span>

<span data-ttu-id="06a15-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06a15-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06a15-105">Recupere as propriedades e as relações de um [objeto ipNamedLocation.](../resources/ipNamedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="06a15-105">Retrieve the properties and relationships of an [ipNamedLocation](../resources/ipNamedLocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="06a15-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="06a15-106">Permissions</span></span>

<span data-ttu-id="06a15-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06a15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="06a15-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="06a15-109">Permission type</span></span>                        | <span data-ttu-id="06a15-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="06a15-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="06a15-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="06a15-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="06a15-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="06a15-112">Policy.Read.All</span></span> |
| <span data-ttu-id="06a15-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="06a15-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06a15-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06a15-114">Not supported.</span></span> |
| <span data-ttu-id="06a15-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="06a15-115">Application</span></span>                            | <span data-ttu-id="06a15-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="06a15-116">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="06a15-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="06a15-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/conditionalAccess/namedLocations/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="06a15-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="06a15-118">Optional query parameters</span></span>

<span data-ttu-id="06a15-119">Este método dá suporte ao `select` parâmetro de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="06a15-119">This method supports the `select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="06a15-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="06a15-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="06a15-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="06a15-121">Request headers</span></span>

| <span data-ttu-id="06a15-122">Nome</span><span class="sxs-lookup"><span data-stu-id="06a15-122">Name</span></span>      |<span data-ttu-id="06a15-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="06a15-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="06a15-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="06a15-124">Authorization</span></span> | <span data-ttu-id="06a15-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="06a15-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="06a15-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="06a15-127">Request body</span></span>

<span data-ttu-id="06a15-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="06a15-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06a15-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="06a15-129">Response</span></span>

<span data-ttu-id="06a15-130">Se tiver êxito, este método retornará um código de `200 OK` resposta e o objeto [ipNamedLocation](../resources/ipnamedlocation.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="06a15-130">If successful, this method returns a `200 OK` response code and the requested [ipNamedLocation](../resources/ipnamedlocation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="06a15-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="06a15-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="06a15-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="06a15-132">Request</span></span>

<span data-ttu-id="06a15-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="06a15-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="06a15-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="06a15-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_ipnamedlocation"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identity/conditionalAccess/namedLocations/0854951d-5fc0-4eb1-b392-9b2c9d7949c2
```
# <a name="c"></a>[<span data-ttu-id="06a15-135">C#</span><span class="sxs-lookup"><span data-stu-id="06a15-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-ipnamedlocation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="06a15-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="06a15-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-ipnamedlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="06a15-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="06a15-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-ipnamedlocation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="06a15-138">Java</span><span class="sxs-lookup"><span data-stu-id="06a15-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-ipnamedlocation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="06a15-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="06a15-139">Response</span></span>

<span data-ttu-id="06a15-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="06a15-140">The following is an example of the response.</span></span>

> <span data-ttu-id="06a15-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="06a15-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ipNamedLocation"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#namedLocations/$entity",
    "@odata.type": "#microsoft.graph.ipNamedLocation",
    "id": "0854951d-5fc0-4eb1-b392-9b2c9d7949c2",
    "displayName": "Untrusted IP named location",
    "modifiedDateTime": "2019-09-04T01:11:34.9387578Z",
    "createdDateTime": "2019-09-04T01:11:34.9387578Z",
    "isTrusted": false,
    "ipRanges": [
        {
            "@odata.type": "#microsoft.graph.iPv4CidrRange",
            "cidrAddress": "12.34.221.11/22"
        },
        {
            "@odata.type": "#microsoft.graph.iPv6CidrRange",
            "cidrAddress": "2001:0:9d38:90d6:0:0:0:0/63"
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get ipNamedLocation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


