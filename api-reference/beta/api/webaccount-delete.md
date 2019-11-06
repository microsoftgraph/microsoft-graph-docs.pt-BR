---
title: Excluir conta da
description: Excluir um objeto webaccount do perfil de um usuário.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: c895c0564cc14036aa72944a3d498b2a76d6cf4b
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37996204"
---
# <a name="delete-webaccount"></a><span data-ttu-id="deffd-103">Excluir conta da</span><span class="sxs-lookup"><span data-stu-id="deffd-103">Delete webAccount</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="deffd-104">Exclua um objeto [webaccount](../resources/webaccount.md) do perfil do usuário.</span><span class="sxs-lookup"><span data-stu-id="deffd-104">Delete a [webAccount](../resources/webaccount.md) object from the user's profile.</span></span>

## <a name="permissions"></a><span data-ttu-id="deffd-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="deffd-105">Permissions</span></span>

<span data-ttu-id="deffd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="deffd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="deffd-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="deffd-108">Permission type</span></span>                        | <span data-ttu-id="deffd-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="deffd-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="deffd-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="deffd-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="deffd-111">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="deffd-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="deffd-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="deffd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="deffd-113">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="deffd-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="deffd-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="deffd-114">Application</span></span>                            | <span data-ttu-id="deffd-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="deffd-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="deffd-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="deffd-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/webAccounts/{id}
```

## <a name="request-headers"></a><span data-ttu-id="deffd-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="deffd-117">Request headers</span></span>

| <span data-ttu-id="deffd-118">Nome</span><span class="sxs-lookup"><span data-stu-id="deffd-118">Name</span></span>           |<span data-ttu-id="deffd-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="deffd-119">Description</span></span>                 |
|:---------------|:---------------------------|
| <span data-ttu-id="deffd-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="deffd-120">Authorization</span></span>  | <span data-ttu-id="deffd-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="deffd-p102">Bearer {token}. Required.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="deffd-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="deffd-123">Request body</span></span>

<span data-ttu-id="deffd-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="deffd-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="deffd-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="deffd-125">Response</span></span>

<span data-ttu-id="deffd-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="deffd-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="deffd-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="deffd-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="deffd-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="deffd-129">Request</span></span>

<span data-ttu-id="deffd-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="deffd-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="deffd-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="deffd-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_webaccount"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/webAccounts/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="deffd-132">C#</span><span class="sxs-lookup"><span data-stu-id="deffd-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-webaccount-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="deffd-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="deffd-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-webaccount-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="deffd-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="deffd-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-webaccount-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="deffd-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="deffd-135">Response</span></span>

<span data-ttu-id="deffd-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="deffd-136">The following is an example of the response.</span></span>

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
