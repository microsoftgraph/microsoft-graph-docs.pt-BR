---
title: Excluir um appRoleAssignment de uma entidade de serviço
description: Exclua um appRoleAssignment de uma entidade de serviço.
localization_priority: Normal
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: e9371de86e49efae1ca85852abb1e02e955d22e5
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135832"
---
# <a name="delete-an-approleassignment-granted-to-a-service-principal"></a><span data-ttu-id="d9082-103">Excluir um appRoleAssignment concedido a uma entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="d9082-103">Delete an appRoleAssignment granted to a service principal</span></span>

<span data-ttu-id="d9082-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9082-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d9082-105">Exclui um [appRoleAssignment que](../resources/approleassignment.md) uma entidade de serviço recebeu.</span><span class="sxs-lookup"><span data-stu-id="d9082-105">Deletes an [appRoleAssignment](../resources/approleassignment.md) that a service principal has been granted.</span></span>

<span data-ttu-id="d9082-106">Funções de aplicativo que são atribuídas a entidades de serviço também são conhecidas como [permissões de aplicativo.](/azure/active-directory/develop/v2-permissions-and-consent#permission-types)</span><span class="sxs-lookup"><span data-stu-id="d9082-106">App roles which are assigned to service principals are also known as [application permissions](/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span></span> <span data-ttu-id="d9082-107">Excluir uma atribuição de função de aplicativo para uma entidade de serviço é equivalente a revogar a concessão de permissão somente de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d9082-107">Deleting an app role assignment for a service principal is equivalent to revoking the app-only permission grant.</span></span>

## <a name="permissions"></a><span data-ttu-id="d9082-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="d9082-108">Permissions</span></span>

<span data-ttu-id="d9082-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9082-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9082-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d9082-111">Permission type</span></span>      | <span data-ttu-id="d9082-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d9082-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9082-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d9082-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d9082-114">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d9082-114">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d9082-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d9082-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9082-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9082-116">Not supported.</span></span>    |
|<span data-ttu-id="d9082-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d9082-117">Application</span></span> | <span data-ttu-id="d9082-118">AppRoleAssignment.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9082-118">AppRoleAssignment.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d9082-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d9082-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{id}/appRoleAssignments/{id}
```

> [!NOTE]
> <span data-ttu-id="d9082-120">Como prática recomendável, recomendamos excluir atribuições de função de aplicativo por meio da relação da entidade de serviço de recurso, em vez da relação do usuário, grupo ou entidade de `appRoleAssignedTo` serviço  `appRoleAssignments` atribuído.</span><span class="sxs-lookup"><span data-stu-id="d9082-120">As a best practice, we recommend deleting app role assignments through the `appRoleAssignedTo` relationship of the _resource_ service principal, instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d9082-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d9082-121">Request headers</span></span>

| <span data-ttu-id="d9082-122">Nome</span><span class="sxs-lookup"><span data-stu-id="d9082-122">Name</span></span>       | <span data-ttu-id="d9082-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="d9082-123">Type</span></span> | <span data-ttu-id="d9082-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9082-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d9082-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="d9082-125">Authorization</span></span>  | <span data-ttu-id="d9082-126">string</span><span class="sxs-lookup"><span data-stu-id="d9082-126">string</span></span>  | <span data-ttu-id="d9082-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d9082-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d9082-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d9082-129">Request body</span></span>

<span data-ttu-id="d9082-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d9082-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9082-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9082-131">Response</span></span>

<span data-ttu-id="d9082-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d9082-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d9082-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d9082-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d9082-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9082-135">Request</span></span>

<span data-ttu-id="d9082-136">Aqui está um exemplo da solicitação para excluir uma atribuição de função de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d9082-136">Here is an example of the request to delete an app role assignment.</span></span>


# <a name="http"></a>[<span data-ttu-id="d9082-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="d9082-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_delete_approleassignment"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/servicePrincipals/{id}/appRoleAssignments/{id}
```
# <a name="c"></a>[<span data-ttu-id="d9082-138">C#</span><span class="sxs-lookup"><span data-stu-id="d9082-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-delete-approleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d9082-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d9082-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-delete-approleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d9082-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d9082-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-delete-approleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d9082-141">Java</span><span class="sxs-lookup"><span data-stu-id="d9082-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-delete-approleassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d9082-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9082-142">Response</span></span>

<span data-ttu-id="d9082-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d9082-143">The following is an example of the response.</span></span>

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
