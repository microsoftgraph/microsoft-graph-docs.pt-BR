---
title: Criar conexão
description: Use esta API para criar um novo externalConnection.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: b69cf68f178a3a8a3ad21928ca4ccbf6dc5b59fb
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869770"
---
# <a name="create-connection"></a><span data-ttu-id="0d3a9-103">Criar conexão</span><span class="sxs-lookup"><span data-stu-id="0d3a9-103">Create connection</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d3a9-104">Criar um novo [externalConnection](../resources/externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="0d3a9-104">Create a new [externalConnection](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="0d3a9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0d3a9-105">Permissions</span></span>

<span data-ttu-id="0d3a9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d3a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0d3a9-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0d3a9-108">Permission type</span></span>                        | <span data-ttu-id="0d3a9-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0d3a9-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0d3a9-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0d3a9-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0d3a9-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d3a9-111">Not supported.</span></span> |
| <span data-ttu-id="0d3a9-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0d3a9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d3a9-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d3a9-113">Not supported.</span></span> |
| <span data-ttu-id="0d3a9-114">Application</span><span class="sxs-lookup"><span data-stu-id="0d3a9-114">Application</span></span>                            | <span data-ttu-id="0d3a9-115">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d3a9-115">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d3a9-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0d3a9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /external/connections
```

## <a name="request-headers"></a><span data-ttu-id="0d3a9-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0d3a9-117">Request headers</span></span>

| <span data-ttu-id="0d3a9-118">Nome</span><span class="sxs-lookup"><span data-stu-id="0d3a9-118">Name</span></span>          | <span data-ttu-id="0d3a9-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d3a9-119">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="0d3a9-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="0d3a9-120">Authorization</span></span> | <span data-ttu-id="0d3a9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0d3a9-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="0d3a9-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0d3a9-123">Content-Type</span></span>  | <span data-ttu-id="0d3a9-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0d3a9-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0d3a9-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0d3a9-126">Request body</span></span>

<span data-ttu-id="0d3a9-127">No corpo da solicitação, forneça uma representação JSON de um objeto [externalConnection](../resources/externalconnection.md) .</span><span class="sxs-lookup"><span data-stu-id="0d3a9-127">In the request body, supply a JSON representation of an [externalConnection](../resources/externalconnection.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="0d3a9-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d3a9-128">Response</span></span>

<span data-ttu-id="0d3a9-129">Se bem-sucedido, este método retorna `201 Created` um código de resposta e um novo objeto [externalConnection](../resources/externalconnection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0d3a9-129">If successful, this method returns `201 Created` response code and a new [externalConnection](../resources/externalconnection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0d3a9-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0d3a9-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0d3a9-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0d3a9-131">Request</span></span>

<span data-ttu-id="0d3a9-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0d3a9-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0d3a9-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="0d3a9-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_connection_from_external"
}-->

```http
POST https://graph.microsoft.com/beta/external/connections
Content-type: application/json

{
  "id": "contosohr",
  "name": "Contoso HR",
  "description": "Connection to index Contoso HR system"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0d3a9-134">C#</span><span class="sxs-lookup"><span data-stu-id="0d3a9-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-connection-from-external-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0d3a9-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0d3a9-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-connection-from-external-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0d3a9-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0d3a9-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-connection-from-external-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="0d3a9-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d3a9-137">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="0d3a9-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0d3a9-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnection"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "contosohr",
  "name": "Contoso HR",
  "description": "Connection to index Contoso HR system",
  "configuration": {
    "authorizedApps": [
      "d310d35d-72ec-47dd-92f2-fb9c40936555"
    ]
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create connection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
