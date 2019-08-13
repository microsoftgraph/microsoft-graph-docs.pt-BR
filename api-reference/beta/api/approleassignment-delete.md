---
title: Excluir appRoleAssignment
description: Exclua appRoleAssignment.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: a6572f08f6a4a45b4cdae162c51c2a137ae2afa7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36318569"
---
# <a name="delete-approleassignment"></a><span data-ttu-id="fee0e-103">Excluir appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="fee0e-103">Delete appRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fee0e-104">Exclua appRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="fee0e-104">Delete appRoleAssignment.</span></span>
## <a name="permissions"></a><span data-ttu-id="fee0e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="fee0e-105">Permissions</span></span>
<span data-ttu-id="fee0e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fee0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fee0e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fee0e-108">Permission type</span></span>      | <span data-ttu-id="fee0e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fee0e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fee0e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fee0e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fee0e-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fee0e-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fee0e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fee0e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fee0e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fee0e-113">Not supported.</span></span>    |
|<span data-ttu-id="fee0e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fee0e-114">Application</span></span> | <span data-ttu-id="fee0e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fee0e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fee0e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fee0e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}/appRoleAssignments/{id}
DELETE /servicePrincipals/{id}/appRoleAssignedTo
DELETE /groups/{id}/appRoleAssignments/{id}

```
## <a name="request-headers"></a><span data-ttu-id="fee0e-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fee0e-117">Request headers</span></span>
| <span data-ttu-id="fee0e-118">Nome</span><span class="sxs-lookup"><span data-stu-id="fee0e-118">Name</span></span>       | <span data-ttu-id="fee0e-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="fee0e-119">Type</span></span> | <span data-ttu-id="fee0e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="fee0e-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fee0e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="fee0e-121">Authorization</span></span>  | <span data-ttu-id="fee0e-122">string</span><span class="sxs-lookup"><span data-stu-id="fee0e-122">string</span></span>  | <span data-ttu-id="fee0e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fee0e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fee0e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fee0e-125">Request body</span></span>
<span data-ttu-id="fee0e-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fee0e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fee0e-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="fee0e-127">Response</span></span>

<span data-ttu-id="fee0e-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fee0e-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fee0e-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fee0e-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fee0e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fee0e-131">Request</span></span>
<span data-ttu-id="fee0e-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fee0e-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fee0e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="fee0e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_approleassignment"
}-->
```http
DELETE https://graph.microsoft.com/beta/appRoleAssignments/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fee0e-134">C#</span><span class="sxs-lookup"><span data-stu-id="fee0e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-approleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fee0e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fee0e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-approleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fee0e-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="fee0e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-approleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="fee0e-137">Java</span><span class="sxs-lookup"><span data-stu-id="fee0e-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-approleassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fee0e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="fee0e-138">Response</span></span>
<span data-ttu-id="fee0e-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fee0e-139">Here is an example of the response.</span></span> 
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
