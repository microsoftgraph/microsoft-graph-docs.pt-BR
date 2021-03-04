---
title: Excluir userAccountInformation
description: Exclua um objeto userAccountInformation.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 9f922b7ed4f55b6f7a4ad4b80b6b0c9bb2125052
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433494"
---
# <a name="delete-useraccountinformation"></a><span data-ttu-id="d1dd3-103">Excluir userAccountInformation</span><span class="sxs-lookup"><span data-stu-id="d1dd3-103">Delete userAccountInformation</span></span>

<span data-ttu-id="d1dd3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1dd3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1dd3-105">[Exclua um objeto userAccountInformation](../resources/useraccountinformation.md) do perfil de um [usuário.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="d1dd3-105">Delete an [userAccountInformation](../resources/useraccountinformation.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d1dd3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d1dd3-106">Permissions</span></span>

<span data-ttu-id="d1dd3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1dd3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d1dd3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d1dd3-109">Permission type</span></span>                        | <span data-ttu-id="d1dd3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d1dd3-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d1dd3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d1dd3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d1dd3-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1dd3-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="d1dd3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d1dd3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1dd3-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1dd3-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="d1dd3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d1dd3-115">Application</span></span>                            | <span data-ttu-id="d1dd3-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1dd3-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="d1dd3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d1dd3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/profile/account/{id}
DELETE /users/{id | userPrincipalName}/profile/account/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d1dd3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d1dd3-118">Request headers</span></span>

| <span data-ttu-id="d1dd3-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d1dd3-119">Name</span></span>           | <span data-ttu-id="d1dd3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1dd3-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="d1dd3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d1dd3-121">Authorization</span></span>  | <span data-ttu-id="d1dd3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d1dd3-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d1dd3-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d1dd3-124">Request body</span></span>

<span data-ttu-id="d1dd3-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d1dd3-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1dd3-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1dd3-126">Response</span></span>

<span data-ttu-id="d1dd3-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d1dd3-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d1dd3-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d1dd3-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d1dd3-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d1dd3-130">Request</span></span>

<span data-ttu-id="d1dd3-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d1dd3-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d1dd3-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="d1dd3-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_useraccountinformation"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/profile/account/{id}
```
# <a name="c"></a>[<span data-ttu-id="d1dd3-133">C#</span><span class="sxs-lookup"><span data-stu-id="d1dd3-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-useraccountinformation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d1dd3-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d1dd3-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-useraccountinformation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d1dd3-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d1dd3-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-useraccountinformation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d1dd3-136">Java</span><span class="sxs-lookup"><span data-stu-id="d1dd3-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-useraccountinformation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d1dd3-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1dd3-137">Response</span></span>

<span data-ttu-id="d1dd3-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d1dd3-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

