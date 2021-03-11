---
title: Excluir um usuário - Microsoft Graph API
description: Descreve o método de exclusão de recursos do usuário (entidade) do Microsoft Graph API (REST).
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 705899489cb754fac5bbaac17fb75417195a484f
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721765"
---
# <a name="delete-a-user"></a><span data-ttu-id="5313c-103">Excluir um usuário</span><span class="sxs-lookup"><span data-stu-id="5313c-103">Delete a user</span></span>

<span data-ttu-id="5313c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5313c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5313c-105">Excluir usuário.</span><span class="sxs-lookup"><span data-stu-id="5313c-105">Delete user.</span></span>  

<span data-ttu-id="5313c-106">Quando excluído, os recursos do usuário são movidos para um contêiner temporário e poderá ser restaurados dentro de 30 dias.</span><span class="sxs-lookup"><span data-stu-id="5313c-106">When deleted, user resources are moved to a temporary container and can be restored within 30 days.</span></span>  <span data-ttu-id="5313c-107">Após esse período, elas serão permanentemente excluídos.</span><span class="sxs-lookup"><span data-stu-id="5313c-107">After that time, they are permanently deleted.</span></span>  <span data-ttu-id="5313c-108">Para saber mais, confira [deletedItems](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="5313c-108">To learn more, see [deletedItems](../resources/directory.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5313c-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="5313c-109">Permissions</span></span>

<span data-ttu-id="5313c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5313c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5313c-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5313c-112">Permission type</span></span>      | <span data-ttu-id="5313c-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5313c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5313c-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5313c-114">Delegated (work or school account)</span></span> | <span data-ttu-id="5313c-115">User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5313c-115">User.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5313c-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5313c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5313c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5313c-117">Not supported.</span></span>    |
|<span data-ttu-id="5313c-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5313c-118">Application</span></span> | <span data-ttu-id="5313c-119">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5313c-119">User.ReadWrite.All</span></span> |

<span data-ttu-id="5313c-120">A conta profissional ou escolar deve desempenhar uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="5313c-120">The work or school account must be in one of the following roles:</span></span>
+ <span data-ttu-id="5313c-121">Administrador Global</span><span class="sxs-lookup"><span data-stu-id="5313c-121">Global Administrator</span></span>
+ <span data-ttu-id="5313c-122">Administrador do usuário</span><span class="sxs-lookup"><span data-stu-id="5313c-122">User Administrator</span></span>

<span data-ttu-id="5313c-123">Somente um Administrador Global pode excluir um usuário em uma função de Administrador Global ou _qualquer_ usuário no locatário.</span><span class="sxs-lookup"><span data-stu-id="5313c-123">Only a Global Administrator can delete a user in a Global Administrator role or _any_ user in the tenant.</span></span> <span data-ttu-id="5313c-124">Um administrador de usuários só pode excluir usuários que não sejam administradores ou que tenham funções limitadas específicas.</span><span class="sxs-lookup"><span data-stu-id="5313c-124">A User Administrator can only delete users who are non-administrators or in specific limited roles.</span></span> <span data-ttu-id="5313c-125">Para obter mais detalhes, consulte [Permissões de função de administrador no Microsoft Azure Active Directory](/azure/active-directory/roles/permissions-reference#available-roles).</span><span class="sxs-lookup"><span data-stu-id="5313c-125">For more details, see [Administrator role permissions in Azure AD](/azure/active-directory/roles/permissions-reference#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="5313c-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5313c-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="5313c-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5313c-127">Request headers</span></span>

| <span data-ttu-id="5313c-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5313c-128">Header</span></span>       | <span data-ttu-id="5313c-129">Valor</span><span class="sxs-lookup"><span data-stu-id="5313c-129">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="5313c-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="5313c-130">Authorization</span></span>  | <span data-ttu-id="5313c-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5313c-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5313c-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5313c-133">Request body</span></span>

<span data-ttu-id="5313c-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5313c-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5313c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="5313c-135">Response</span></span>

<span data-ttu-id="5313c-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5313c-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5313c-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5313c-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="5313c-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5313c-139">Request</span></span>

<span data-ttu-id="5313c-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5313c-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5313c-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="5313c-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_user"
}-->
```http
DELETE https://graph.microsoft.com/beta/users/ba9a3254-9f18-4209-aeb3-9e42a35b5be4 
```
# <a name="c"></a>[<span data-ttu-id="5313c-142">C#</span><span class="sxs-lookup"><span data-stu-id="5313c-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5313c-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5313c-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5313c-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5313c-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5313c-145">Java</span><span class="sxs-lookup"><span data-stu-id="5313c-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="5313c-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="5313c-146">Response</span></span>

<span data-ttu-id="5313c-147">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5313c-147">Here is an example of the response.</span></span> 
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


