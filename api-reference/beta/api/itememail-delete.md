---
title: Excluir email
description: Exclua um objeto de email de um perfil de usuário.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: bc1f870054bd2120b8b7c543d2880d30eb52290c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48952463"
---
# <a name="delete-itememail"></a><span data-ttu-id="e0abe-103">Excluir email</span><span class="sxs-lookup"><span data-stu-id="e0abe-103">Delete itemEmail</span></span>

<span data-ttu-id="e0abe-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0abe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0abe-105">Excluir um objeto de [email](../resources/itememail.md) do [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="e0abe-105">Delete an [itemEmail](../resources/itememail.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e0abe-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e0abe-106">Permissions</span></span>

<span data-ttu-id="e0abe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0abe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e0abe-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e0abe-109">Permission type</span></span>                        | <span data-ttu-id="e0abe-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e0abe-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e0abe-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e0abe-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e0abe-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e0abe-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="e0abe-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e0abe-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0abe-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e0abe-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="e0abe-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e0abe-115">Application</span></span>                            | <span data-ttu-id="e0abe-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0abe-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="e0abe-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e0abe-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/emails/{id}
DELETE /users/{id | userPrincipalName}/profile/emails/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e0abe-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e0abe-118">Request headers</span></span>

| <span data-ttu-id="e0abe-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e0abe-119">Name</span></span>           |<span data-ttu-id="e0abe-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0abe-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="e0abe-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e0abe-121">Authorization</span></span>  | <span data-ttu-id="e0abe-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e0abe-p102">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="e0abe-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e0abe-124">Request body</span></span>

<span data-ttu-id="e0abe-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e0abe-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e0abe-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0abe-126">Response</span></span>

<span data-ttu-id="e0abe-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e0abe-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e0abe-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e0abe-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e0abe-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e0abe-130">Request</span></span>

<span data-ttu-id="e0abe-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e0abe-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e0abe-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="e0abe-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_itememail"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/emails/{id}
```

# <a name="c"></a>[<span data-ttu-id="e0abe-133">C#</span><span class="sxs-lookup"><span data-stu-id="e0abe-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-itememail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e0abe-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e0abe-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-itememail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e0abe-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e0abe-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-itememail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e0abe-136">Java</span><span class="sxs-lookup"><span data-stu-id="e0abe-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-itememail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="e0abe-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0abe-137">Response</span></span>

<span data-ttu-id="e0abe-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e0abe-138">The following is an example of the response.</span></span>

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
  "description": "Delete itemEmail",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


