---
title: Excluir workPosition
description: Excluir um objeto workPosition do perfil de um usuário.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 372c1518a7c7c6e63d0671b13175b75418003b1d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48977356"
---
# <a name="delete-workposition"></a><span data-ttu-id="cf1a6-103">Excluir workPosition</span><span class="sxs-lookup"><span data-stu-id="cf1a6-103">Delete workPosition</span></span>

<span data-ttu-id="cf1a6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf1a6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf1a6-105">Excluir um objeto [workPosition](../resources/workposition.md) específico do [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="cf1a6-105">Delete a specific [workPosition](../resources/workposition.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cf1a6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cf1a6-106">Permissions</span></span>

<span data-ttu-id="cf1a6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf1a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cf1a6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cf1a6-109">Permission type</span></span>                        | <span data-ttu-id="cf1a6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cf1a6-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cf1a6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cf1a6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cf1a6-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="cf1a6-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="cf1a6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cf1a6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf1a6-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="cf1a6-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="cf1a6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cf1a6-115">Application</span></span>                            | <span data-ttu-id="cf1a6-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf1a6-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="cf1a6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cf1a6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/positions/{id}
DELETE /users/{id | userPrincipalName}/profile/positions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="cf1a6-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cf1a6-118">Request headers</span></span>

| <span data-ttu-id="cf1a6-119">Nome</span><span class="sxs-lookup"><span data-stu-id="cf1a6-119">Name</span></span>           |<span data-ttu-id="cf1a6-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf1a6-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="cf1a6-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="cf1a6-121">Authorization</span></span>  | <span data-ttu-id="cf1a6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cf1a6-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="cf1a6-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cf1a6-124">Content-Type</span></span>   | <span data-ttu-id="cf1a6-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cf1a6-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="cf1a6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cf1a6-127">Request body</span></span>

<span data-ttu-id="cf1a6-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cf1a6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf1a6-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf1a6-129">Response</span></span>

<span data-ttu-id="cf1a6-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cf1a6-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cf1a6-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="cf1a6-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cf1a6-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cf1a6-133">Request</span></span>

<span data-ttu-id="cf1a6-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cf1a6-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cf1a6-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="cf1a6-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_workposition"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/positions/{id}
```
# <a name="c"></a>[<span data-ttu-id="cf1a6-136">C#</span><span class="sxs-lookup"><span data-stu-id="cf1a6-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-workposition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cf1a6-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cf1a6-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-workposition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cf1a6-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cf1a6-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-workposition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cf1a6-139">Java</span><span class="sxs-lookup"><span data-stu-id="cf1a6-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-workposition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cf1a6-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf1a6-140">Response</span></span>

<span data-ttu-id="cf1a6-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cf1a6-141">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```


