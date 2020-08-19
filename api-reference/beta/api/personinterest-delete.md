---
title: Excluir personInterest
description: Exclua o objeto personInterest do perfil de um usuário.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 8362b22678a463bae545a7c32fbfca2fe2f4d88c
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809254"
---
# <a name="delete-personinterest"></a><span data-ttu-id="7908e-103">Excluir personInterest</span><span class="sxs-lookup"><span data-stu-id="7908e-103">Delete personInterest</span></span>

<span data-ttu-id="7908e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7908e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7908e-105">Exclui um objeto [personInterest](../resources/personinterest.md) do [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="7908e-105">Deletes a [personInterest](../resources/personinterest.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7908e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7908e-106">Permissions</span></span>

<span data-ttu-id="7908e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7908e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7908e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7908e-109">Permission type</span></span>                        | <span data-ttu-id="7908e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7908e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7908e-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7908e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7908e-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="7908e-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="7908e-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7908e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7908e-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="7908e-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="7908e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7908e-115">Application</span></span>                            | <span data-ttu-id="7908e-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7908e-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="7908e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7908e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/interests/{id}
DELETE /users/{id | userPrincipalName}/profile/interests/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7908e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7908e-118">Request headers</span></span>

| <span data-ttu-id="7908e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="7908e-119">Name</span></span>           |<span data-ttu-id="7908e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="7908e-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="7908e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7908e-121">Authorization</span></span>  | <span data-ttu-id="7908e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7908e-p102">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="7908e-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7908e-124">Request body</span></span>

<span data-ttu-id="7908e-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7908e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7908e-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="7908e-126">Response</span></span>

<span data-ttu-id="7908e-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7908e-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7908e-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7908e-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7908e-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7908e-130">Request</span></span>

<span data-ttu-id="7908e-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7908e-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7908e-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="7908e-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_personinterest"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/interests/{id}
```
# <a name="c"></a>[<span data-ttu-id="7908e-133">C#</span><span class="sxs-lookup"><span data-stu-id="7908e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-personinterest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7908e-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7908e-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-personinterest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7908e-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7908e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-personinterest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7908e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="7908e-136">Response</span></span>

<span data-ttu-id="7908e-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7908e-137">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
