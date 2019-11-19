---
title: Obter esquema
description: Recuperar as propriedades de um esquema para um externalConnection.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: da42ecae79e7e0a81a77edf510a082bb8d3990c2
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703718"
---
# <a name="get-schema"></a><span data-ttu-id="3616c-103">Obter esquema</span><span class="sxs-lookup"><span data-stu-id="3616c-103">Get schema</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3616c-104">Recuperar as propriedades de um [esquema](../resources/schema.md) para um [externalConnection](../resources/externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="3616c-104">Retrieve the properties of a [schema](../resources/schema.md) for an [externalConnection](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="3616c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3616c-105">Permissions</span></span>

<span data-ttu-id="3616c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3616c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3616c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3616c-108">Permission type</span></span>                        | <span data-ttu-id="3616c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3616c-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3616c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3616c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="3616c-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3616c-111">Not supported.</span></span> |
| <span data-ttu-id="3616c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3616c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3616c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3616c-113">Not supported.</span></span> |
| <span data-ttu-id="3616c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3616c-114">Application</span></span>                            | <span data-ttu-id="3616c-115">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3616c-115">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3616c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3616c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections/{id}/schema
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3616c-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3616c-117">Optional query parameters</span></span>

<span data-ttu-id="3616c-118">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3616c-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="3616c-119">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="3616c-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3616c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3616c-120">Request headers</span></span>

| <span data-ttu-id="3616c-121">Nome</span><span class="sxs-lookup"><span data-stu-id="3616c-121">Name</span></span>          | <span data-ttu-id="3616c-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="3616c-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="3616c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3616c-123">Authorization</span></span> | <span data-ttu-id="3616c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3616c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3616c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3616c-126">Request body</span></span>

<span data-ttu-id="3616c-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3616c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3616c-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="3616c-128">Response</span></span>

<span data-ttu-id="3616c-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto de [esquema](../resources/schema.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3616c-129">If successful, this method returns a `200 OK` response code and the requested [schema](../resources/schema.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3616c-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3616c-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3616c-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3616c-131">Request</span></span>

<span data-ttu-id="3616c-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3616c-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3616c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="3616c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_schema"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/external/connections/contosohr/schema
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3616c-134">C#</span><span class="sxs-lookup"><span data-stu-id="3616c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schema-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3616c-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3616c-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schema-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3616c-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3616c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schema-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="3616c-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="3616c-137">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="3616c-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3616c-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schema"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "baseType": "microsoft.graph.externalItem",
  "properties": [
    {
      "name": "title",
      "type": "String",
      "isSearchable": true,
      "isRetrievable": true
    },
    {
      "name": "priority",
      "type": "String",
      "isQueryable": true,
      "isRetrievable": true
    },
    {
      "name": "assignee",
      "type": "String",
      "isRetrievable": true
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get schema",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
