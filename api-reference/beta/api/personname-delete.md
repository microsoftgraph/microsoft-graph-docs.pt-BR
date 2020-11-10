---
title: Excluir PersonName
description: Exclua o objeto PersonName do perfil de um usuário.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 4716679cd69eccd3f59f1eec4ea4cc4b464b7f23
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48975011"
---
# <a name="delete-personname"></a><span data-ttu-id="ab26d-103">Excluir PersonName</span><span class="sxs-lookup"><span data-stu-id="ab26d-103">Delete personName</span></span>

<span data-ttu-id="ab26d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab26d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab26d-105">Excluir um objeto [PersonName](../resources/personname.md) do [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="ab26d-105">Delete a [personName](../resources/personname.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ab26d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ab26d-106">Permissions</span></span>

<span data-ttu-id="ab26d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab26d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ab26d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ab26d-109">Permission type</span></span>                        | <span data-ttu-id="ab26d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ab26d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ab26d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ab26d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ab26d-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ab26d-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="ab26d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ab26d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab26d-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ab26d-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="ab26d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ab26d-115">Application</span></span>                            | <span data-ttu-id="ab26d-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab26d-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="ab26d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ab26d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/names/{id}
DELETE /users/{id | userPrincipalName}/profile/names/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ab26d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ab26d-118">Request headers</span></span>

| <span data-ttu-id="ab26d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ab26d-119">Name</span></span>           |<span data-ttu-id="ab26d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab26d-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="ab26d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ab26d-121">Authorization</span></span>  | <span data-ttu-id="ab26d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ab26d-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="ab26d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ab26d-124">Content-Type</span></span>   | <span data-ttu-id="ab26d-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ab26d-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ab26d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ab26d-127">Request body</span></span>

<span data-ttu-id="ab26d-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ab26d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab26d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab26d-129">Response</span></span>

<span data-ttu-id="ab26d-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ab26d-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ab26d-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ab26d-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ab26d-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ab26d-133">Request</span></span>

<span data-ttu-id="ab26d-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ab26d-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ab26d-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="ab26d-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_personname"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/names/{id}
```
# <a name="c"></a>[<span data-ttu-id="ab26d-136">C#</span><span class="sxs-lookup"><span data-stu-id="ab26d-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-personname-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ab26d-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ab26d-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-personname-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ab26d-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ab26d-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-personname-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ab26d-139">Java</span><span class="sxs-lookup"><span data-stu-id="ab26d-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-personname-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="ab26d-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab26d-140">Response</span></span>

<span data-ttu-id="ab26d-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ab26d-141">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```


