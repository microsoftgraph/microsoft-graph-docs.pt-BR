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
# <a name="get-schema"></a><span data-ttu-id="4874e-103">Obter esquema</span><span class="sxs-lookup"><span data-stu-id="4874e-103">Get schema</span></span>

<span data-ttu-id="4874e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4874e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4874e-105">Recuperar as propriedades de um [esquema](../resources/schema.md) para um [externalConnection](../resources/externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="4874e-105">Retrieve the properties of a [schema](../resources/schema.md) for an [externalConnection](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="4874e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4874e-106">Permissions</span></span>

<span data-ttu-id="4874e-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="4874e-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="4874e-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4874e-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4874e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4874e-109">Permission type</span></span>                        | <span data-ttu-id="4874e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4874e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4874e-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4874e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4874e-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4874e-112">Not supported.</span></span> |
| <span data-ttu-id="4874e-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4874e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4874e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4874e-114">Not supported.</span></span> |
| <span data-ttu-id="4874e-115">Application</span><span class="sxs-lookup"><span data-stu-id="4874e-115">Application</span></span>                            | <span data-ttu-id="4874e-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4874e-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4874e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4874e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections/{id}/schema
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4874e-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4874e-118">Optional query parameters</span></span>

<span data-ttu-id="4874e-119">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4874e-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="4874e-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="4874e-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="4874e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4874e-121">Request headers</span></span>

| <span data-ttu-id="4874e-122">Nome</span><span class="sxs-lookup"><span data-stu-id="4874e-122">Name</span></span>          | <span data-ttu-id="4874e-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="4874e-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="4874e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="4874e-124">Authorization</span></span> | <span data-ttu-id="4874e-125">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="4874e-125">Bearer {token}.</span></span> <span data-ttu-id="4874e-126">Required.</span><span class="sxs-lookup"><span data-stu-id="4874e-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4874e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4874e-127">Request body</span></span>

<span data-ttu-id="4874e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4874e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4874e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4874e-129">Response</span></span>

<span data-ttu-id="4874e-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto de [esquema](../resources/schema.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4874e-130">If successful, this method returns a `200 OK` response code and the requested [schema](../resources/schema.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4874e-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4874e-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4874e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4874e-132">Request</span></span>

<span data-ttu-id="4874e-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4874e-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4874e-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="4874e-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_schema"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/external/connections/contosohr/schema
```
# <a name="c"></a>[<span data-ttu-id="4874e-135">C#</span><span class="sxs-lookup"><span data-stu-id="4874e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schema-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4874e-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4874e-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schema-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4874e-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4874e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schema-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="4874e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="4874e-138">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="4874e-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4874e-139">The following is an example of the response.</span></span>

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
