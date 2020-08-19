---
title: Excluir skillProficiency
description: Exclua skillProficiency.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 501eb80a9ab304579920d7f615a6a08b5a764577
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811151"
---
# <a name="delete-skillproficiency"></a><span data-ttu-id="38fed-103">Excluir skillProficiency</span><span class="sxs-lookup"><span data-stu-id="38fed-103">Delete skillProficiency</span></span>

<span data-ttu-id="38fed-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38fed-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38fed-105">Excluir um objeto [skillProficiency](../resources/skillproficiency.md) do [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="38fed-105">Delete a [skillProficiency](../resources/skillproficiency.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="38fed-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="38fed-106">Permissions</span></span>

<span data-ttu-id="38fed-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38fed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="38fed-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="38fed-109">Permission type</span></span>                        | <span data-ttu-id="38fed-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="38fed-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="38fed-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="38fed-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="38fed-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="38fed-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="38fed-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="38fed-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38fed-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="38fed-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="38fed-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="38fed-115">Application</span></span>                            | <span data-ttu-id="38fed-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38fed-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="38fed-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="38fed-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/skills/{id}
DELETE /users/{id | userPrincipalName}/profile/skills/{id}
```

## <a name="request-headers"></a><span data-ttu-id="38fed-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="38fed-118">Request headers</span></span>

| <span data-ttu-id="38fed-119">Nome</span><span class="sxs-lookup"><span data-stu-id="38fed-119">Name</span></span>           |<span data-ttu-id="38fed-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="38fed-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="38fed-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="38fed-121">Authorization</span></span>  | <span data-ttu-id="38fed-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38fed-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="38fed-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="38fed-124">Content-Type</span></span>   | <span data-ttu-id="38fed-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38fed-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="38fed-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="38fed-127">Request body</span></span>

<span data-ttu-id="38fed-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="38fed-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38fed-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="38fed-129">Response</span></span>

<span data-ttu-id="38fed-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="38fed-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="38fed-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="38fed-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="38fed-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="38fed-133">Request</span></span>

<span data-ttu-id="38fed-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="38fed-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="38fed-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="38fed-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_skillproficiency"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/skills/{id}
```
# <a name="c"></a>[<span data-ttu-id="38fed-136">C#</span><span class="sxs-lookup"><span data-stu-id="38fed-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-skillproficiency-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="38fed-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="38fed-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-skillproficiency-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="38fed-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="38fed-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-skillproficiency-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="38fed-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="38fed-139">Response</span></span>

<span data-ttu-id="38fed-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="38fed-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
