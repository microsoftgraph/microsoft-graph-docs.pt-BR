---
title: Excluir publishedResource
description: Excluir um objeto [publishedResource](../resources/publishedresource.md) .
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0e1079c21fe1f33dca424a4d6a374f02baa86563
ms.sourcegitcommit: ee41ba9ec6001716f1a9d575741bbeef577e2473
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/09/2020
ms.locfileid: "43200177"
---
# <a name="delete-publishedresource"></a><span data-ttu-id="b757c-103">Excluir publishedResource</span><span class="sxs-lookup"><span data-stu-id="b757c-103">Delete publishedResource</span></span>

<span data-ttu-id="b757c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b757c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b757c-105">Excluir um objeto [publishedResource](../resources/publishedresource.md) .</span><span class="sxs-lookup"><span data-stu-id="b757c-105">Delete a [publishedResource](../resources/publishedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b757c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b757c-106">Permissions</span></span>

<span data-ttu-id="b757c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b757c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b757c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b757c-109">Permission type</span></span>                        | <span data-ttu-id="b757c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b757c-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="b757c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b757c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b757c-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b757c-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="b757c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b757c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b757c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b757c-114">Not supported.</span></span> |
| <span data-ttu-id="b757c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b757c-115">Application</span></span>                            | <span data-ttu-id="b757c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b757c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b757c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b757c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE ~/onPremisesPublishingProfiles/{publishingType}/publishedResources/{id1}/agentGroups/{id2}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="b757c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b757c-118">Request headers</span></span>

| <span data-ttu-id="b757c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b757c-119">Name</span></span>          | <span data-ttu-id="b757c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b757c-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b757c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b757c-121">Authorization</span></span> | <span data-ttu-id="b757c-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="b757c-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="b757c-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b757c-123">Request body</span></span>

<span data-ttu-id="b757c-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b757c-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b757c-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="b757c-125">Response</span></span>

<span data-ttu-id="b757c-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b757c-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b757c-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b757c-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b757c-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b757c-129">Request</span></span>

<span data-ttu-id="b757c-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b757c-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b757c-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="b757c-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_publishedresource"
}-->

```http
DELETE https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/publishedResources/1234b780-965f-4149-85c5-a8c73e58b67d/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/$ref
```
# <a name="c"></a>[<span data-ttu-id="b757c-132">C#</span><span class="sxs-lookup"><span data-stu-id="b757c-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-publishedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b757c-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b757c-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-publishedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b757c-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b757c-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-publishedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b757c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="b757c-135">Response</span></span>

<span data-ttu-id="b757c-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b757c-136">The following is an example of the response.</span></span>

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
