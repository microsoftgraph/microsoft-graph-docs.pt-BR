---
title: Obter esquema
description: Recuperar as propriedades de um esquema para um externalConnection.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: d27457c3aab9876bc26d95ad2e5f52a1b11bdb79
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48975333"
---
# <a name="get-schema"></a><span data-ttu-id="8846c-103">Obter esquema</span><span class="sxs-lookup"><span data-stu-id="8846c-103">Get schema</span></span>

<span data-ttu-id="8846c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8846c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8846c-105">Recuperar as propriedades de um [esquema](../resources/schema.md) para um [externalConnection](../resources/externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="8846c-105">Retrieve the properties of a [schema](../resources/schema.md) for an [externalConnection](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="8846c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8846c-106">Permissions</span></span>

<span data-ttu-id="8846c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8846c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8846c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8846c-109">Permission type</span></span>                        | <span data-ttu-id="8846c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8846c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8846c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8846c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8846c-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8846c-112">Not supported.</span></span> |
| <span data-ttu-id="8846c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8846c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8846c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8846c-114">Not supported.</span></span> |
| <span data-ttu-id="8846c-115">Application</span><span class="sxs-lookup"><span data-stu-id="8846c-115">Application</span></span>                            | <span data-ttu-id="8846c-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8846c-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8846c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8846c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections/{id}/schema
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8846c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8846c-118">Optional query parameters</span></span>

<span data-ttu-id="8846c-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8846c-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="8846c-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="8846c-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="8846c-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8846c-121">Request headers</span></span>

| <span data-ttu-id="8846c-122">Nome</span><span class="sxs-lookup"><span data-stu-id="8846c-122">Name</span></span>          | <span data-ttu-id="8846c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="8846c-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="8846c-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8846c-124">Authorization</span></span> | <span data-ttu-id="8846c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8846c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8846c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8846c-127">Request body</span></span>

<span data-ttu-id="8846c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8846c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8846c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8846c-129">Response</span></span>

<span data-ttu-id="8846c-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto de [esquema](../resources/schema.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8846c-130">If successful, this method returns a `200 OK` response code and the requested [schema](../resources/schema.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8846c-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8846c-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8846c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8846c-132">Request</span></span>

<span data-ttu-id="8846c-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8846c-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8846c-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="8846c-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_schema"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/external/connections/contosohr/schema
```
# <a name="c"></a>[<span data-ttu-id="8846c-135">C#</span><span class="sxs-lookup"><span data-stu-id="8846c-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schema-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8846c-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8846c-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schema-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8846c-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8846c-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schema-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8846c-138">Java</span><span class="sxs-lookup"><span data-stu-id="8846c-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-schema-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="8846c-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="8846c-139">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="8846c-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8846c-140">The following is an example of the response.</span></span>

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
      "name": "ticketTitle",
      "type": "String",
      "isSearchable": true,
      "isRetrievable": true,
      "labels": [
        "title"
      ]
    },
    {
      "name": "priority",
      "type": "String",
      "isQueryable": true,
      "isRetrievable": true,
      "isRefinable": true,
      "isSearchable": false
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


