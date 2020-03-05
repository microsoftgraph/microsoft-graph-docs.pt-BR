---
title: Obter esquema
description: Recuperar as propriedades de um esquema para um externalConnection.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: de4e793a224466738773f959892a31b002737f92
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453762"
---
# <a name="get-schema"></a><span data-ttu-id="bb401-103">Obter esquema</span><span class="sxs-lookup"><span data-stu-id="bb401-103">Get schema</span></span>

<span data-ttu-id="bb401-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="bb401-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb401-105">Recuperar as propriedades de um [esquema](../resources/schema.md) para um [externalConnection](../resources/externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="bb401-105">Retrieve the properties of a [schema](../resources/schema.md) for an [externalConnection](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="bb401-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bb401-106">Permissions</span></span>

<span data-ttu-id="bb401-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb401-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bb401-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bb401-109">Permission type</span></span>                        | <span data-ttu-id="bb401-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bb401-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bb401-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bb401-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bb401-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb401-112">Not supported.</span></span> |
| <span data-ttu-id="bb401-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bb401-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb401-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb401-114">Not supported.</span></span> |
| <span data-ttu-id="bb401-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bb401-115">Application</span></span>                            | <span data-ttu-id="bb401-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb401-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bb401-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bb401-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections/{id}/schema
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bb401-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bb401-118">Optional query parameters</span></span>

<span data-ttu-id="bb401-119">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bb401-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="bb401-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="bb401-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="bb401-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bb401-121">Request headers</span></span>

| <span data-ttu-id="bb401-122">Nome</span><span class="sxs-lookup"><span data-stu-id="bb401-122">Name</span></span>          | <span data-ttu-id="bb401-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb401-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="bb401-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="bb401-124">Authorization</span></span> | <span data-ttu-id="bb401-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bb401-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bb401-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bb401-127">Request body</span></span>

<span data-ttu-id="bb401-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bb401-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb401-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb401-129">Response</span></span>

<span data-ttu-id="bb401-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto de [esquema](../resources/schema.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bb401-130">If successful, this method returns a `200 OK` response code and the requested [schema](../resources/schema.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bb401-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="bb401-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bb401-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bb401-132">Request</span></span>

<span data-ttu-id="bb401-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bb401-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bb401-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="bb401-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_schema"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/external/connections/contosohr/schema
```
# <a name="c"></a>[<span data-ttu-id="bb401-135">C#</span><span class="sxs-lookup"><span data-stu-id="bb401-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schema-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bb401-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bb401-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schema-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bb401-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bb401-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schema-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="bb401-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb401-138">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="bb401-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bb401-139">The following is an example of the response.</span></span>

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
