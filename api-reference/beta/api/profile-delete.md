---
title: Excluir perfil
description: Excluir perfil.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: e70ef31e6eec65520a7d2773b7e86aa76059f406
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455232"
---
# <a name="delete-profile"></a><span data-ttu-id="bd8bb-103">Excluir perfil</span><span class="sxs-lookup"><span data-stu-id="bd8bb-103">Delete profile</span></span>

<span data-ttu-id="bd8bb-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="bd8bb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd8bb-105">Exclua o objeto de [perfil](../resources/profile.md) da conta de um usuário.</span><span class="sxs-lookup"><span data-stu-id="bd8bb-105">Delete [profile](../resources/profile.md) object from a user's account.</span></span>

## <a name="permissions"></a><span data-ttu-id="bd8bb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bd8bb-106">Permissions</span></span>

<span data-ttu-id="bd8bb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd8bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bd8bb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bd8bb-109">Permission type</span></span>                        | <span data-ttu-id="bd8bb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bd8bb-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="bd8bb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bd8bb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bd8bb-112">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="bd8bb-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="bd8bb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bd8bb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd8bb-114">User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="bd8bb-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="bd8bb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bd8bb-115">Application</span></span>                            | <span data-ttu-id="bd8bb-116">User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="bd8bb-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="bd8bb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bd8bb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile
```

## <a name="request-headers"></a><span data-ttu-id="bd8bb-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bd8bb-118">Request headers</span></span>

| <span data-ttu-id="bd8bb-119">Nome</span><span class="sxs-lookup"><span data-stu-id="bd8bb-119">Name</span></span>           |<span data-ttu-id="bd8bb-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd8bb-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="bd8bb-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="bd8bb-121">Authorization</span></span>  | <span data-ttu-id="bd8bb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bd8bb-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="bd8bb-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bd8bb-124">Content-Type</span></span>   | <span data-ttu-id="bd8bb-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bd8bb-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bd8bb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bd8bb-127">Request body</span></span>

<span data-ttu-id="bd8bb-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bd8bb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd8bb-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd8bb-129">Response</span></span>

<span data-ttu-id="bd8bb-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bd8bb-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bd8bb-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="bd8bb-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bd8bb-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bd8bb-133">Request</span></span>

<span data-ttu-id="bd8bb-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bd8bb-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bd8bb-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="bd8bb-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_profile"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile
```
# <a name="c"></a>[<span data-ttu-id="bd8bb-136">C#</span><span class="sxs-lookup"><span data-stu-id="bd8bb-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bd8bb-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bd8bb-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bd8bb-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bd8bb-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bd8bb-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd8bb-139">Response</span></span>

<span data-ttu-id="bd8bb-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bd8bb-140">The following is an example of the response.</span></span>

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
  "description": "Delete profile",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
