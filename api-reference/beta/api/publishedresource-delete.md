---
title: Excluir publishedResource
description: Excluir um objeto [publishedResource](../resources/publishedresource.md) .
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2b5c520746acc71e99e5297df06f630dde783e56
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36342184"
---
# <a name="delete-publishedresource"></a><span data-ttu-id="ceac5-103">Excluir publishedResource</span><span class="sxs-lookup"><span data-stu-id="ceac5-103">Delete publishedResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ceac5-104">Excluir um objeto [publishedResource](../resources/publishedresource.md) .</span><span class="sxs-lookup"><span data-stu-id="ceac5-104">Delete a [publishedResource](../resources/publishedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ceac5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ceac5-105">Permissions</span></span>

<span data-ttu-id="ceac5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ceac5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ceac5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ceac5-108">Permission type</span></span>                        | <span data-ttu-id="ceac5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ceac5-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="ceac5-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ceac5-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ceac5-111">OnPremisesPublishingProfiles. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ceac5-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="ceac5-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ceac5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ceac5-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ceac5-113">Not supported.</span></span> |
| <span data-ttu-id="ceac5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ceac5-114">Application</span></span>                            | <span data-ttu-id="ceac5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ceac5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ceac5-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ceac5-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE ~/onPremisesPublishingProfiles/{publishingType}/publishedResources/{id1}/agentGroups/{id2}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="ceac5-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ceac5-117">Request headers</span></span>

| <span data-ttu-id="ceac5-118">Nome</span><span class="sxs-lookup"><span data-stu-id="ceac5-118">Name</span></span>          | <span data-ttu-id="ceac5-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="ceac5-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ceac5-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="ceac5-120">Authorization</span></span> | <span data-ttu-id="ceac5-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="ceac5-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ceac5-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ceac5-122">Request body</span></span>

<span data-ttu-id="ceac5-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ceac5-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ceac5-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="ceac5-124">Response</span></span>

<span data-ttu-id="ceac5-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ceac5-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ceac5-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ceac5-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ceac5-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ceac5-128">Request</span></span>

<span data-ttu-id="ceac5-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ceac5-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ceac5-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="ceac5-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_publishedresource"
}-->

```http
DELETE https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/publishedResources/1234b780-965f-4149-85c5-a8c73e58b67d/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/$ref
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ceac5-131">C#</span><span class="sxs-lookup"><span data-stu-id="ceac5-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-publishedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ceac5-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ceac5-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-publishedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ceac5-133">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="ceac5-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-publishedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ceac5-134">Java</span><span class="sxs-lookup"><span data-stu-id="ceac5-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-publishedresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ceac5-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="ceac5-135">Response</span></span>

<span data-ttu-id="ceac5-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ceac5-136">The following is an example of the response.</span></span>

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
