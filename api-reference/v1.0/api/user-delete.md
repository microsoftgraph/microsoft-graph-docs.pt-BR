---
title: Excluir um usuário - Microsoft Graph API
description: Descreve o método de exclusão de recursos do usuário (entidade) do Microsoft Graph API (REST).
author: krbain
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: ca9cbb2fc392a01db68c61d2b5755a7381d27981
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509599"
---
# <a name="delete-a-user"></a><span data-ttu-id="e6258-103">Excluir um usuário</span><span class="sxs-lookup"><span data-stu-id="e6258-103">Delete a user</span></span>

<span data-ttu-id="e6258-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6258-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e6258-105">Excluir usuário.</span><span class="sxs-lookup"><span data-stu-id="e6258-105">Delete user.</span></span>  

<span data-ttu-id="e6258-106">Quando excluído, os recursos do usuário são movidos para um contêiner temporário e poderá ser restaurados dentro de 30 dias.</span><span class="sxs-lookup"><span data-stu-id="e6258-106">When deleted, user resources are moved to a temporary container and can be restored within 30 days.</span></span>  <span data-ttu-id="e6258-107">Após esse período, elas serão permanentemente excluídos.</span><span class="sxs-lookup"><span data-stu-id="e6258-107">After that time, they are permanently deleted.</span></span>  <span data-ttu-id="e6258-108">Para saber mais, confira [deletedItems](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="e6258-108">To learn more, see [deletedItems](../resources/directory.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e6258-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="e6258-109">Permissions</span></span>

<span data-ttu-id="e6258-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6258-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6258-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e6258-112">Permission type</span></span>      | <span data-ttu-id="e6258-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e6258-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e6258-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e6258-114">Delegated (work or school account)</span></span> | <span data-ttu-id="e6258-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e6258-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e6258-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e6258-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6258-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e6258-117">Not supported.</span></span>    |
|<span data-ttu-id="e6258-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e6258-118">Application</span></span> | <span data-ttu-id="e6258-119">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6258-119">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e6258-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e6258-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="e6258-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e6258-121">Request headers</span></span>

| <span data-ttu-id="e6258-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e6258-122">Header</span></span>       | <span data-ttu-id="e6258-123">Valor</span><span class="sxs-lookup"><span data-stu-id="e6258-123">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="e6258-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e6258-124">Authorization</span></span>  | <span data-ttu-id="e6258-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e6258-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e6258-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e6258-127">Request body</span></span>

<span data-ttu-id="e6258-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e6258-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e6258-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6258-129">Response</span></span>

<span data-ttu-id="e6258-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e6258-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6258-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e6258-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e6258-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e6258-133">Request</span></span>

<span data-ttu-id="e6258-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e6258-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e6258-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="e6258-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_user"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/users/{user-id}
```
# <a name="c"></a>[<span data-ttu-id="e6258-136">C#</span><span class="sxs-lookup"><span data-stu-id="e6258-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e6258-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e6258-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e6258-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e6258-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e6258-139">Java</span><span class="sxs-lookup"><span data-stu-id="e6258-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="e6258-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6258-140">Response</span></span>

<span data-ttu-id="e6258-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e6258-141">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
