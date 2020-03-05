---
title: Excluir appRoleAssignment
description: Exclua appRoleAssignment.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 9a8c0d6f2ff76e8c95190cce52cecd8c19fd6b8a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441386"
---
# <a name="delete-approleassignment"></a><span data-ttu-id="6b5f9-103">Excluir appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="6b5f9-103">Delete appRoleAssignment</span></span>

<span data-ttu-id="6b5f9-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6b5f9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b5f9-105">Exclua appRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="6b5f9-105">Delete appRoleAssignment.</span></span>
## <a name="permissions"></a><span data-ttu-id="6b5f9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6b5f9-106">Permissions</span></span>
<span data-ttu-id="6b5f9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b5f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b5f9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6b5f9-109">Permission type</span></span>      | <span data-ttu-id="6b5f9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6b5f9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6b5f9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6b5f9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6b5f9-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6b5f9-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6b5f9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6b5f9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b5f9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6b5f9-114">Not supported.</span></span>    |
|<span data-ttu-id="6b5f9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b5f9-115">Application</span></span> | <span data-ttu-id="6b5f9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6b5f9-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6b5f9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6b5f9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}/appRoleAssignments/{id}
DELETE /groups/{id}/appRoleAssignments/{id}
DELETE /servicePrincipals/{id}/appRoleAssignments/{id}
DELETE /servicePrincipals/{id}/appRoleAssignedTo/{id}

```
## <a name="request-headers"></a><span data-ttu-id="6b5f9-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6b5f9-118">Request headers</span></span>
| <span data-ttu-id="6b5f9-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6b5f9-119">Name</span></span>       | <span data-ttu-id="6b5f9-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b5f9-120">Type</span></span> | <span data-ttu-id="6b5f9-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b5f9-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6b5f9-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6b5f9-122">Authorization</span></span>  | <span data-ttu-id="6b5f9-123">string</span><span class="sxs-lookup"><span data-stu-id="6b5f9-123">string</span></span>  | <span data-ttu-id="6b5f9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6b5f9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6b5f9-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6b5f9-126">Request body</span></span>
<span data-ttu-id="6b5f9-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6b5f9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6b5f9-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b5f9-128">Response</span></span>

<span data-ttu-id="6b5f9-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6b5f9-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b5f9-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6b5f9-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6b5f9-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6b5f9-132">Request</span></span>
<span data-ttu-id="6b5f9-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6b5f9-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6b5f9-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="6b5f9-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_approleassignment"
}-->
```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/appRoleAssignedTo/{id}
```
# <a name="c"></a>[<span data-ttu-id="6b5f9-135">C#</span><span class="sxs-lookup"><span data-stu-id="6b5f9-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-approleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6b5f9-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6b5f9-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-approleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6b5f9-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6b5f9-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-approleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6b5f9-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b5f9-138">Response</span></span>
<span data-ttu-id="6b5f9-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6b5f9-139">Here is an example of the response.</span></span> 
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
