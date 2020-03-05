---
title: Excluir namedLocation
description: Excluir um objeto namedLocation.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 44c8144476dfec7dae9563bd77ae467dc549110c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456779"
---
# <a name="delete-namedlocation"></a><span data-ttu-id="22bbc-103">Excluir namedLocation</span><span class="sxs-lookup"><span data-stu-id="22bbc-103">Delete namedLocation</span></span>

<span data-ttu-id="22bbc-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="22bbc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22bbc-105">Excluir um objeto [namedLocation](../resources/namedlocation.md) .</span><span class="sxs-lookup"><span data-stu-id="22bbc-105">Delete a [namedLocation](../resources/namedlocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="22bbc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="22bbc-106">Permissions</span></span>

<span data-ttu-id="22bbc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22bbc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="22bbc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="22bbc-109">Permission type</span></span>                        | <span data-ttu-id="22bbc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="22bbc-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="22bbc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="22bbc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="22bbc-112">Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="22bbc-112">Policy.ReadWrite.ConditionalAccess</span></span> |
| <span data-ttu-id="22bbc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="22bbc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22bbc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22bbc-114">Not supported.</span></span> |
| <span data-ttu-id="22bbc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="22bbc-115">Application</span></span>                            | <span data-ttu-id="22bbc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22bbc-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="22bbc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="22bbc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /conditionalAccess/namedLocations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="22bbc-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="22bbc-118">Request headers</span></span>

| <span data-ttu-id="22bbc-119">Nome</span><span class="sxs-lookup"><span data-stu-id="22bbc-119">Name</span></span>          | <span data-ttu-id="22bbc-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="22bbc-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="22bbc-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="22bbc-121">Authorization</span></span> | <span data-ttu-id="22bbc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="22bbc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="22bbc-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="22bbc-124">Request body</span></span>

<span data-ttu-id="22bbc-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="22bbc-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22bbc-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="22bbc-126">Response</span></span>

<span data-ttu-id="22bbc-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="22bbc-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="22bbc-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="22bbc-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="22bbc-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="22bbc-130">Request</span></span>

<span data-ttu-id="22bbc-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="22bbc-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="22bbc-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="22bbc-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_namedlocation"
}-->

```http
DELETE https://graph.microsoft.com/beta/conditionalAccess/namedLocations/0854951d-5fc0-4eb1-b392-9b2c9d7949c2
```
# <a name="c"></a>[<span data-ttu-id="22bbc-133">C#</span><span class="sxs-lookup"><span data-stu-id="22bbc-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-namedlocation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="22bbc-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="22bbc-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-namedlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="22bbc-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="22bbc-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-namedlocation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="22bbc-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="22bbc-136">Response</span></span>

<span data-ttu-id="22bbc-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="22bbc-137">The following is an example of the response.</span></span>

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
  "description": "Delete namedLocation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
