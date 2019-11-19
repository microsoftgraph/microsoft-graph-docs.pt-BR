---
title: Obter namedLocation
description: Recupere as propriedades e os relacionamentos de um objeto namedlocation.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 90a4efbe68dda34995d73242f033d84013ef1620
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703725"
---
# <a name="get-namedlocation"></a><span data-ttu-id="7a7d4-103">Obter namedLocation</span><span class="sxs-lookup"><span data-stu-id="7a7d4-103">Get namedLocation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a7d4-104">Recupere as propriedades e os relacionamentos de um objeto [namedLocation](../resources/namedlocation.md) .</span><span class="sxs-lookup"><span data-stu-id="7a7d4-104">Retrieve the properties and relationships of a [namedLocation](../resources/namedlocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7a7d4-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7a7d4-105">Permissions</span></span>

<span data-ttu-id="7a7d4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a7d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7a7d4-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7a7d4-108">Permission type</span></span>                        | <span data-ttu-id="7a7d4-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7a7d4-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7a7d4-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7a7d4-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="7a7d4-111">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="7a7d4-111">Policy.Read.All</span></span> |
| <span data-ttu-id="7a7d4-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7a7d4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7a7d4-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7a7d4-113">Not supported.</span></span> |
| <span data-ttu-id="7a7d4-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7a7d4-114">Application</span></span>                            | <span data-ttu-id="7a7d4-115">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="7a7d4-115">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7a7d4-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7a7d4-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /conditionalAccess/namedLocations/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7a7d4-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7a7d4-117">Optional query parameters</span></span>

<span data-ttu-id="7a7d4-118">Este método oferece suporte `select` ao parâmetro de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7a7d4-118">This method supports the `select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="7a7d4-119">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="7a7d4-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7a7d4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7a7d4-120">Request headers</span></span>

| <span data-ttu-id="7a7d4-121">Nome</span><span class="sxs-lookup"><span data-stu-id="7a7d4-121">Name</span></span>      |<span data-ttu-id="7a7d4-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a7d4-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7a7d4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7a7d4-123">Authorization</span></span> | <span data-ttu-id="7a7d4-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a7d4-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7a7d4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7a7d4-126">Request body</span></span>

<span data-ttu-id="7a7d4-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7a7d4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7a7d4-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a7d4-128">Response</span></span>

<span data-ttu-id="7a7d4-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [namedLocation](../resources/namedlocation.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7a7d4-129">If successful, this method returns a `200 OK` response code and the requested [namedLocation](../resources/namedlocation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7a7d4-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7a7d4-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7a7d4-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7a7d4-131">Request</span></span>

<span data-ttu-id="7a7d4-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7a7d4-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7a7d4-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="7a7d4-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_namedlocation"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/conditionalAccess/namedLocations/0854951d-5fc0-4eb1-b392-9b2c9d7949c2
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7a7d4-134">C#</span><span class="sxs-lookup"><span data-stu-id="7a7d4-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-namedlocation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7a7d4-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7a7d4-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-namedlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7a7d4-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7a7d4-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-namedlocation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7a7d4-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a7d4-137">Response</span></span>

<span data-ttu-id="7a7d4-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7a7d4-138">The following is an example of the response.</span></span>

> <span data-ttu-id="7a7d4-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7a7d4-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedLocation"
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
  "description": "Get namedLocation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
