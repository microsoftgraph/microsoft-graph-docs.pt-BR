---
title: Excluir conta da
description: Excluir um objeto webaccount do perfil de um usuário.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: a7424ce21138eed70a26e358d362dae3c75fcef0
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229070"
---
# <a name="delete-webaccount"></a><span data-ttu-id="83e01-103">Excluir conta da</span><span class="sxs-lookup"><span data-stu-id="83e01-103">Delete webAccount</span></span>

<span data-ttu-id="83e01-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83e01-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83e01-105">Exclua um objeto [webaccount](../resources/webaccount.md) do perfil do usuário.</span><span class="sxs-lookup"><span data-stu-id="83e01-105">Delete a [webAccount](../resources/webaccount.md) object from the user's profile.</span></span>

## <a name="permissions"></a><span data-ttu-id="83e01-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="83e01-106">Permissions</span></span>

<span data-ttu-id="83e01-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83e01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="83e01-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="83e01-109">Permission type</span></span>                        | <span data-ttu-id="83e01-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="83e01-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="83e01-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="83e01-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="83e01-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="83e01-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="83e01-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="83e01-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83e01-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="83e01-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="83e01-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="83e01-115">Application</span></span>                            | <span data-ttu-id="83e01-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83e01-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="83e01-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="83e01-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/webAccounts/{id}
```

## <a name="request-headers"></a><span data-ttu-id="83e01-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="83e01-118">Request headers</span></span>

| <span data-ttu-id="83e01-119">Nome</span><span class="sxs-lookup"><span data-stu-id="83e01-119">Name</span></span>           | <span data-ttu-id="83e01-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="83e01-120">Description</span></span>                 |
|:---------------|:----------------------------|
| <span data-ttu-id="83e01-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="83e01-121">Authorization</span></span>  | <span data-ttu-id="83e01-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="83e01-p102">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="83e01-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="83e01-124">Request body</span></span>

<span data-ttu-id="83e01-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="83e01-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="83e01-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="83e01-126">Response</span></span>

<span data-ttu-id="83e01-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="83e01-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="83e01-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="83e01-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="83e01-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="83e01-130">Request</span></span>

<span data-ttu-id="83e01-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="83e01-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="83e01-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="83e01-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_webaccount"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/webAccounts/{id}
```
# <a name="c"></a>[<span data-ttu-id="83e01-133">C#</span><span class="sxs-lookup"><span data-stu-id="83e01-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-webaccount-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="83e01-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="83e01-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-webaccount-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="83e01-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="83e01-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-webaccount-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="83e01-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="83e01-136">Response</span></span>

<span data-ttu-id="83e01-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="83e01-137">The following is an example of the response.</span></span>

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
  "description": "Delete webAccount",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
