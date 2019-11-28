---
title: Excluir ipNamedLocation
description: Excluir um objeto ipNamedLocation.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 914475879a47b008b04955991a7d0c7e8f89e152
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636852"
---
# <a name="delete-ipnamedlocation"></a><span data-ttu-id="a89ea-103">Excluir ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="a89ea-103">Delete ipNamedLocation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a89ea-104">Excluir um objeto [ipNamedLocation](../resources/ipNamedLocation.md) .</span><span class="sxs-lookup"><span data-stu-id="a89ea-104">Delete an [ipNamedLocation](../resources/ipNamedLocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a89ea-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a89ea-105">Permissions</span></span>

<span data-ttu-id="a89ea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a89ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a89ea-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a89ea-108">Permission type</span></span>                        | <span data-ttu-id="a89ea-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a89ea-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a89ea-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a89ea-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a89ea-111">Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="a89ea-111">Policy.ReadWrite.ConditionalAccess</span></span> |
| <span data-ttu-id="a89ea-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a89ea-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a89ea-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a89ea-113">Not supported.</span></span> |
| <span data-ttu-id="a89ea-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a89ea-114">Application</span></span>                            | <span data-ttu-id="a89ea-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a89ea-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a89ea-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a89ea-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /conditionalAccess/namedLocations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a89ea-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a89ea-117">Request headers</span></span>

| <span data-ttu-id="a89ea-118">Nome</span><span class="sxs-lookup"><span data-stu-id="a89ea-118">Name</span></span>          | <span data-ttu-id="a89ea-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="a89ea-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a89ea-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="a89ea-120">Authorization</span></span> | <span data-ttu-id="a89ea-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a89ea-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a89ea-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a89ea-123">Request body</span></span>

<span data-ttu-id="a89ea-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a89ea-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a89ea-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="a89ea-125">Response</span></span>

<span data-ttu-id="a89ea-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a89ea-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a89ea-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a89ea-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a89ea-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a89ea-129">Request</span></span>

<span data-ttu-id="a89ea-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a89ea-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a89ea-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="a89ea-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_ipnamedlocation"
}-->

```http
DELETE https://graph.microsoft.com/beta/conditionalAccess/namedLocations/0854951d-5fc0-4eb1-b392-9b2c9d7949c2
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a89ea-132">C#</span><span class="sxs-lookup"><span data-stu-id="a89ea-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-ipnamedlocation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a89ea-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a89ea-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-ipnamedlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a89ea-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a89ea-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-ipnamedlocation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a89ea-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="a89ea-135">Response</span></span>

<span data-ttu-id="a89ea-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a89ea-136">The following is an example of the response.</span></span>

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
  "description": "Delete ipNamedLocation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
