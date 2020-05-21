---
title: Conceder um appRoleAssignment a um usuário
description: Conceda a um usuário uma atribuição de função de aplicativo.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: c6a34fa1116b5679c70997913b93b74d41b9e459
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44332470"
---
# <a name="grant-an-approleassignment-to-a-user"></a><span data-ttu-id="10f61-103">Conceder um appRoleAssignment a um usuário</span><span class="sxs-lookup"><span data-stu-id="10f61-103">Grant an appRoleAssignment to a user</span></span>

<span data-ttu-id="10f61-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10f61-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10f61-105">Use esta API para atribuir uma função de aplicativo a um usuário.</span><span class="sxs-lookup"><span data-stu-id="10f61-105">Use this API to assign an app role to a user.</span></span> <span data-ttu-id="10f61-106">Para conceder a um usuário uma atribuição de função de aplicativo, você precisa de três identificadores:</span><span class="sxs-lookup"><span data-stu-id="10f61-106">To grant an app role assignment to a user, you need three identifiers:</span></span>

- <span data-ttu-id="10f61-107">`principalId`: O `id` do usuário para o qual você está atribuindo a função de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="10f61-107">`principalId`: The `id` of the user to whom you are assigning the app role.</span></span>
- <span data-ttu-id="10f61-108">`resourceId`: O `id` do recurso `servicePrincipal` que definiu a função de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="10f61-108">`resourceId`: The `id` of the resource `servicePrincipal` that has defined the app role.</span></span>
- <span data-ttu-id="10f61-109">`appRoleId`: O `id` `appRole` (definido na entidade de segurança do serviço de recursos) a ser atribuído ao usuário.</span><span class="sxs-lookup"><span data-stu-id="10f61-109">`appRoleId`: The `id` of the `appRole` (defined on the resource service principal) to assign to the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="10f61-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="10f61-110">Permissions</span></span>

<span data-ttu-id="10f61-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10f61-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10f61-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="10f61-113">Permission type</span></span>      | <span data-ttu-id="10f61-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="10f61-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="10f61-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="10f61-115">Delegated (work or school account)</span></span> | <span data-ttu-id="10f61-116">AppRoleAssignment. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="10f61-116">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="10f61-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="10f61-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10f61-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="10f61-118">Not supported.</span></span>    |
|<span data-ttu-id="10f61-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="10f61-119">Application</span></span> | <span data-ttu-id="10f61-120">AppRoleAssignment. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="10f61-120">AppRoleAssignment.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="10f61-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="10f61-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/appRoleAssignments
```

> [!NOTE]
> <span data-ttu-id="10f61-122">Como prática recomendada, recomendamos a criação de atribuições de função de aplicativo através da `appRoleAssignedTo` relação da entidade de serviço de _recurso_ , em vez da `appRoleAssignments` relação do usuário, grupo ou entidade de serviço atribuída.</span><span class="sxs-lookup"><span data-stu-id="10f61-122">As a best practice, we recommend creating app role assignments through the `appRoleAssignedTo` relationship of the _resource_ service principal, instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="10f61-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="10f61-123">Request headers</span></span>

| <span data-ttu-id="10f61-124">Nome</span><span class="sxs-lookup"><span data-stu-id="10f61-124">Name</span></span>       | <span data-ttu-id="10f61-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="10f61-125">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="10f61-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="10f61-126">Authorization</span></span> | <span data-ttu-id="10f61-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="10f61-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="10f61-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="10f61-129">Content-Type</span></span> | <span data-ttu-id="10f61-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="10f61-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="10f61-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="10f61-132">Request body</span></span>

<span data-ttu-id="10f61-133">No corpo da solicitação, forneça uma representação JSON de um objeto [appRoleAssignment](../resources/approleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="10f61-133">In the request body, supply a JSON representation of an [appRoleAssignment](../resources/approleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="10f61-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="10f61-134">Response</span></span>

<span data-ttu-id="10f61-135">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [appRoleAssignment](../resources/approleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="10f61-135">If successful, this method returns a `201 Created` response code and an [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="10f61-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="10f61-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="10f61-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="10f61-137">Request</span></span>

<span data-ttu-id="10f61-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="10f61-138">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="10f61-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="10f61-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_create_approleassignment"
}-->

```http
POST https://graph.microsoft.com/beta/users/{id}/appRoleAssignments
Content-Type: application/json
Content-Length: 110

{
  "principalId": "principalId-value",
  "resourceId": "resourceId-value",
  "appRoleId": "appRoleId-value"
}
```
# <a name="c"></a>[<span data-ttu-id="10f61-140">C#</span><span class="sxs-lookup"><span data-stu-id="10f61-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-create-approleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="10f61-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="10f61-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-create-approleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="10f61-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="10f61-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-create-approleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="10f61-143">Neste exemplo, `{id}` e `{principalId-value}` seria o `id` do usuário atribuído.</span><span class="sxs-lookup"><span data-stu-id="10f61-143">In this example, `{id}` and `{principalId-value}` would both be the `id` of the assigned user.</span></span>

### <a name="response"></a><span data-ttu-id="10f61-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="10f61-144">Response</span></span>

<span data-ttu-id="10f61-145">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="10f61-145">Here is an example of the response.</span></span> 

> <span data-ttu-id="10f61-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="10f61-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 253

{
  "id": "id-value",
  "creationTimestamp": "2016-10-19T10:37:00Z",
  "principalType": "principalType-value",
  "principalId": "principalId-value",
  "principalDisplayName": "principalDisplayName-value",
  "resourceId": "resourceId-value",
  "resourceDisplayName": "resourceDisplayName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create appRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
