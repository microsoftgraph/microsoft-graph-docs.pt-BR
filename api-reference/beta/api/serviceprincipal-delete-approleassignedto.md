---
title: Excluir um appRoleAssignment concedido para uma entidade de serviço
description: Exclua um appRoleAssignment concedido para uma entidade de serviço.
localization_priority: Normal
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: b6083a3fdadebfb6d9c5d2541609f9ec870b9051
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132166"
---
# <a name="delete-an-approleassignment-granted-for-a-service-principal"></a><span data-ttu-id="fbc14-103">Excluir um appRoleAssignment concedido para uma entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="fbc14-103">Delete an appRoleAssignment granted for a service principal</span></span>

<span data-ttu-id="fbc14-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fbc14-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fbc14-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fbc14-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fbc14-106">Exclui um [appRoleAssignment que](../resources/approleassignment.md) um usuário, grupo ou entidade de serviço cliente recebeu para uma entidade de serviço de recurso.</span><span class="sxs-lookup"><span data-stu-id="fbc14-106">Deletes an [appRoleAssignment](../resources/approleassignment.md) that a user, group, or client service principal has been granted for a resource service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="fbc14-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="fbc14-107">Permissions</span></span>

<span data-ttu-id="fbc14-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fbc14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbc14-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fbc14-110">Permission type</span></span>      | <span data-ttu-id="fbc14-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fbc14-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fbc14-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fbc14-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fbc14-113">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fbc14-113">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fbc14-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fbc14-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fbc14-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fbc14-115">Not supported.</span></span>    |
|<span data-ttu-id="fbc14-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fbc14-116">Application</span></span> | <span data-ttu-id="fbc14-117">AppRoleAssignment.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbc14-117">AppRoleAssignment.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fbc14-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fbc14-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{id}/appRoleAssignedTo/{id}
```

> [!NOTE]
> <span data-ttu-id="fbc14-119">Como prática recomendável, recomendamos excluir atribuições de função de aplicativo por meio da relação da entidade de serviço de recurso, em vez da relação do usuário, grupo ou entidade de `appRoleAssignedTo` serviço  `appRoleAssignments` atribuído.</span><span class="sxs-lookup"><span data-stu-id="fbc14-119">As a best practice, we recommend deleting app role assignments through the `appRoleAssignedTo` relationship of the _resource_ service principal, instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fbc14-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fbc14-120">Request headers</span></span>

| <span data-ttu-id="fbc14-121">Nome</span><span class="sxs-lookup"><span data-stu-id="fbc14-121">Name</span></span>       | <span data-ttu-id="fbc14-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="fbc14-122">Type</span></span> | <span data-ttu-id="fbc14-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="fbc14-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fbc14-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="fbc14-124">Authorization</span></span>  | <span data-ttu-id="fbc14-125">string</span><span class="sxs-lookup"><span data-stu-id="fbc14-125">string</span></span>  | <span data-ttu-id="fbc14-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fbc14-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fbc14-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fbc14-128">Request body</span></span>

<span data-ttu-id="fbc14-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fbc14-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fbc14-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="fbc14-130">Response</span></span>

<span data-ttu-id="fbc14-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fbc14-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fbc14-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fbc14-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fbc14-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fbc14-134">Request</span></span>

<span data-ttu-id="fbc14-135">Aqui está um exemplo da solicitação para excluir uma atribuição de função de aplicativo da entidade de serviço de recurso.</span><span class="sxs-lookup"><span data-stu-id="fbc14-135">Here is an example of the request to delete an app role assignment from the resource service principal.</span></span>


# <a name="http"></a>[<span data-ttu-id="fbc14-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="fbc14-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_delete_approleassignedto"
}-->

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/appRoleAssignedTo/{id}
```
# <a name="c"></a>[<span data-ttu-id="fbc14-137">C#</span><span class="sxs-lookup"><span data-stu-id="fbc14-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-delete-approleassignedto-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fbc14-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fbc14-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-delete-approleassignedto-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fbc14-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fbc14-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-delete-approleassignedto-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fbc14-140">Java</span><span class="sxs-lookup"><span data-stu-id="fbc14-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-delete-approleassignedto-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fbc14-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="fbc14-141">Response</span></span>

<span data-ttu-id="fbc14-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fbc14-142">The following is an example of the response.</span></span>

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



