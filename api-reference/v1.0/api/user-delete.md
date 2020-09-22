---
title: Excluir um usuário - Microsoft Graph API
description: Descreve o método de exclusão de recursos do usuário (entidade) do Microsoft Graph API (REST).
author: krbain
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: b4ecb9ebf2b022ebdddd41e5b63595b55ca49154
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037945"
---
# <a name="delete-a-user"></a><span data-ttu-id="94fc6-103">Excluir um usuário</span><span class="sxs-lookup"><span data-stu-id="94fc6-103">Delete a user</span></span>

<span data-ttu-id="94fc6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94fc6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="94fc6-105">Excluir usuário.</span><span class="sxs-lookup"><span data-stu-id="94fc6-105">Delete user.</span></span>  

<span data-ttu-id="94fc6-106">Quando excluído, os recursos do usuário são movidos para um contêiner temporário e poderá ser restaurados dentro de 30 dias.</span><span class="sxs-lookup"><span data-stu-id="94fc6-106">When deleted, user resources are moved to a temporary container and can be restored within 30 days.</span></span>  <span data-ttu-id="94fc6-107">Após esse período, elas serão permanentemente excluídos.</span><span class="sxs-lookup"><span data-stu-id="94fc6-107">After that time, they are permanently deleted.</span></span>  <span data-ttu-id="94fc6-108">Para saber mais, confira [deletedItems](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="94fc6-108">To learn more, see [deletedItems](../resources/directory.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="94fc6-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="94fc6-109">Permissions</span></span>

<span data-ttu-id="94fc6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94fc6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94fc6-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94fc6-112">Permission type</span></span>      | <span data-ttu-id="94fc6-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="94fc6-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94fc6-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94fc6-114">Delegated (work or school account)</span></span> | <span data-ttu-id="94fc6-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="94fc6-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="94fc6-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="94fc6-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94fc6-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94fc6-117">Not supported.</span></span>    |
|<span data-ttu-id="94fc6-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="94fc6-118">Application</span></span> | <span data-ttu-id="94fc6-119">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94fc6-119">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="94fc6-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="94fc6-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="94fc6-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="94fc6-121">Request headers</span></span>

| <span data-ttu-id="94fc6-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="94fc6-122">Header</span></span>       | <span data-ttu-id="94fc6-123">Valor</span><span class="sxs-lookup"><span data-stu-id="94fc6-123">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="94fc6-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="94fc6-124">Authorization</span></span>  | <span data-ttu-id="94fc6-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94fc6-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="94fc6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="94fc6-127">Request body</span></span>

<span data-ttu-id="94fc6-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="94fc6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94fc6-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="94fc6-129">Response</span></span>

<span data-ttu-id="94fc6-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94fc6-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94fc6-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="94fc6-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="94fc6-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94fc6-133">Request</span></span>

<span data-ttu-id="94fc6-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="94fc6-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="94fc6-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="94fc6-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_user"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/users/{user-id}
```
# <a name="c"></a>[<span data-ttu-id="94fc6-136">C#</span><span class="sxs-lookup"><span data-stu-id="94fc6-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="94fc6-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94fc6-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="94fc6-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="94fc6-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="94fc6-139">Java</span><span class="sxs-lookup"><span data-stu-id="94fc6-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="94fc6-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="94fc6-140">Response</span></span>

<span data-ttu-id="94fc6-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94fc6-141">Here is an example of the response.</span></span> 
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

