---
title: Excluir publishedResource
description: Excluir um objeto [publishedResource](../resources/publishedresource.md) .
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 74c20ce468392d3dfb380ea9d341f9c0ccf6e9dd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454862"
---
# <a name="delete-publishedresource"></a><span data-ttu-id="6fa0f-103">Excluir publishedResource</span><span class="sxs-lookup"><span data-stu-id="6fa0f-103">Delete publishedResource</span></span>

<span data-ttu-id="6fa0f-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6fa0f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6fa0f-105">Excluir um objeto [publishedResource](../resources/publishedresource.md) .</span><span class="sxs-lookup"><span data-stu-id="6fa0f-105">Delete a [publishedResource](../resources/publishedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6fa0f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6fa0f-106">Permissions</span></span>

<span data-ttu-id="6fa0f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6fa0f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6fa0f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6fa0f-109">Permission type</span></span>                        | <span data-ttu-id="6fa0f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6fa0f-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="6fa0f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6fa0f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6fa0f-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fa0f-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="6fa0f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6fa0f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6fa0f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6fa0f-114">Not supported.</span></span> |
| <span data-ttu-id="6fa0f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6fa0f-115">Application</span></span>                            | <span data-ttu-id="6fa0f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6fa0f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6fa0f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6fa0f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE ~/onPremisesPublishingProfiles/{publishingType}/publishedResources/{id1}/agentGroups/{id2}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="6fa0f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6fa0f-118">Request headers</span></span>

| <span data-ttu-id="6fa0f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6fa0f-119">Name</span></span>          | <span data-ttu-id="6fa0f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6fa0f-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="6fa0f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6fa0f-121">Authorization</span></span> | <span data-ttu-id="6fa0f-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="6fa0f-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="6fa0f-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6fa0f-123">Request body</span></span>

<span data-ttu-id="6fa0f-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6fa0f-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6fa0f-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="6fa0f-125">Response</span></span>

<span data-ttu-id="6fa0f-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6fa0f-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6fa0f-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6fa0f-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6fa0f-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6fa0f-129">Request</span></span>

<span data-ttu-id="6fa0f-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6fa0f-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6fa0f-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="6fa0f-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_publishedresource"
}-->

```http
DELETE https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/publishedResources/1234b780-965f-4149-85c5-a8c73e58b67d/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/$ref
```
# <a name="c"></a>[<span data-ttu-id="6fa0f-132">C#</span><span class="sxs-lookup"><span data-stu-id="6fa0f-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-publishedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6fa0f-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6fa0f-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-publishedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6fa0f-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6fa0f-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-publishedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6fa0f-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="6fa0f-135">Response</span></span>

<span data-ttu-id="6fa0f-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6fa0f-136">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete publishedResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
