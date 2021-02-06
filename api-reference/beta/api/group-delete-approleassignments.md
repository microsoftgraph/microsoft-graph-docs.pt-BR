---
title: Excluir um appRoleAssignment de um grupo
description: Exclua um appRoleAssignment que tenha sido concedido a um grupo.
localization_priority: Normal
doc_type: apiPageType
ms.prod: groups
author: psignoret
ms.openlocfilehash: 0ea559919312401bec8885f162788b8b01bb0464
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130792"
---
# <a name="delete-an-approleassignment-granted-to-a-group"></a><span data-ttu-id="0b899-103">Excluir um appRoleAssignment concedido a um grupo</span><span class="sxs-lookup"><span data-stu-id="0b899-103">Delete an appRoleAssignment granted to a group</span></span>

<span data-ttu-id="0b899-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b899-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b899-105">Exclui um [appRoleAssignment](../resources/approleassignment.md) que um grupo recebeu.</span><span class="sxs-lookup"><span data-stu-id="0b899-105">Deletes an [appRoleAssignment](../resources/approleassignment.md) that a group has been granted.</span></span>

## <a name="permissions"></a><span data-ttu-id="0b899-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0b899-106">Permissions</span></span>

<span data-ttu-id="0b899-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b899-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b899-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0b899-109">Permission type</span></span>      | <span data-ttu-id="0b899-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0b899-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b899-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0b899-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0b899-112">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0b899-112">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0b899-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0b899-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b899-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0b899-114">Not supported.</span></span>    |
|<span data-ttu-id="0b899-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0b899-115">Application</span></span> | <span data-ttu-id="0b899-116">AppRoleAssignment.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b899-116">AppRoleAssignment.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0b899-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0b899-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /groups/{id}/appRoleAssignments/{id}
```

> [!NOTE]
> <span data-ttu-id="0b899-118">Como prática recomendável, recomendamos excluir atribuições de função de aplicativo por meio da relação da entidade de serviço de recurso, em vez da relação do usuário, grupo ou entidade de `appRoleAssignedTo` serviço  `appRoleAssignments` atribuído.</span><span class="sxs-lookup"><span data-stu-id="0b899-118">As a best practice, we recommend deleting app role assignments through the `appRoleAssignedTo` relationship of the _resource_ service principal, instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0b899-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0b899-119">Request headers</span></span>

| <span data-ttu-id="0b899-120">Nome</span><span class="sxs-lookup"><span data-stu-id="0b899-120">Name</span></span>       | <span data-ttu-id="0b899-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b899-121">Type</span></span> | <span data-ttu-id="0b899-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b899-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0b899-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0b899-123">Authorization</span></span>  | <span data-ttu-id="0b899-124">string</span><span class="sxs-lookup"><span data-stu-id="0b899-124">string</span></span>  | <span data-ttu-id="0b899-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0b899-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0b899-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0b899-127">Request body</span></span>

<span data-ttu-id="0b899-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0b899-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b899-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b899-129">Response</span></span>

<span data-ttu-id="0b899-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0b899-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0b899-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0b899-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0b899-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0b899-133">Request</span></span>

<span data-ttu-id="0b899-134">Aqui está um exemplo da solicitação para excluir uma atribuição de função de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0b899-134">Here is an example of the request to delete an app role assignment.</span></span>


# <a name="http"></a>[<span data-ttu-id="0b899-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b899-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_delete_approleassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/groups/{id}/appRoleAssignments/{id}
```
# <a name="c"></a>[<span data-ttu-id="0b899-136">C#</span><span class="sxs-lookup"><span data-stu-id="0b899-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-delete-approleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0b899-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b899-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-delete-approleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0b899-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b899-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-delete-approleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0b899-139">Java</span><span class="sxs-lookup"><span data-stu-id="0b899-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-delete-approleassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0b899-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b899-140">Response</span></span>

<span data-ttu-id="0b899-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0b899-141">The following is an example of the response.</span></span>

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


