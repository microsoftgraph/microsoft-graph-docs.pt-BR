---
title: Excluir um appRoleAssignment de uma entidade de serviço
description: Exclua um appRoleAssignment de uma entidade de serviço.
localization_priority: Normal
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 73993ee629ad9752192329adf58ec61deb07ecf6
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870532"
---
# <a name="delete-an-approleassignment-granted-to-a-service-principal"></a><span data-ttu-id="c5fe9-103">Excluir um appRoleAssignment concedido a uma entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="c5fe9-103">Delete an appRoleAssignment granted to a service principal</span></span>

<span data-ttu-id="c5fe9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5fe9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c5fe9-105">Exclui um [appRoleAssignment](../resources/approleassignment.md) que uma entidade de serviço recebeu.</span><span class="sxs-lookup"><span data-stu-id="c5fe9-105">Deletes an [appRoleAssignment](../resources/approleassignment.md) that a service principal has been granted.</span></span>

<span data-ttu-id="c5fe9-106">Funções de aplicativo atribuídas a entidades de serviço também são conhecidas como [permissões de aplicativo.](/azure/active-directory/develop/v2-permissions-and-consent#permission-types)</span><span class="sxs-lookup"><span data-stu-id="c5fe9-106">App roles which are assigned to service principals are also known as [application permissions](/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span></span> <span data-ttu-id="c5fe9-107">Excluir uma atribuição de função de aplicativo para uma entidade de serviço equivale a revogar a concessão de permissão somente aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c5fe9-107">Deleting an app role assignment for a service principal is equivalent to revoking the app-only permission grant.</span></span>

## <a name="permissions"></a><span data-ttu-id="c5fe9-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="c5fe9-108">Permissions</span></span>

<span data-ttu-id="c5fe9-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5fe9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5fe9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c5fe9-111">Permission type</span></span>      | <span data-ttu-id="c5fe9-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c5fe9-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5fe9-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c5fe9-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c5fe9-114">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c5fe9-114">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c5fe9-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c5fe9-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5fe9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5fe9-116">Not supported.</span></span>    |
|<span data-ttu-id="c5fe9-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c5fe9-117">Application</span></span> | <span data-ttu-id="c5fe9-118">AppRoleAssignment.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5fe9-118">AppRoleAssignment.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c5fe9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c5fe9-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{servicePrincipal-id}/appRoleAssignments/{appRoleAssignment-id}
```

> [!NOTE]
> <span data-ttu-id="c5fe9-120">Como prática prática, recomendamos excluir atribuições de função de aplicativo por meio da relação da entidade de serviço de recursos, em vez da relação do usuário, grupo ou entidade de `appRoleAssignedTo` serviço  `appRoleAssignments` atribuída.</span><span class="sxs-lookup"><span data-stu-id="c5fe9-120">As a best practice, we recommend deleting app role assignments through the `appRoleAssignedTo` relationship of the _resource_ service principal, instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c5fe9-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c5fe9-121">Request headers</span></span>

| <span data-ttu-id="c5fe9-122">Nome</span><span class="sxs-lookup"><span data-stu-id="c5fe9-122">Name</span></span>       | <span data-ttu-id="c5fe9-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="c5fe9-123">Type</span></span> | <span data-ttu-id="c5fe9-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5fe9-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c5fe9-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c5fe9-125">Authorization</span></span>  | <span data-ttu-id="c5fe9-126">string</span><span class="sxs-lookup"><span data-stu-id="c5fe9-126">string</span></span>  | <span data-ttu-id="c5fe9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c5fe9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c5fe9-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c5fe9-129">Request body</span></span>

<span data-ttu-id="c5fe9-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c5fe9-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5fe9-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5fe9-131">Response</span></span>

<span data-ttu-id="c5fe9-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c5fe9-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c5fe9-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c5fe9-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c5fe9-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c5fe9-135">Request</span></span>

<span data-ttu-id="c5fe9-136">Aqui está um exemplo da solicitação para excluir uma atribuição de função de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c5fe9-136">Here is an example of the request to delete an app role assignment.</span></span>


# <a name="http"></a>[<span data-ttu-id="c5fe9-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="c5fe9-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_delete_approleassignment"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/servicePrincipals/{servicePrincipal-id}/appRoleAssignments/{appRoleAssignment-id}
```
# <a name="c"></a>[<span data-ttu-id="c5fe9-138">C#</span><span class="sxs-lookup"><span data-stu-id="c5fe9-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-delete-approleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c5fe9-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c5fe9-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-delete-approleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c5fe9-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c5fe9-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-delete-approleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c5fe9-141">Java</span><span class="sxs-lookup"><span data-stu-id="c5fe9-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-delete-approleassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c5fe9-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5fe9-142">Response</span></span>

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
