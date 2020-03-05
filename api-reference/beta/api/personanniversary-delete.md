---
title: Excluir personAnniversary
description: Excluir um objeto personAnniversary do perfil de um usuário.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: e11372e158c6f35d53fa48dab301e972323b4ca7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455927"
---
# <a name="delete-personanniversary"></a><span data-ttu-id="b8141-103">Excluir personAnniversary</span><span class="sxs-lookup"><span data-stu-id="b8141-103">Delete personAnniversary</span></span>

<span data-ttu-id="b8141-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b8141-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8141-105">Excluir um objeto [personAnniversary](../resources/personanniversary.md) do [perfil](../resources/profile.md)do usuário.</span><span class="sxs-lookup"><span data-stu-id="b8141-105">Delete a [personAnniversary](../resources/personanniversary.md) object from the user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b8141-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b8141-106">Permissions</span></span>

<span data-ttu-id="b8141-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8141-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b8141-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8141-109">Permission type</span></span>                        | <span data-ttu-id="b8141-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b8141-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b8141-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8141-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b8141-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b8141-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="b8141-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8141-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8141-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b8141-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="b8141-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b8141-115">Application</span></span>                            | <span data-ttu-id="b8141-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8141-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="b8141-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8141-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/anniversaries/{id} 
```

## <a name="request-headers"></a><span data-ttu-id="b8141-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8141-118">Request headers</span></span>

| <span data-ttu-id="b8141-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b8141-119">Name</span></span>           |<span data-ttu-id="b8141-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8141-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="b8141-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b8141-121">Authorization</span></span>  | <span data-ttu-id="b8141-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8141-p102">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="b8141-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b8141-124">Request body</span></span>

<span data-ttu-id="b8141-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b8141-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8141-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8141-126">Response</span></span>

<span data-ttu-id="b8141-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8141-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b8141-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b8141-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b8141-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b8141-130">Request</span></span>

<span data-ttu-id="b8141-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b8141-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b8141-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="b8141-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_personanniversary"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/anniversaries/{id}
```
# <a name="c"></a>[<span data-ttu-id="b8141-133">C#</span><span class="sxs-lookup"><span data-stu-id="b8141-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-personanniversary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b8141-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b8141-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-personanniversary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b8141-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b8141-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-personanniversary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b8141-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8141-136">Response</span></span>

<span data-ttu-id="b8141-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b8141-137">The following is an example of the response.</span></span>

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
  "description": "Delete personAnniversary",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
