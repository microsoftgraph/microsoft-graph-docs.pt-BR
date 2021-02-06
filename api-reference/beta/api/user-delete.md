---
title: Excluir um usuário - Microsoft Graph API
description: Descreve o método de exclusão de recursos do usuário (entidade) do Microsoft Graph API (REST).
author: krbain
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 1c3de475fbe57143478d39dde759ecbad45abf59
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136791"
---
# <a name="delete-a-user"></a><span data-ttu-id="ab1af-103">Excluir um usuário</span><span class="sxs-lookup"><span data-stu-id="ab1af-103">Delete a user</span></span>

<span data-ttu-id="ab1af-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab1af-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab1af-105">Excluir usuário.</span><span class="sxs-lookup"><span data-stu-id="ab1af-105">Delete user.</span></span>  

<span data-ttu-id="ab1af-106">Quando excluído, os recursos do usuário são movidos para um contêiner temporário e poderá ser restaurados dentro de 30 dias.</span><span class="sxs-lookup"><span data-stu-id="ab1af-106">When deleted, user resources are moved to a temporary container and can be restored within 30 days.</span></span>  <span data-ttu-id="ab1af-107">Após esse período, elas serão permanentemente excluídos.</span><span class="sxs-lookup"><span data-stu-id="ab1af-107">After that time, they are permanently deleted.</span></span>  <span data-ttu-id="ab1af-108">Para saber mais, confira [deletedItems](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="ab1af-108">To learn more, see [deletedItems](../resources/directory.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ab1af-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="ab1af-109">Permissions</span></span>

<span data-ttu-id="ab1af-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab1af-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab1af-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ab1af-112">Permission type</span></span>      | <span data-ttu-id="ab1af-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ab1af-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab1af-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ab1af-114">Delegated (work or school account)</span></span> | <span data-ttu-id="ab1af-115">User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ab1af-115">User.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ab1af-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ab1af-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab1af-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ab1af-117">Not supported.</span></span>    |
|<span data-ttu-id="ab1af-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ab1af-118">Application</span></span> | <span data-ttu-id="ab1af-119">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab1af-119">User.ReadWrite.All</span></span> |

<span data-ttu-id="ab1af-120">A conta de trabalho ou de estudante deve estar em uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="ab1af-120">The work or school account must be in one of the following roles:</span></span>
+ <span data-ttu-id="ab1af-121">Administrador Global</span><span class="sxs-lookup"><span data-stu-id="ab1af-121">Global Administrator</span></span>
+ <span data-ttu-id="ab1af-122">Administrador do Usuário</span><span class="sxs-lookup"><span data-stu-id="ab1af-122">User Administrator</span></span>

<span data-ttu-id="ab1af-123">Somente um Administrador Global pode excluir um usuário em uma função de Administrador Global ou _qualquer_ usuário no locatário.</span><span class="sxs-lookup"><span data-stu-id="ab1af-123">Only a Global Administrator can delete a user in a Global Administrator role or _any_ user in the tenant.</span></span> <span data-ttu-id="ab1af-124">Um Administrador de Usuário só pode excluir usuários que não são administradores ou em funções limitadas específicas.</span><span class="sxs-lookup"><span data-stu-id="ab1af-124">A User Administrator can only delete users who are non-administrators or in specific limited roles.</span></span> <span data-ttu-id="ab1af-125">Para obter mais detalhes, consulte [Permissões de função de administrador no Azure AD.](/azure/active-directory/roles/permissions-reference#available-roles)</span><span class="sxs-lookup"><span data-stu-id="ab1af-125">For more details, see [Administrator role permissions in Azure AD](/azure/active-directory/roles/permissions-reference#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="ab1af-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ab1af-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="ab1af-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ab1af-127">Request headers</span></span>

| <span data-ttu-id="ab1af-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ab1af-128">Header</span></span>       | <span data-ttu-id="ab1af-129">Valor</span><span class="sxs-lookup"><span data-stu-id="ab1af-129">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="ab1af-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="ab1af-130">Authorization</span></span>  | <span data-ttu-id="ab1af-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ab1af-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ab1af-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ab1af-133">Request body</span></span>

<span data-ttu-id="ab1af-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ab1af-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab1af-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab1af-135">Response</span></span>

<span data-ttu-id="ab1af-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ab1af-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab1af-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ab1af-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="ab1af-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ab1af-139">Request</span></span>

<span data-ttu-id="ab1af-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ab1af-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ab1af-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="ab1af-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_user"
}-->
```http
DELETE https://graph.microsoft.com/beta/users/ba9a3254-9f18-4209-aeb3-9e42a35b5be4 
```
# <a name="c"></a>[<span data-ttu-id="ab1af-142">C#</span><span class="sxs-lookup"><span data-stu-id="ab1af-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ab1af-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ab1af-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ab1af-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ab1af-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ab1af-145">Java</span><span class="sxs-lookup"><span data-stu-id="ab1af-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="ab1af-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab1af-146">Response</span></span>

<span data-ttu-id="ab1af-147">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ab1af-147">Here is an example of the response.</span></span> 
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


