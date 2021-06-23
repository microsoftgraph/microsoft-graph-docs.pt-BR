---
title: Conceder um appRoleAssignment para uma entidade de serviço
description: Conceder uma atribuição de função de aplicativo a uma entidade de serviço.
localization_priority: Priority
doc_type: apiPageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: 2f664742481dd289582f017b83142ec5db10918f
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060469"
---
# <a name="grant-an-approleassignment-for-a-service-principal"></a><span data-ttu-id="c9562-103">Conceder um appRoleAssignment para uma entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="c9562-103">Grant an appRoleAssignment for a service principal</span></span>

<span data-ttu-id="c9562-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9562-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9562-105">Atribuir uma função de aplicativo a uma entidade de serviço de recurso, a um usuário, grupo ou entidade de serviço de cliente.</span><span class="sxs-lookup"><span data-stu-id="c9562-105">Assign an app role for a resource service principal, to a user, group, or client service principal.</span></span>

<span data-ttu-id="c9562-106">As funções do aplicativo atribuídas às entidades de serviço também são conhecidas como [permissões de aplicativo](/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span><span class="sxs-lookup"><span data-stu-id="c9562-106">App roles that are assigned to service principals are also known as [application permissions](/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span></span> <span data-ttu-id="c9562-107">As permissões de aplicativo podem ser concedidas diretamente com atribuições de função de aplicativo ou por meio de uma [experiência de consentimento](/azure/active-directory/develop/application-consent-experience).</span><span class="sxs-lookup"><span data-stu-id="c9562-107">Application permissions can be granted directly with app role assignments, or through a [consent experience](/azure/active-directory/develop/application-consent-experience).</span></span>

<span data-ttu-id="c9562-108">Para conceder uma atribuição de função de aplicativo, você precisará de três identificadores:</span><span class="sxs-lookup"><span data-stu-id="c9562-108">To grant an app role assignment, you need three identifiers:</span></span>

- <span data-ttu-id="c9562-109">`principalId`: A `id` do **usuário**, **grupo** ou cliente **servicePrincipal** ao qual você está atribuindo a função de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c9562-109">`principalId`: The `id` of the **user**, **group** or client **servicePrincipal** to which you are assigning the app role.</span></span>
- <span data-ttu-id="c9562-110">`resourceId`: A `id` do recurso **servicePrincipal** que definiu a função do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c9562-110">`resourceId`: The `id` of the resource **servicePrincipal** which has defined the app role.</span></span>
- <span data-ttu-id="c9562-111">`appRoleId`: A `id` do **appRole** (definida na entidade de serviço de recurso) para atribuir a um usuário, grupo ou entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="c9562-111">`appRoleId`: The `id` of the **appRole** (defined on the resource service principal) to assign to a user, group, or service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="c9562-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="c9562-112">Permissions</span></span>

<span data-ttu-id="c9562-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9562-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9562-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c9562-115">Permission type</span></span>      | <span data-ttu-id="c9562-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c9562-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c9562-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c9562-117">Delegated (work or school account)</span></span> | <span data-ttu-id="c9562-118">AppRoleAssignment.ReadWrite.All e Application.Read.All, AppRoleAssignment.ReadWrite.All e Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c9562-118">AppRoleAssignment.ReadWrite.All and Application.Read.All, AppRoleAssignment.ReadWrite.All and Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c9562-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c9562-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9562-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c9562-120">Not supported.</span></span>    |
|<span data-ttu-id="c9562-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c9562-121">Application</span></span> | <span data-ttu-id="c9562-122">AppRoleAssignment.ReadWrite.All e Application.Read.All, AppRoleAssignment.ReadWrite.All e Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9562-122">AppRoleAssignment.ReadWrite.All and Application.Read.All, AppRoleAssignment.ReadWrite.All and Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c9562-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c9562-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/appRoleAssignedTo
```

## <a name="request-headers"></a><span data-ttu-id="c9562-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c9562-124">Request headers</span></span>

| <span data-ttu-id="c9562-125">Nome</span><span class="sxs-lookup"><span data-stu-id="c9562-125">Name</span></span>       | <span data-ttu-id="c9562-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9562-126">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="c9562-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="c9562-127">Authorization</span></span> | <span data-ttu-id="c9562-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c9562-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c9562-130">Content-type</span><span class="sxs-lookup"><span data-stu-id="c9562-130">Content-type</span></span> | <span data-ttu-id="c9562-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c9562-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c9562-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c9562-133">Request body</span></span>

<span data-ttu-id="c9562-134">No corpo da solicitação, forneça uma representação JSON de um objeto [appRoleAssignment](../resources/approleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c9562-134">In the request body, supply a JSON representation of an [appRoleAssignment](../resources/approleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c9562-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9562-135">Response</span></span>

<span data-ttu-id="c9562-136">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [appRoleAssignment](../resources/approleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c9562-136">If successful, this method returns a `201 Created` response code and an [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c9562-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c9562-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c9562-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c9562-138">Request</span></span>

<span data-ttu-id="c9562-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c9562-139">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c9562-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="c9562-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_create_approleassignedto"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/9028d19c-26a9-4809-8e3f-20ff73e2d75e/appRoleAssignedTo
Content-Type: application/json

{
  "principalId": "33ad69f9-da99-4bed-acd0-3f24235cb296",
  "resourceId": "9028d19c-26a9-4809-8e3f-20ff73e2d75e",
  "appRoleId": "ef7437e6-4f94-4a0a-a110-a439eb2aa8f7"
}
```
# <a name="c"></a>[<span data-ttu-id="c9562-141">C#</span><span class="sxs-lookup"><span data-stu-id="c9562-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-create-approleassignedto-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c9562-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c9562-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-create-approleassignedto-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c9562-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c9562-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-create-approleassignedto-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c9562-144">Java</span><span class="sxs-lookup"><span data-stu-id="c9562-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-create-approleassignedto-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="c9562-145">Neste exemplo, `{id}` e `{resourceId-value}` seriam os `id` da entidade de serviço de recurso e `{principalId}` seria o `id` do objeto de serviço de cliente, grupo ou cliente atribuído.</span><span class="sxs-lookup"><span data-stu-id="c9562-145">In this example, `{id}` and `{resourceId-value}` would both be the `id` of the resource service principal, and `{principalId}` would be the `id` of the assigned user, group, or client service principal.</span></span>

### <a name="response"></a><span data-ttu-id="c9562-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9562-146">Response</span></span>

<span data-ttu-id="c9562-147">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c9562-147">Here is an example of the response.</span></span> 

> <span data-ttu-id="c9562-148">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c9562-148">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#servicePrincipals('9028d19c-26a9-4809-8e3f-20ff73e2d75e')/appRoleAssignedTo/$entity",
  "id": "-WmtM5na7Uus0D8kI1yylpU9Mdo0Pb9OoBJvd3T5eKc",
  "deletedDateTime": null,
  "appRoleId": "ef7437e6-4f94-4a0a-a110-a439eb2aa8f7",
  "creationTimestamp": "2021-02-15T16:14:59.8643039Z",
  "principalDisplayName": "Parents of Contoso",
  "principalId": "33ad69f9-da99-4bed-acd0-3f24235cb296",
  "principalType": "Group",
  "resourceDisplayName": "Fabrikam App",
  "resourceId": "9028d19c-26a9-4809-8e3f-20ff73e2d75e"
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
