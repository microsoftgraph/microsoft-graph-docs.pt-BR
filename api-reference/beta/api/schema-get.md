---
title: Obter esquema
description: Recuperar as propriedades de um esquema para um externalConnection.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 7b946638c4d433e8cae6c6459ac434041c17f7bb
ms.sourcegitcommit: 05645bc582d14781a9ca6b78ed598a4e7dc26869
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2020
ms.locfileid: "44990294"
---
# <a name="get-schema"></a><span data-ttu-id="4529f-103">Obter esquema</span><span class="sxs-lookup"><span data-stu-id="4529f-103">Get schema</span></span>

<span data-ttu-id="4529f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4529f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4529f-105">Recuperar as propriedades de um [esquema](../resources/schema.md) para um [externalConnection](../resources/externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="4529f-105">Retrieve the properties of a [schema](../resources/schema.md) for an [externalConnection](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="4529f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4529f-106">Permissions</span></span>

<span data-ttu-id="4529f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4529f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4529f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4529f-109">Permission type</span></span>                        | <span data-ttu-id="4529f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4529f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4529f-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4529f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4529f-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4529f-112">Not supported.</span></span> |
| <span data-ttu-id="4529f-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4529f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4529f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4529f-114">Not supported.</span></span> |
| <span data-ttu-id="4529f-115">Application</span><span class="sxs-lookup"><span data-stu-id="4529f-115">Application</span></span>                            | <span data-ttu-id="4529f-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4529f-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4529f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4529f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections/{id}/schema
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4529f-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4529f-118">Optional query parameters</span></span>

<span data-ttu-id="4529f-119">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4529f-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="4529f-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="4529f-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="4529f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4529f-121">Request headers</span></span>

| <span data-ttu-id="4529f-122">Nome</span><span class="sxs-lookup"><span data-stu-id="4529f-122">Name</span></span>          | <span data-ttu-id="4529f-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="4529f-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="4529f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="4529f-124">Authorization</span></span> | <span data-ttu-id="4529f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4529f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4529f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4529f-127">Request body</span></span>

<span data-ttu-id="4529f-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4529f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4529f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4529f-129">Response</span></span>

<span data-ttu-id="4529f-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto de [esquema](../resources/schema.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4529f-130">If successful, this method returns a `200 OK` response code and the requested [schema](../resources/schema.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4529f-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4529f-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4529f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4529f-132">Request</span></span>

<span data-ttu-id="4529f-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4529f-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4529f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="4529f-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_schema"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/external/connections/contosohr/schema
```
# <a name="c"></a>[<span data-ttu-id="4529f-135">C#</span><span class="sxs-lookup"><span data-stu-id="4529f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schema-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4529f-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4529f-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schema-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4529f-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4529f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schema-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="4529f-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="4529f-138">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="4529f-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4529f-139">The following is an example of the response.</span></span>

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
