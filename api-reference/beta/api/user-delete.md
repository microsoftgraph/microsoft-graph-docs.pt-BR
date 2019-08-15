---
title: Excluir um usuário - Microsoft Graph API
description: Descreve o método de exclusão de recursos do usuário (entidade) do Microsoft Graph API (REST).
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4ef3d3de7b5c5ade167446b9943859608bacee25
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36409060"
---
# <a name="delete-a-user"></a><span data-ttu-id="19490-103">Excluir um usuário</span><span class="sxs-lookup"><span data-stu-id="19490-103">Delete a user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19490-104">Excluir usuário.</span><span class="sxs-lookup"><span data-stu-id="19490-104">Delete user.</span></span>  

<span data-ttu-id="19490-105">Quando excluído, os recursos do usuário são movidos para um contêiner temporário e poderá ser restaurados dentro de 30 dias.</span><span class="sxs-lookup"><span data-stu-id="19490-105">When deleted, user resources are moved to a temporary container and can be restored within 30 days.</span></span>  <span data-ttu-id="19490-106">Após esse período, elas serão permanentemente excluídos.</span><span class="sxs-lookup"><span data-stu-id="19490-106">After that time, they are permanently deleted.</span></span>  <span data-ttu-id="19490-107">Para saber mais, confira [deletedItems](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="19490-107">To learn more, see [deletedItems](../resources/directory.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="19490-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="19490-108">Permissions</span></span>

<span data-ttu-id="19490-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19490-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19490-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="19490-111">Permission type</span></span>      | <span data-ttu-id="19490-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="19490-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="19490-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="19490-113">Delegated (work or school account)</span></span> | <span data-ttu-id="19490-114">User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="19490-114">User.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="19490-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="19490-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19490-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="19490-116">Not supported.</span></span>    |
|<span data-ttu-id="19490-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="19490-117">Application</span></span> | <span data-ttu-id="19490-118">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19490-118">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="19490-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="19490-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="19490-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="19490-120">Request headers</span></span>

| <span data-ttu-id="19490-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="19490-121">Header</span></span>       | <span data-ttu-id="19490-122">Valor</span><span class="sxs-lookup"><span data-stu-id="19490-122">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="19490-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="19490-123">Authorization</span></span>  | <span data-ttu-id="19490-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="19490-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="19490-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="19490-126">Request body</span></span>

<span data-ttu-id="19490-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="19490-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="19490-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="19490-128">Response</span></span>

<span data-ttu-id="19490-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="19490-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19490-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="19490-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="19490-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="19490-132">Request</span></span>

<span data-ttu-id="19490-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="19490-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="19490-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="19490-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_user"
}-->
```http
DELETE https://graph.microsoft.com/beta/users/ba9a3254-9f18-4209-aeb3-9e42a35b5be4 
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="19490-135">C#</span><span class="sxs-lookup"><span data-stu-id="19490-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="19490-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="19490-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="19490-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="19490-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="19490-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="19490-138">Response</span></span>

<span data-ttu-id="19490-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="19490-139">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
