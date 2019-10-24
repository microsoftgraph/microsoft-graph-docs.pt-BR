---
title: Obter ipNamedLocation
description: Recupere as propriedades e os relacionamentos de um objeto ipnamedlocation.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b9aeb1bd07c465e73f55cf95fef71a80c8f5bb8f
ms.sourcegitcommit: d189830649794365464e37539e02239f883011da
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/24/2019
ms.locfileid: "37653710"
---
# <a name="get-ipnamedlocation"></a><span data-ttu-id="e39d2-103">Obter ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="e39d2-103">Get ipNamedLocation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e39d2-104">Recupere as propriedades e os relacionamentos de um objeto [ipNamedLocation](../resources/ipNamedLocation.md) .</span><span class="sxs-lookup"><span data-stu-id="e39d2-104">Retrieve the properties and relationships of an [ipNamedLocation](../resources/ipNamedLocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e39d2-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e39d2-105">Permissions</span></span>

<span data-ttu-id="e39d2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e39d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e39d2-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e39d2-108">Permission type</span></span>                        | <span data-ttu-id="e39d2-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e39d2-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e39d2-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e39d2-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e39d2-111">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="e39d2-111">Policy.Read.All</span></span> |
| <span data-ttu-id="e39d2-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e39d2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e39d2-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e39d2-113">Not supported.</span></span> |
| <span data-ttu-id="e39d2-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e39d2-114">Application</span></span>                            | <span data-ttu-id="e39d2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e39d2-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e39d2-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e39d2-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /conditionalAccess/namedLocations/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e39d2-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e39d2-117">Optional query parameters</span></span>

<span data-ttu-id="e39d2-118">Este método oferece suporte `select` ao parâmetro de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e39d2-118">This method supports the `select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="e39d2-119">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="e39d2-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e39d2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e39d2-120">Request headers</span></span>

| <span data-ttu-id="e39d2-121">Nome</span><span class="sxs-lookup"><span data-stu-id="e39d2-121">Name</span></span>      |<span data-ttu-id="e39d2-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e39d2-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e39d2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e39d2-123">Authorization</span></span> | <span data-ttu-id="e39d2-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e39d2-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e39d2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e39d2-126">Request body</span></span>

<span data-ttu-id="e39d2-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e39d2-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e39d2-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e39d2-128">Response</span></span>

<span data-ttu-id="e39d2-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [ipNamedLocation](../resources/ipnamedlocation.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e39d2-129">If successful, this method returns a `200 OK` response code and the requested [ipNamedLocation](../resources/ipnamedlocation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e39d2-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e39d2-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e39d2-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e39d2-131">Request</span></span>

<span data-ttu-id="e39d2-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e39d2-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_ipnamedlocation"
}-->

```http
GET https://graph.microsoft.com/beta/conditionalAccess/namedLocations/0854951d-5fc0-4eb1-b392-9b2c9d7949c2
```

### <a name="response"></a><span data-ttu-id="e39d2-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e39d2-133">Response</span></span>

<span data-ttu-id="e39d2-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e39d2-134">The following is an example of the response.</span></span>

> <span data-ttu-id="e39d2-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e39d2-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
