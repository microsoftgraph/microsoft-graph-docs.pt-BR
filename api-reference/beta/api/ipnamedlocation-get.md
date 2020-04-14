---
title: Obter ipNamedLocation
description: Recupere as propriedades e os relacionamentos de um objeto ipnamedlocation.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 56adfa46c706bbee37ab8d84f86e60ef2558cd34
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43458146"
---
# <a name="get-ipnamedlocation"></a><span data-ttu-id="47140-103">Obter ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="47140-103">Get ipNamedLocation</span></span>

<span data-ttu-id="47140-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47140-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47140-105">Recupere as propriedades e os relacionamentos de um objeto [ipNamedLocation](../resources/ipNamedLocation.md) .</span><span class="sxs-lookup"><span data-stu-id="47140-105">Retrieve the properties and relationships of an [ipNamedLocation](../resources/ipNamedLocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="47140-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="47140-106">Permissions</span></span>

<span data-ttu-id="47140-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47140-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="47140-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="47140-109">Permission type</span></span>                        | <span data-ttu-id="47140-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="47140-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="47140-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="47140-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="47140-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="47140-112">Policy.Read.All</span></span> |
| <span data-ttu-id="47140-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="47140-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47140-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47140-114">Not supported.</span></span> |
| <span data-ttu-id="47140-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="47140-115">Application</span></span>                            | <span data-ttu-id="47140-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="47140-116">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="47140-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="47140-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/conditionalAccess/namedLocations/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="47140-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="47140-118">Optional query parameters</span></span>

<span data-ttu-id="47140-119">Este método oferece suporte `select` ao parâmetro de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="47140-119">This method supports the `select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="47140-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="47140-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="47140-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="47140-121">Request headers</span></span>

| <span data-ttu-id="47140-122">Nome</span><span class="sxs-lookup"><span data-stu-id="47140-122">Name</span></span>      |<span data-ttu-id="47140-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="47140-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="47140-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="47140-124">Authorization</span></span> | <span data-ttu-id="47140-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="47140-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="47140-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="47140-127">Request body</span></span>

<span data-ttu-id="47140-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="47140-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47140-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="47140-129">Response</span></span>

<span data-ttu-id="47140-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [ipNamedLocation](../resources/ipnamedlocation.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47140-130">If successful, this method returns a `200 OK` response code and the requested [ipNamedLocation](../resources/ipnamedlocation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="47140-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="47140-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="47140-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="47140-132">Request</span></span>

<span data-ttu-id="47140-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="47140-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="47140-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="47140-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_ipnamedlocation"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identity/conditionalAccess/namedLocations/0854951d-5fc0-4eb1-b392-9b2c9d7949c2
```
# <a name="c"></a>[<span data-ttu-id="47140-135">C#</span><span class="sxs-lookup"><span data-stu-id="47140-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-ipnamedlocation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="47140-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="47140-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-ipnamedlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="47140-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="47140-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-ipnamedlocation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="47140-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="47140-138">Response</span></span>

<span data-ttu-id="47140-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="47140-139">The following is an example of the response.</span></span>

> <span data-ttu-id="47140-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="47140-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
