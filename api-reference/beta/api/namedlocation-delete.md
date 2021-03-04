---
title: Excluir namedLocation
description: Exclua um objeto namedLocation.
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 6785a3d6e80d19372bf5d935e300fea0e19497e1
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443657"
---
# <a name="delete-namedlocation"></a><span data-ttu-id="382bf-103">Excluir namedLocation</span><span class="sxs-lookup"><span data-stu-id="382bf-103">Delete namedLocation</span></span>

<span data-ttu-id="382bf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="382bf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="382bf-105">Exclua [um objeto namedLocation.](../resources/namedlocation.md)</span><span class="sxs-lookup"><span data-stu-id="382bf-105">Delete a [namedLocation](../resources/namedlocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="382bf-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="382bf-106">Permissions</span></span>

<span data-ttu-id="382bf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="382bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="382bf-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="382bf-109">Permission type</span></span>                        | <span data-ttu-id="382bf-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="382bf-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="382bf-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="382bf-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="382bf-112">Policy.Read.All e Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="382bf-112">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |
| <span data-ttu-id="382bf-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="382bf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="382bf-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="382bf-114">Not supported.</span></span> |
| <span data-ttu-id="382bf-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="382bf-115">Application</span></span>                            | <span data-ttu-id="382bf-116">Policy.Read.All e Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="382bf-116">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |

## <a name="http-request"></a><span data-ttu-id="382bf-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="382bf-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identity/conditionalAccess/namedLocations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="382bf-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="382bf-118">Request headers</span></span>

| <span data-ttu-id="382bf-119">Nome</span><span class="sxs-lookup"><span data-stu-id="382bf-119">Name</span></span>          | <span data-ttu-id="382bf-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="382bf-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="382bf-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="382bf-121">Authorization</span></span> | <span data-ttu-id="382bf-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="382bf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="382bf-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="382bf-124">Request body</span></span>

<span data-ttu-id="382bf-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="382bf-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="382bf-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="382bf-126">Response</span></span>

<span data-ttu-id="382bf-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="382bf-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="382bf-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="382bf-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="382bf-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="382bf-130">Request</span></span>

<span data-ttu-id="382bf-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="382bf-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="382bf-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="382bf-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_namedlocation"
}-->

```http
DELETE https://graph.microsoft.com/beta/identity/conditionalAccess/namedLocations/0854951d-5fc0-4eb1-b392-9b2c9d7949c2
```
# <a name="c"></a>[<span data-ttu-id="382bf-133">C#</span><span class="sxs-lookup"><span data-stu-id="382bf-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-namedlocation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="382bf-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="382bf-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-namedlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="382bf-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="382bf-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-namedlocation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="382bf-136">Java</span><span class="sxs-lookup"><span data-stu-id="382bf-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-namedlocation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="382bf-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="382bf-137">Response</span></span>

<span data-ttu-id="382bf-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="382bf-138">The following is an example of the response.</span></span>

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


