---
title: Excluir languageProficiency
description: Excluir um objeto languageProficiency do perfil de um usuário.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: aa3e9e08733e76f170940c5004680a4e37443655
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47999311"
---
# <a name="delete-languageproficiency"></a><span data-ttu-id="e7610-103">Excluir languageProficiency</span><span class="sxs-lookup"><span data-stu-id="e7610-103">Delete languageProficiency</span></span>

<span data-ttu-id="e7610-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7610-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7610-105">Excluir um objeto [languageProficiency](../resources/languageproficiency.md) do [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="e7610-105">Delete a [languageProficiency](../resources/languageproficiency.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e7610-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e7610-106">Permissions</span></span>

<span data-ttu-id="e7610-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7610-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e7610-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e7610-109">Permission type</span></span>                        | <span data-ttu-id="e7610-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e7610-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e7610-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e7610-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e7610-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e7610-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="e7610-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e7610-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7610-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e7610-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="e7610-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e7610-115">Application</span></span>                            | <span data-ttu-id="e7610-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7610-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="e7610-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e7610-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/languages/{id}
DELETE /users/{id | userPrincipalName}/profile/languages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e7610-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e7610-118">Request headers</span></span>

| <span data-ttu-id="e7610-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e7610-119">Name</span></span>           |<span data-ttu-id="e7610-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7610-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="e7610-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e7610-121">Authorization</span></span>  | <span data-ttu-id="e7610-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7610-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="e7610-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e7610-124">Content-Type</span></span>   | <span data-ttu-id="e7610-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7610-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e7610-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e7610-127">Request body</span></span>

<span data-ttu-id="e7610-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e7610-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7610-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7610-129">Response</span></span>

<span data-ttu-id="e7610-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e7610-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e7610-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e7610-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e7610-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7610-133">Request</span></span>

<span data-ttu-id="e7610-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e7610-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e7610-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="e7610-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_languageproficiency"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/languages/{id}
```
# <a name="c"></a>[<span data-ttu-id="e7610-136">C#</span><span class="sxs-lookup"><span data-stu-id="e7610-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-languageproficiency-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e7610-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e7610-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-languageproficiency-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e7610-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e7610-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-languageproficiency-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="e7610-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7610-139">Response</span></span>

<span data-ttu-id="e7610-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e7610-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```


