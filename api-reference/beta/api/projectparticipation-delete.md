---
title: Excluir projectParticipation
description: Exclua o objeto projectParticipation do perfil de um usuário.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 84ce60da7c06768f076af4771b7a99411cd55d25
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47986205"
---
# <a name="delete-projectparticipation"></a><span data-ttu-id="54969-103">Excluir projectParticipation</span><span class="sxs-lookup"><span data-stu-id="54969-103">Delete projectParticipation</span></span>

<span data-ttu-id="54969-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54969-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54969-105">Excluir um objeto [projectParticipation](../resources/projectparticipation.md) do [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="54969-105">Delete a [projectParticipation](../resources/projectparticipation.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="54969-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="54969-106">Permissions</span></span>

<span data-ttu-id="54969-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54969-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="54969-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="54969-109">Permission type</span></span>                        | <span data-ttu-id="54969-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="54969-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="54969-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="54969-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="54969-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="54969-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="54969-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="54969-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54969-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="54969-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="54969-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="54969-115">Application</span></span>                            | <span data-ttu-id="54969-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54969-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="54969-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="54969-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/projects/{id}
DELETE /users/{id | userPrincipalName}/profile/projects/{id}
```

## <a name="request-headers"></a><span data-ttu-id="54969-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="54969-118">Request headers</span></span>

| <span data-ttu-id="54969-119">Nome</span><span class="sxs-lookup"><span data-stu-id="54969-119">Name</span></span>           |<span data-ttu-id="54969-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="54969-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="54969-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="54969-121">Authorization</span></span>  | <span data-ttu-id="54969-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="54969-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="54969-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="54969-124">Content-Type</span></span>   | <span data-ttu-id="54969-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="54969-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="54969-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="54969-127">Request body</span></span>

<span data-ttu-id="54969-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="54969-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="54969-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="54969-129">Response</span></span>

<span data-ttu-id="54969-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="54969-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="54969-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="54969-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="54969-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="54969-133">Request</span></span>

<span data-ttu-id="54969-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="54969-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="54969-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="54969-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_projectparticipation"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/projects/{id}
```
# <a name="c"></a>[<span data-ttu-id="54969-136">C#</span><span class="sxs-lookup"><span data-stu-id="54969-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-projectparticipation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="54969-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="54969-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-projectparticipation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="54969-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="54969-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-projectparticipation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="54969-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="54969-139">Response</span></span>

<span data-ttu-id="54969-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="54969-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```


