---
title: Excluir um appRoleAssignment concedido a um usuário
description: Excluir um appRoleAssignment que tenha sido concedido a um usuário.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: ef5b321435601ba5e9a39a5148e067eed7b985bf
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48976551"
---
# <a name="delete-an-approleassignment-granted-to-a-user"></a><span data-ttu-id="d0a85-103">Excluir um appRoleAssignment concedido a um usuário</span><span class="sxs-lookup"><span data-stu-id="d0a85-103">Delete an appRoleAssignment granted to a user</span></span>

<span data-ttu-id="d0a85-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0a85-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0a85-105">Excluir um [appRoleAssignment](../resources/approleassignment.md) que tenha sido concedido a um usuário.</span><span class="sxs-lookup"><span data-stu-id="d0a85-105">Delete an [appRoleAssignment](../resources/approleassignment.md) that has been granted to a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="d0a85-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d0a85-106">Permissions</span></span>

<span data-ttu-id="d0a85-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0a85-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0a85-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d0a85-109">Permission type</span></span>      | <span data-ttu-id="d0a85-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d0a85-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0a85-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d0a85-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d0a85-112">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d0a85-112">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d0a85-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d0a85-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0a85-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d0a85-114">Not supported.</span></span>    |
|<span data-ttu-id="d0a85-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d0a85-115">Application</span></span> | <span data-ttu-id="d0a85-116">AppRoleAssignment.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0a85-116">AppRoleAssignment.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d0a85-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d0a85-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /users/{id}/appRoleAssignments/{id}
```

> [!NOTE]
> <span data-ttu-id="d0a85-118">Como prática recomendada, recomendamos a exclusão de atribuições de função de aplicativo através da `appRoleAssignedTo` relação da entidade de serviço de _recurso_ , em vez da `appRoleAssignments` relação do usuário, grupo ou entidade de serviço atribuída.</span><span class="sxs-lookup"><span data-stu-id="d0a85-118">As a best practice, we recommend deleting app role assignments through the `appRoleAssignedTo` relationship of the _resource_ service principal, instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d0a85-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d0a85-119">Request headers</span></span>

| <span data-ttu-id="d0a85-120">Nome</span><span class="sxs-lookup"><span data-stu-id="d0a85-120">Name</span></span>       | <span data-ttu-id="d0a85-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="d0a85-121">Type</span></span> | <span data-ttu-id="d0a85-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0a85-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d0a85-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d0a85-123">Authorization</span></span>  | <span data-ttu-id="d0a85-124">string</span><span class="sxs-lookup"><span data-stu-id="d0a85-124">string</span></span>  | <span data-ttu-id="d0a85-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d0a85-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d0a85-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d0a85-127">Request body</span></span>

<span data-ttu-id="d0a85-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d0a85-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d0a85-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0a85-129">Response</span></span>

<span data-ttu-id="d0a85-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d0a85-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d0a85-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d0a85-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d0a85-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d0a85-133">Request</span></span>

<span data-ttu-id="d0a85-134">Veja a seguir um exemplo da solicitação para excluir uma atribuição de função de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d0a85-134">Here is an example of the request to delete an app role assignment.</span></span>


# <a name="http"></a>[<span data-ttu-id="d0a85-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="d0a85-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_delete_approleassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/users/{id}/appRoleAssignments/{id}
```
# <a name="c"></a>[<span data-ttu-id="d0a85-136">C#</span><span class="sxs-lookup"><span data-stu-id="d0a85-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-delete-approleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d0a85-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d0a85-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-delete-approleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d0a85-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d0a85-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-delete-approleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d0a85-139">Java</span><span class="sxs-lookup"><span data-stu-id="d0a85-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-delete-approleassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d0a85-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0a85-140">Response</span></span>

<span data-ttu-id="d0a85-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d0a85-141">Here is an example of the response.</span></span>

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
  "description": "Delete appRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


