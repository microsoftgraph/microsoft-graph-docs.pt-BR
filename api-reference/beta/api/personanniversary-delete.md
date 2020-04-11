---
title: Excluir personAnniversary
description: Excluir um objeto personAnniversary do perfil de um usuário.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 0a6d63a32157d888fadfdb800c3f239ea6e92f98
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43228749"
---
# <a name="delete-personanniversary"></a><span data-ttu-id="e1118-103">Excluir personAnniversary</span><span class="sxs-lookup"><span data-stu-id="e1118-103">Delete personAnniversary</span></span>

<span data-ttu-id="e1118-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1118-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1118-105">Excluir um objeto [personAnniversary](../resources/personanniversary.md) do [perfil](../resources/profile.md)do usuário.</span><span class="sxs-lookup"><span data-stu-id="e1118-105">Delete a [personAnniversary](../resources/personanniversary.md) object from the user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e1118-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e1118-106">Permissions</span></span>

<span data-ttu-id="e1118-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1118-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e1118-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1118-109">Permission type</span></span>                        | <span data-ttu-id="e1118-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e1118-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e1118-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1118-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e1118-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e1118-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="e1118-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1118-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1118-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e1118-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="e1118-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e1118-115">Application</span></span>                            | <span data-ttu-id="e1118-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1118-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="e1118-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1118-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/anniversaries/{id} 
```

## <a name="request-headers"></a><span data-ttu-id="e1118-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1118-118">Request headers</span></span>

| <span data-ttu-id="e1118-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e1118-119">Name</span></span>           |<span data-ttu-id="e1118-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1118-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="e1118-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1118-121">Authorization</span></span>  | <span data-ttu-id="e1118-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1118-p102">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="e1118-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1118-124">Request body</span></span>

<span data-ttu-id="e1118-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e1118-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1118-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1118-126">Response</span></span>

<span data-ttu-id="e1118-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1118-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e1118-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e1118-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e1118-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1118-130">Request</span></span>

<span data-ttu-id="e1118-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1118-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e1118-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="e1118-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_personanniversary"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/anniversaries/{id}
```
# <a name="c"></a>[<span data-ttu-id="e1118-133">C#</span><span class="sxs-lookup"><span data-stu-id="e1118-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-personanniversary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e1118-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e1118-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-personanniversary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e1118-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e1118-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-personanniversary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="e1118-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1118-136">Response</span></span>

<span data-ttu-id="e1118-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e1118-137">The following is an example of the response.</span></span>

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
