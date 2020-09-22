---
title: Excluir conta da
description: Excluir um objeto webaccount do perfil de um usuário.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 55e3d63d48b4a1c443eafefc047aad9b9bf23be5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48022054"
---
# <a name="delete-webaccount"></a><span data-ttu-id="463e9-103">Excluir conta da</span><span class="sxs-lookup"><span data-stu-id="463e9-103">Delete webAccount</span></span>

<span data-ttu-id="463e9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="463e9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="463e9-105">Excluir um objeto [webaccount](../resources/webaccount.md) do [perfil](../resources/profile.md)de um usuário.</span><span class="sxs-lookup"><span data-stu-id="463e9-105">Delete a [webAccount](../resources/webaccount.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="463e9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="463e9-106">Permissions</span></span>

<span data-ttu-id="463e9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="463e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="463e9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="463e9-109">Permission type</span></span>                        | <span data-ttu-id="463e9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="463e9-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="463e9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="463e9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="463e9-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="463e9-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="463e9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="463e9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="463e9-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="463e9-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="463e9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="463e9-115">Application</span></span>                            | <span data-ttu-id="463e9-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="463e9-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="463e9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="463e9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/webAccounts/{id}
DELETE /users/{id | userPrincipalName}/profile/webAccounts/{id}
```

## <a name="request-headers"></a><span data-ttu-id="463e9-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="463e9-118">Request headers</span></span>

| <span data-ttu-id="463e9-119">Nome</span><span class="sxs-lookup"><span data-stu-id="463e9-119">Name</span></span>           | <span data-ttu-id="463e9-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="463e9-120">Description</span></span>                 |
|:---------------|:----------------------------|
| <span data-ttu-id="463e9-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="463e9-121">Authorization</span></span>  | <span data-ttu-id="463e9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="463e9-p102">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="463e9-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="463e9-124">Request body</span></span>

<span data-ttu-id="463e9-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="463e9-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="463e9-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="463e9-126">Response</span></span>

<span data-ttu-id="463e9-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="463e9-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="463e9-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="463e9-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="463e9-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="463e9-130">Request</span></span>

<span data-ttu-id="463e9-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="463e9-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="463e9-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="463e9-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_webaccount"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/webAccounts/{id}
```
# <a name="c"></a>[<span data-ttu-id="463e9-133">C#</span><span class="sxs-lookup"><span data-stu-id="463e9-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-webaccount-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="463e9-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="463e9-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-webaccount-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="463e9-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="463e9-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-webaccount-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="463e9-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="463e9-136">Response</span></span>

<span data-ttu-id="463e9-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="463e9-137">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```


