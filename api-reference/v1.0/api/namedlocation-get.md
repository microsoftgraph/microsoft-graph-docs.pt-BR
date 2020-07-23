---
title: Obter namedLocation
description: Recupere as propriedades e os relacionamentos de um objeto namedlocation.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e2ee8a9be544679464e9aea9fdd2702c0a01ffc9
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384443"
---
# <a name="get-namedlocation"></a><span data-ttu-id="80bec-103">Obter namedLocation</span><span class="sxs-lookup"><span data-stu-id="80bec-103">Get namedLocation</span></span>

<span data-ttu-id="80bec-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80bec-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="80bec-105">Recupere as propriedades e os relacionamentos de um objeto [namedLocation](../resources/namedlocation.md) .</span><span class="sxs-lookup"><span data-stu-id="80bec-105">Retrieve the properties and relationships of a [namedLocation](../resources/namedlocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="80bec-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="80bec-106">Permissions</span></span>

<span data-ttu-id="80bec-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80bec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="80bec-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="80bec-109">Permission type</span></span>                        | <span data-ttu-id="80bec-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="80bec-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="80bec-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="80bec-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="80bec-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="80bec-112">Policy.Read.All</span></span> |
| <span data-ttu-id="80bec-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="80bec-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80bec-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="80bec-114">Not supported.</span></span> |
| <span data-ttu-id="80bec-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="80bec-115">Application</span></span>                            | <span data-ttu-id="80bec-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="80bec-116">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="80bec-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="80bec-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/conditionalAccess/namedLocations/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="80bec-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="80bec-118">Optional query parameters</span></span>

<span data-ttu-id="80bec-119">Este método oferece suporte ao `select` parâmetro de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="80bec-119">This method supports the `select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="80bec-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="80bec-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="80bec-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="80bec-121">Request headers</span></span>

| <span data-ttu-id="80bec-122">Nome</span><span class="sxs-lookup"><span data-stu-id="80bec-122">Name</span></span>      |<span data-ttu-id="80bec-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="80bec-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="80bec-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="80bec-124">Authorization</span></span> | <span data-ttu-id="80bec-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="80bec-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="80bec-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="80bec-127">Request body</span></span>

<span data-ttu-id="80bec-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="80bec-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="80bec-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="80bec-129">Response</span></span>

<span data-ttu-id="80bec-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [namedLocation](../resources/namedlocation.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="80bec-130">If successful, this method returns a `200 OK` response code and the requested [namedLocation](../resources/namedlocation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="80bec-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="80bec-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="80bec-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="80bec-132">Request</span></span>

<span data-ttu-id="80bec-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="80bec-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_namedlocation"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/identity/conditionalAccess/namedLocations/0854951d-5fc0-4eb1-b392-9b2c9d7949c2
```

### <a name="response"></a><span data-ttu-id="80bec-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="80bec-134">Response</span></span>

<span data-ttu-id="80bec-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="80bec-135">The following is an example of the response.</span></span>

> <span data-ttu-id="80bec-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="80bec-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedLocation"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#namedLocations/$entity",
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
