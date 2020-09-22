---
title: Excluir personInterest
description: Exclua o objeto personInterest do perfil de um usuário.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 4143d9ab789052dc92502a12a45aa37977756339
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48036181"
---
# <a name="delete-personinterest"></a><span data-ttu-id="5cabd-103">Excluir personInterest</span><span class="sxs-lookup"><span data-stu-id="5cabd-103">Delete personInterest</span></span>

<span data-ttu-id="5cabd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5cabd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5cabd-105">Exclui um objeto [personInterest](../resources/personinterest.md) do [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="5cabd-105">Deletes a [personInterest](../resources/personinterest.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5cabd-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5cabd-106">Permissions</span></span>

<span data-ttu-id="5cabd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5cabd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5cabd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5cabd-109">Permission type</span></span>                        | <span data-ttu-id="5cabd-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5cabd-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5cabd-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5cabd-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5cabd-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="5cabd-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="5cabd-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5cabd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5cabd-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="5cabd-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="5cabd-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5cabd-115">Application</span></span>                            | <span data-ttu-id="5cabd-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5cabd-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="5cabd-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5cabd-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/interests/{id}
DELETE /users/{id | userPrincipalName}/profile/interests/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5cabd-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5cabd-118">Request headers</span></span>

| <span data-ttu-id="5cabd-119">Nome</span><span class="sxs-lookup"><span data-stu-id="5cabd-119">Name</span></span>           |<span data-ttu-id="5cabd-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5cabd-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="5cabd-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5cabd-121">Authorization</span></span>  | <span data-ttu-id="5cabd-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5cabd-p102">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="5cabd-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5cabd-124">Request body</span></span>

<span data-ttu-id="5cabd-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5cabd-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5cabd-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="5cabd-126">Response</span></span>

<span data-ttu-id="5cabd-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5cabd-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5cabd-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5cabd-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5cabd-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5cabd-130">Request</span></span>

<span data-ttu-id="5cabd-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5cabd-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5cabd-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="5cabd-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_personinterest"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/interests/{id}
```
# <a name="c"></a>[<span data-ttu-id="5cabd-133">C#</span><span class="sxs-lookup"><span data-stu-id="5cabd-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-personinterest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5cabd-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5cabd-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-personinterest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5cabd-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5cabd-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-personinterest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5cabd-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="5cabd-136">Response</span></span>

<span data-ttu-id="5cabd-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5cabd-137">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```


