---
title: Criar conexão
description: Use esta API para criar um novo externalConnection.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 67ccd63264d478ec33046cf03f6f8998ad3af7ba
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42422345"
---
# <a name="create-connection"></a><span data-ttu-id="b074a-103">Criar conexão</span><span class="sxs-lookup"><span data-stu-id="b074a-103">Create connection</span></span>

<span data-ttu-id="b074a-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b074a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b074a-105">Criar um novo [externalConnection](../resources/externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="b074a-105">Create a new [externalConnection](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="b074a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b074a-106">Permissions</span></span>

<span data-ttu-id="b074a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b074a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b074a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b074a-109">Permission type</span></span>                        | <span data-ttu-id="b074a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b074a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b074a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b074a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b074a-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b074a-112">Not supported.</span></span> |
| <span data-ttu-id="b074a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b074a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b074a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b074a-114">Not supported.</span></span> |
| <span data-ttu-id="b074a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b074a-115">Application</span></span>                            | <span data-ttu-id="b074a-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b074a-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b074a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b074a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /external/connections
```

## <a name="request-headers"></a><span data-ttu-id="b074a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b074a-118">Request headers</span></span>

| <span data-ttu-id="b074a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b074a-119">Name</span></span>          | <span data-ttu-id="b074a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b074a-120">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="b074a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b074a-121">Authorization</span></span> | <span data-ttu-id="b074a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b074a-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="b074a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b074a-124">Content-Type</span></span>  | <span data-ttu-id="b074a-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b074a-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b074a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b074a-127">Request body</span></span>

<span data-ttu-id="b074a-128">No corpo da solicitação, forneça uma representação JSON de um objeto [externalConnection](../resources/externalconnection.md) .</span><span class="sxs-lookup"><span data-stu-id="b074a-128">In the request body, supply a JSON representation of an [externalConnection](../resources/externalconnection.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b074a-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b074a-129">Response</span></span>

<span data-ttu-id="b074a-130">Se bem-sucedido, este método retorna `201 Created` um código de resposta e um novo objeto [externalConnection](../resources/externalconnection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b074a-130">If successful, this method returns `201 Created` response code and a new [externalConnection](../resources/externalconnection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b074a-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b074a-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b074a-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b074a-132">Request</span></span>

<span data-ttu-id="b074a-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b074a-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b074a-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b074a-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b074a-135">C#</span><span class="sxs-lookup"><span data-stu-id="b074a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-connection-from-external-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b074a-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b074a-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-connection-from-external-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b074a-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b074a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-connection-from-external-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="b074a-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="b074a-138">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="b074a-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b074a-139">The following is an example of the response.</span></span>

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
