---
title: Excluir um appRoleAssignment concedido para uma entidade de serviço
description: Exclua um appRoleAssignment concedido para uma entidade de serviço.
localization_priority: Normal
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 6e0e124d285bbc22a87ef6073339cdf0f8ab7741
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50958197"
---
# <a name="delete-an-approleassignment-granted-for-a-service-principal"></a><span data-ttu-id="46ba0-103">Excluir um appRoleAssignment concedido para uma entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="46ba0-103">Delete an appRoleAssignment granted for a service principal</span></span>

<span data-ttu-id="46ba0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46ba0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="46ba0-105">Exclui um [appRoleAssignment](../resources/approleassignment.md) que um usuário, grupo ou entidade de serviço cliente foi concedido para uma entidade de serviço de recursos.</span><span class="sxs-lookup"><span data-stu-id="46ba0-105">Deletes an [appRoleAssignment](../resources/approleassignment.md) that a user, group, or client service principal has been granted for a resource service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="46ba0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="46ba0-106">Permissions</span></span>

<span data-ttu-id="46ba0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46ba0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46ba0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="46ba0-109">Permission type</span></span>      | <span data-ttu-id="46ba0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="46ba0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="46ba0-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="46ba0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="46ba0-112">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="46ba0-112">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="46ba0-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="46ba0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46ba0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46ba0-114">Not supported.</span></span>    |
|<span data-ttu-id="46ba0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="46ba0-115">Application</span></span> | <span data-ttu-id="46ba0-116">AppRoleAssignment.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46ba0-116">AppRoleAssignment.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="46ba0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="46ba0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{id}/appRoleAssignedTo/{id}
```

> [!NOTE]
> <span data-ttu-id="46ba0-118">Como prática prática, recomendamos excluir atribuições de função de aplicativo por meio da relação da entidade de serviço de recursos, em vez da relação do usuário, grupo ou entidade de `appRoleAssignedTo` serviço  `appRoleAssignments` atribuída.</span><span class="sxs-lookup"><span data-stu-id="46ba0-118">As a best practice, we recommend deleting app role assignments through the `appRoleAssignedTo` relationship of the _resource_ service principal, instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="46ba0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="46ba0-119">Request headers</span></span>

| <span data-ttu-id="46ba0-120">Nome</span><span class="sxs-lookup"><span data-stu-id="46ba0-120">Name</span></span>       | <span data-ttu-id="46ba0-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="46ba0-121">Type</span></span> | <span data-ttu-id="46ba0-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="46ba0-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="46ba0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="46ba0-123">Authorization</span></span>  | <span data-ttu-id="46ba0-124">string</span><span class="sxs-lookup"><span data-stu-id="46ba0-124">string</span></span>  | <span data-ttu-id="46ba0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46ba0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="46ba0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="46ba0-127">Request body</span></span>

<span data-ttu-id="46ba0-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="46ba0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46ba0-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="46ba0-129">Response</span></span>

<span data-ttu-id="46ba0-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="46ba0-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="46ba0-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="46ba0-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="46ba0-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46ba0-133">Request</span></span>

<span data-ttu-id="46ba0-134">Aqui está um exemplo da solicitação para excluir uma atribuição de função de aplicativo da entidade de serviço de recursos.</span><span class="sxs-lookup"><span data-stu-id="46ba0-134">Here is an example of the request to delete an app role assignment from the resource service principal.</span></span>


# <a name="http"></a>[<span data-ttu-id="46ba0-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="46ba0-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_delete_approleassignedto"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/servicePrincipals/{id}/appRoleAssignedTo/{id}
```
# <a name="c"></a>[<span data-ttu-id="46ba0-136">C#</span><span class="sxs-lookup"><span data-stu-id="46ba0-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-delete-approleassignedto-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="46ba0-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="46ba0-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-delete-approleassignedto-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="46ba0-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="46ba0-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-delete-approleassignedto-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="46ba0-139">Java</span><span class="sxs-lookup"><span data-stu-id="46ba0-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-delete-approleassignedto-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="46ba0-140">Neste exemplo, seria a id da entidade de serviço de recursos e seria a id do usuário, grupo ou entidade de serviço `{resource-SP-id}` `{principalId}` cliente atribuída.</span><span class="sxs-lookup"><span data-stu-id="46ba0-140">In this example, `{resource-SP-id}` would be the id of the resource service principal, and `{principalId}` would be the id of the assigned user, group, or client service principal.</span></span>

### <a name="response"></a><span data-ttu-id="46ba0-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="46ba0-141">Response</span></span>

<span data-ttu-id="46ba0-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="46ba0-142">The following is an example of the response.</span></span>

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

