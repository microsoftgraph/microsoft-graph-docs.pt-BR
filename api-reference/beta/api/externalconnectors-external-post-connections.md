---
title: Criar conexão
description: Use essa API para criar um novo externalConnection.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: c4415c33e759bde7a95eb37ec6254762a925058e
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467557"
---
# <a name="create-connection"></a><span data-ttu-id="7188c-103">Criar conexão</span><span class="sxs-lookup"><span data-stu-id="7188c-103">Create connection</span></span>

<span data-ttu-id="7188c-104">Namespace: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="7188c-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7188c-105">Crie um novo [externalConnection](../resources/externalconnectors-externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="7188c-105">Create a new [externalConnection](../resources/externalconnectors-externalconnection.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7188c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7188c-106">Permissions</span></span>

<span data-ttu-id="7188c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7188c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7188c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7188c-109">Permission type</span></span>                        | <span data-ttu-id="7188c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7188c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7188c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7188c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7188c-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7188c-112">Not supported.</span></span> |
| <span data-ttu-id="7188c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7188c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7188c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7188c-114">Not supported.</span></span> |
| <span data-ttu-id="7188c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7188c-115">Application</span></span>                            | <span data-ttu-id="7188c-116">ExternalConnection.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="7188c-116">ExternalConnection.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="7188c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7188c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /external/connections
```

## <a name="request-headers"></a><span data-ttu-id="7188c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7188c-118">Request headers</span></span>

| <span data-ttu-id="7188c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="7188c-119">Name</span></span>          | <span data-ttu-id="7188c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="7188c-120">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="7188c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7188c-121">Authorization</span></span> | <span data-ttu-id="7188c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7188c-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="7188c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7188c-124">Content-Type</span></span>  | <span data-ttu-id="7188c-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7188c-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7188c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7188c-127">Request body</span></span>

<span data-ttu-id="7188c-128">No corpo da solicitação, fornece uma representação JSON de um [objeto externalConnection.](../resources/externalconnectors-externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="7188c-128">In the request body, supply a JSON representation of an [externalConnection](../resources/externalconnectors-externalconnection.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7188c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="7188c-129">Response</span></span>

<span data-ttu-id="7188c-130">Se tiver êxito, este método retornará `201 Created` o código de resposta e um novo objeto [externalConnection](../resources/externalconnectors-externalconnection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7188c-130">If successful, this method returns `201 Created` response code and a new [externalConnection](../resources/externalconnectors-externalconnection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7188c-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7188c-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7188c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7188c-132">Request</span></span>

<span data-ttu-id="7188c-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7188c-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7188c-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="7188c-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="7188c-135">C#</span><span class="sxs-lookup"><span data-stu-id="7188c-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-connection-from-external-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7188c-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7188c-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-connection-from-external-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7188c-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7188c-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-connection-from-external-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7188c-138">Java</span><span class="sxs-lookup"><span data-stu-id="7188c-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-connection-from-external-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="7188c-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="7188c-139">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="7188c-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7188c-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnectors.externalConnection"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "contosohr",
  "name": "Contoso HR",
  "description": "Connection to index Contoso HR system",
  "state": "draft",
  "configuration": {
    "authorizedAppIds": [
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


