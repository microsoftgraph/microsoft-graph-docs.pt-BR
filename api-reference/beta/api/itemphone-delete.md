---
title: Excluir o número de telefone
description: Excluir um objeto MyPhone do perfil de um usuário.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: da4866a6b5c5dbe2a8b0d65a04ae4dd7bccbb4a9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42457237"
---
# <a name="delete-itemphonenumber"></a><span data-ttu-id="7c150-103">Excluir itemPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="7c150-103">Delete itemPhoneNumber</span></span>

<span data-ttu-id="7c150-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7c150-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c150-105">Exclua um objeto [MyPhone](../resources/itemphone.md) do [perfil](../resources/profile.md)do usuário.</span><span class="sxs-lookup"><span data-stu-id="7c150-105">Delete an [itemPhone](../resources/itemphone.md) object from the user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7c150-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7c150-106">Permissions</span></span>

<span data-ttu-id="7c150-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c150-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7c150-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7c150-109">Permission type</span></span>                        | <span data-ttu-id="7c150-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7c150-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7c150-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7c150-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7c150-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="7c150-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="7c150-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7c150-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c150-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="7c150-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="7c150-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7c150-115">Application</span></span>                            | <span data-ttu-id="7c150-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c150-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="7c150-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7c150-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/phones/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7c150-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7c150-118">Request headers</span></span>

| <span data-ttu-id="7c150-119">Nome</span><span class="sxs-lookup"><span data-stu-id="7c150-119">Name</span></span>           |<span data-ttu-id="7c150-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c150-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="7c150-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7c150-121">Authorization</span></span>  | <span data-ttu-id="7c150-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7c150-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="7c150-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7c150-124">Content-Type</span></span>   | <span data-ttu-id="7c150-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7c150-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7c150-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7c150-127">Request body</span></span>

<span data-ttu-id="7c150-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7c150-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7c150-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c150-129">Response</span></span>

<span data-ttu-id="7c150-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7c150-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7c150-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7c150-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7c150-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7c150-133">Request</span></span>

<span data-ttu-id="7c150-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7c150-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7c150-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="7c150-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_itemphone"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/phones/{id}
```
# <a name="c"></a>[<span data-ttu-id="7c150-136">C#</span><span class="sxs-lookup"><span data-stu-id="7c150-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-itemphone-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7c150-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7c150-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-itemphone-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7c150-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7c150-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-itemphone-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7c150-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c150-139">Response</span></span>

<span data-ttu-id="7c150-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7c150-140">The following is an example of the response.</span></span>

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
  "description": "Delete itemPhone",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
