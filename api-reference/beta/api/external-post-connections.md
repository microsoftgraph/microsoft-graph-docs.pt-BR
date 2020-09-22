---
title: Criar conexão
description: Use esta API para criar um novo externalConnection.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 2e2ebd954bf83b710835b6ad54fff7d7206a0025
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47980887"
---
# <a name="create-connection"></a><span data-ttu-id="b9c64-103">Criar conexão</span><span class="sxs-lookup"><span data-stu-id="b9c64-103">Create connection</span></span>

<span data-ttu-id="b9c64-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9c64-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9c64-105">Criar um novo [externalConnection](../resources/externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="b9c64-105">Create a new [externalConnection](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="b9c64-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b9c64-106">Permissions</span></span>

<span data-ttu-id="b9c64-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9c64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b9c64-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b9c64-109">Permission type</span></span>                        | <span data-ttu-id="b9c64-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b9c64-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b9c64-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b9c64-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b9c64-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9c64-112">Not supported.</span></span> |
| <span data-ttu-id="b9c64-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b9c64-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9c64-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9c64-114">Not supported.</span></span> |
| <span data-ttu-id="b9c64-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b9c64-115">Application</span></span>                            | <span data-ttu-id="b9c64-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9c64-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9c64-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b9c64-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /external/connections
```

## <a name="request-headers"></a><span data-ttu-id="b9c64-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b9c64-118">Request headers</span></span>

| <span data-ttu-id="b9c64-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b9c64-119">Name</span></span>          | <span data-ttu-id="b9c64-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9c64-120">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="b9c64-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b9c64-121">Authorization</span></span> | <span data-ttu-id="b9c64-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9c64-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="b9c64-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b9c64-124">Content-Type</span></span>  | <span data-ttu-id="b9c64-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9c64-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b9c64-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b9c64-127">Request body</span></span>

<span data-ttu-id="b9c64-128">No corpo da solicitação, forneça uma representação JSON de um objeto [externalConnection](../resources/externalconnection.md) .</span><span class="sxs-lookup"><span data-stu-id="b9c64-128">In the request body, supply a JSON representation of an [externalConnection](../resources/externalconnection.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b9c64-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9c64-129">Response</span></span>

<span data-ttu-id="b9c64-130">Se bem-sucedido, este método retorna `201 Created` um código de resposta e um novo objeto [externalConnection](../resources/externalconnection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b9c64-130">If successful, this method returns `201 Created` response code and a new [externalConnection](../resources/externalconnection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b9c64-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b9c64-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b9c64-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b9c64-132">Request</span></span>

<span data-ttu-id="b9c64-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b9c64-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b9c64-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b9c64-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b9c64-135">C#</span><span class="sxs-lookup"><span data-stu-id="b9c64-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-connection-from-external-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b9c64-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b9c64-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-connection-from-external-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b9c64-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b9c64-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-connection-from-external-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="b9c64-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9c64-138">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="b9c64-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b9c64-139">The following is an example of the response.</span></span>

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


