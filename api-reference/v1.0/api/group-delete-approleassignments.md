---
title: Excluir um appRoleAssignment de um grupo
description: Excluir um appRoleAssignment que tenha sido concedido a um grupo.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 1b4f1b66a0d5fb33669719a33598fc47ffe2efb7
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44332398"
---
# <a name="delete-an-approleassignment-granted-to-a-group"></a><span data-ttu-id="a8e54-103">Excluir um appRoleAssignment concedido a um grupo</span><span class="sxs-lookup"><span data-stu-id="a8e54-103">Delete an appRoleAssignment granted to a group</span></span>

<span data-ttu-id="a8e54-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8e54-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a8e54-105">Exclui um [appRoleAssignment](../resources/approleassignment.md) que um grupo foi concedido.</span><span class="sxs-lookup"><span data-stu-id="a8e54-105">Deletes an [appRoleAssignment](../resources/approleassignment.md) which a group has been granted.</span></span>

## <a name="permissions"></a><span data-ttu-id="a8e54-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a8e54-106">Permissions</span></span>

<span data-ttu-id="a8e54-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8e54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8e54-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a8e54-109">Permission type</span></span>      | <span data-ttu-id="a8e54-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a8e54-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a8e54-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a8e54-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a8e54-112">AppRoleAssignment. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="a8e54-112">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a8e54-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a8e54-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8e54-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a8e54-114">Not supported.</span></span>    |
|<span data-ttu-id="a8e54-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a8e54-115">Application</span></span> | <span data-ttu-id="a8e54-116">AppRoleAssignment. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="a8e54-116">AppRoleAssignment.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a8e54-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a8e54-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /groups/{id}/appRoleAssignments/{id}
```

> [!NOTE]
> <span data-ttu-id="a8e54-118">Como prática recomendada, recomendamos a exclusão de atribuições de função de aplicativo através da `appRoleAssignedTo` relação da entidade de serviço de _recurso_ , em vez da `appRoleAssignments` relação do usuário, grupo ou entidade de serviço atribuída.</span><span class="sxs-lookup"><span data-stu-id="a8e54-118">As a best practice, we recommend deleting app role assignments through the `appRoleAssignedTo` relationship of the _resource_ service principal, instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a8e54-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a8e54-119">Request headers</span></span>

| <span data-ttu-id="a8e54-120">Nome</span><span class="sxs-lookup"><span data-stu-id="a8e54-120">Name</span></span>       | <span data-ttu-id="a8e54-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8e54-121">Type</span></span> | <span data-ttu-id="a8e54-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8e54-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a8e54-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a8e54-123">Authorization</span></span>  | <span data-ttu-id="a8e54-124">string</span><span class="sxs-lookup"><span data-stu-id="a8e54-124">string</span></span>  | <span data-ttu-id="a8e54-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a8e54-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a8e54-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a8e54-127">Request body</span></span>

<span data-ttu-id="a8e54-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a8e54-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a8e54-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8e54-129">Response</span></span>

<span data-ttu-id="a8e54-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a8e54-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a8e54-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a8e54-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a8e54-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a8e54-133">Request</span></span>

<span data-ttu-id="a8e54-134">Veja a seguir um exemplo da solicitação para excluir uma atribuição de função de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a8e54-134">Here is an example of the request to delete an app role assignment.</span></span>


# <a name="http"></a>[<span data-ttu-id="a8e54-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="a8e54-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_delete_approleassignment"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/appRoleAssignments/{id}
```
# <a name="c"></a>[<span data-ttu-id="a8e54-136">C#</span><span class="sxs-lookup"><span data-stu-id="a8e54-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-delete-approleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a8e54-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a8e54-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-delete-approleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a8e54-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a8e54-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-delete-approleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a8e54-139">Java</span><span class="sxs-lookup"><span data-stu-id="a8e54-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-delete-approleassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a8e54-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8e54-140">Response</span></span>

<span data-ttu-id="a8e54-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a8e54-141">The following is an example of the response.</span></span>

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
