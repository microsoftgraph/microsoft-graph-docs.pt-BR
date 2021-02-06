---
title: Conceder um appRoleAssignment a uma entidade de serviço
description: Conceder uma atribuição de função de aplicativo a uma entidade de serviço.
localization_priority: Priority
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 56bf801b932f1458d871df8bbe51f40340302087
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134243"
---
# <a name="grant-an-approleassignment-to-a-service-principal"></a><span data-ttu-id="68fbf-103">Conceder um appRoleAssignment a uma entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="68fbf-103">Grant an appRoleAssignment to a service principal</span></span>

<span data-ttu-id="68fbf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68fbf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68fbf-105">Atribuir uma função de aplicativo a uma entidade de serviço do cliente.</span><span class="sxs-lookup"><span data-stu-id="68fbf-105">Assign an app role to a client service principal.</span></span>

<span data-ttu-id="68fbf-106">As funções do aplicativo atribuídas às entidades de serviço também são conhecidas como [permissões de aplicativo](/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span><span class="sxs-lookup"><span data-stu-id="68fbf-106">App roles that are assigned to service principals are also known as [application permissions](/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span></span> <span data-ttu-id="68fbf-107">As permissões de aplicativo podem ser concedidas diretamente com atribuições de função de aplicativo ou por meio de uma [experiência de consentimento](/azure/active-directory/develop/application-consent-experience).</span><span class="sxs-lookup"><span data-stu-id="68fbf-107">Application permissions can be granted directly with app role assignments, or through a [consent experience](/azure/active-directory/develop/application-consent-experience).</span></span>

<span data-ttu-id="68fbf-108">Para conceder uma atribuição de função de aplicativo a uma entidade de serviço do cliente, você precisa de três identificadores:</span><span class="sxs-lookup"><span data-stu-id="68fbf-108">To grant an app role assignment to a client service principal, you need three identifiers:</span></span>

- <span data-ttu-id="68fbf-109">`principalId`: A `id` da entidade de serviço do cliente ao qual você está atribuindo a função de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="68fbf-109">`principalId`: The `id` of the client service principal to which you are assigning the app role.</span></span>
- <span data-ttu-id="68fbf-110">`resourceId`: A `id` do recurso `servicePrincipal` (a API) que definiu a função do aplicativo (a permissão do aplicativo).</span><span class="sxs-lookup"><span data-stu-id="68fbf-110">`resourceId`: The `id` of the resource `servicePrincipal` (the API) which has defined the app role (the application permission).</span></span>
- <span data-ttu-id="68fbf-111">`appRoleId`: A `id` da `appRole` (definido na entidade de serviço do recurso) para atribuir à entidade de serviço do cliente.</span><span class="sxs-lookup"><span data-stu-id="68fbf-111">`appRoleId`: The `id` of the `appRole` (defined on the resource service principal) to assign to the client service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="68fbf-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="68fbf-112">Permissions</span></span>

<span data-ttu-id="68fbf-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68fbf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68fbf-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="68fbf-115">Permission type</span></span>      | <span data-ttu-id="68fbf-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="68fbf-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="68fbf-117">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="68fbf-117">Delegated (work or school account)</span></span> | <span data-ttu-id="68fbf-118">AppRoleAssignment. ReadWrite.All, Directory. ReadWrite.All, Directory. AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="68fbf-118">AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="68fbf-119">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="68fbf-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68fbf-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="68fbf-120">Not supported.</span></span>    |
|<span data-ttu-id="68fbf-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="68fbf-121">Application</span></span> | <span data-ttu-id="68fbf-122">AppRoleAssignment. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="68fbf-122">AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="68fbf-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="68fbf-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/appRoleAssignments
```

> [!NOTE]
> <span data-ttu-id="68fbf-124">Como prática recomendada, recomendamos que você crie atribuições de função de aplicativo por meio da [`appRoleAssignedTo`relação do _recurso_ da entidade de serviço](serviceprincipal-post-approleassignedto.md), em vez da `appRoleAssignments`relação do usuário, grupo ou entidade de serviço atribuída.</span><span class="sxs-lookup"><span data-stu-id="68fbf-124">As a best practice, we recommend creating app role assignments through the [`appRoleAssignedTo` relationship of the _resource_ service principal](serviceprincipal-post-approleassignedto.md), instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="68fbf-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="68fbf-125">Request headers</span></span>

| <span data-ttu-id="68fbf-126">Nome</span><span class="sxs-lookup"><span data-stu-id="68fbf-126">Name</span></span>       | <span data-ttu-id="68fbf-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="68fbf-127">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="68fbf-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="68fbf-128">Authorization</span></span> | <span data-ttu-id="68fbf-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="68fbf-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="68fbf-131">Content-type</span><span class="sxs-lookup"><span data-stu-id="68fbf-131">Content-type</span></span> | <span data-ttu-id="68fbf-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="68fbf-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="68fbf-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="68fbf-134">Request body</span></span>

<span data-ttu-id="68fbf-135">No corpo da solicitação, forneça uma representação JSON de um objeto [appRoleAssignment](../resources/approleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="68fbf-135">In the request body, supply a JSON representation of an [appRoleAssignment](../resources/approleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="68fbf-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="68fbf-136">Response</span></span>

<span data-ttu-id="68fbf-137">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [appRoleAssignment](../resources/approleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="68fbf-137">If successful, this method returns a `201 Created` response code and an [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="68fbf-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="68fbf-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="68fbf-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="68fbf-139">Request</span></span>

<span data-ttu-id="68fbf-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="68fbf-140">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="68fbf-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="68fbf-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_create_approleassignment"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/appRoleAssignments
Content-Type: application/json
Content-Length: 110

{
  "principalId": "principalId-value",
  "resourceId": "resourceId-value",
  "appRoleId": "appRoleId-value"
}
```
# <a name="c"></a>[<span data-ttu-id="68fbf-142">C#</span><span class="sxs-lookup"><span data-stu-id="68fbf-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-create-approleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="68fbf-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="68fbf-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-create-approleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="68fbf-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="68fbf-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-create-approleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="68fbf-145">Java</span><span class="sxs-lookup"><span data-stu-id="68fbf-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-create-approleassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="68fbf-146">Nesse exemplo, a `{id}` e o `{principalId-value}` seriam as `id` da entidade de serviço de cliente atribuída e o `{resourceId}` seria a `id` da entidade de serviço de recurso (a API).</span><span class="sxs-lookup"><span data-stu-id="68fbf-146">In this example, `{id}` and `{principalId-value}` would both be the `id` of the assigned client service principal, and `{resourceId}` would be the `id` of the resource service principal (the API).</span></span>

### <a name="response"></a><span data-ttu-id="68fbf-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="68fbf-147">Response</span></span>

<span data-ttu-id="68fbf-148">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="68fbf-148">Here is an example of the response.</span></span> 

> <span data-ttu-id="68fbf-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="68fbf-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment"
} -->

```http
HTTP/1.1 201 Created
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

