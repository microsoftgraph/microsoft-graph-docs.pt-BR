---
title: Excluir externalConnection
description: Exclua uma externalConnection.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 37b46e3cd6de8a12d6a77106abbe81a8a5da090f
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2021
ms.locfileid: "49943609"
---
# <a name="delete-externalconnection"></a><span data-ttu-id="12926-103">Excluir externalConnection</span><span class="sxs-lookup"><span data-stu-id="12926-103">Delete externalConnection</span></span>

<span data-ttu-id="12926-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12926-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12926-105">[Exclua uma externalConnection](../resources/externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="12926-105">Delete an [externalConnection](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="12926-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="12926-106">Permissions</span></span>

<span data-ttu-id="12926-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12926-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="12926-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="12926-109">Permission type</span></span>                        | <span data-ttu-id="12926-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="12926-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="12926-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="12926-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="12926-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="12926-112">Not supported.</span></span> |
| <span data-ttu-id="12926-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="12926-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12926-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="12926-114">Not supported.</span></span> |
| <span data-ttu-id="12926-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="12926-115">Application</span></span>                            | <span data-ttu-id="12926-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12926-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="12926-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="12926-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /external/connections/{id}
```

## <a name="request-headers"></a><span data-ttu-id="12926-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="12926-118">Request headers</span></span>

| <span data-ttu-id="12926-119">Nome</span><span class="sxs-lookup"><span data-stu-id="12926-119">Name</span></span>          | <span data-ttu-id="12926-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="12926-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="12926-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="12926-121">Authorization</span></span> | <span data-ttu-id="12926-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="12926-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="12926-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="12926-124">Request body</span></span>

<span data-ttu-id="12926-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="12926-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12926-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="12926-126">Response</span></span>

<span data-ttu-id="12926-p103">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="12926-p103">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="12926-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="12926-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="12926-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="12926-130">Request</span></span>

<span data-ttu-id="12926-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="12926-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="12926-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="12926-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_connection"
}-->

```http
DELETE https://graph.microsoft.com/beta/connections/contosohr
```
# <a name="c"></a>[<span data-ttu-id="12926-133">C#</span><span class="sxs-lookup"><span data-stu-id="12926-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-connection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="12926-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="12926-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-connection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="12926-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="12926-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-connection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="12926-136">Java</span><span class="sxs-lookup"><span data-stu-id="12926-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-connection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="12926-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="12926-137">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="12926-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="12926-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete externalConnection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


