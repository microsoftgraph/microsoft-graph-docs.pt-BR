---
title: Excluir unifiedRoleAssignment
description: Excluir um objeto unifiedRoleAssignment.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f11d0017c9dc7ac403f40ee8e913b489bf3969e7
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48978154"
---
# <a name="delete-unifiedroleassignment"></a><span data-ttu-id="5d6b8-103">Excluir unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="5d6b8-103">Delete unifiedRoleAssignment</span></span>

<span data-ttu-id="5d6b8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d6b8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d6b8-105">Excluir um objeto [unifiedRoleAssignment](../resources/unifiedRoleAssignment.md) .</span><span class="sxs-lookup"><span data-stu-id="5d6b8-105">Delete a [unifiedRoleAssignment](../resources/unifiedRoleAssignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5d6b8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5d6b8-106">Permissions</span></span>

<span data-ttu-id="5d6b8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d6b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5d6b8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5d6b8-109">Permission type</span></span>                        | <span data-ttu-id="5d6b8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5d6b8-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5d6b8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5d6b8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5d6b8-112">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="5d6b8-112">RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="5d6b8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5d6b8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d6b8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5d6b8-114">Not supported.</span></span> |
| <span data-ttu-id="5d6b8-115">Application</span><span class="sxs-lookup"><span data-stu-id="5d6b8-115">Application</span></span>                            | <span data-ttu-id="5d6b8-116">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="5d6b8-116">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d6b8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5d6b8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /roleManagement/directory/roleAssignments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5d6b8-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5d6b8-118">Request headers</span></span>

| <span data-ttu-id="5d6b8-119">Nome</span><span class="sxs-lookup"><span data-stu-id="5d6b8-119">Name</span></span>          | <span data-ttu-id="5d6b8-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d6b8-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="5d6b8-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5d6b8-121">Authorization</span></span> | <span data-ttu-id="5d6b8-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="5d6b8-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="5d6b8-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5d6b8-123">Request body</span></span>

<span data-ttu-id="5d6b8-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5d6b8-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5d6b8-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d6b8-125">Response</span></span>

<span data-ttu-id="5d6b8-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5d6b8-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d6b8-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5d6b8-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="5d6b8-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5d6b8-129">Request</span></span>

<span data-ttu-id="5d6b8-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5d6b8-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5d6b8-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="5d6b8-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroleassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="c"></a>[<span data-ttu-id="5d6b8-132">C#</span><span class="sxs-lookup"><span data-stu-id="5d6b8-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedroleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5d6b8-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5d6b8-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedroleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5d6b8-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5d6b8-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedroleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5d6b8-135">Java</span><span class="sxs-lookup"><span data-stu-id="5d6b8-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-unifiedroleassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5d6b8-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d6b8-136">Response</span></span>

<span data-ttu-id="5d6b8-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5d6b8-137">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete unifiedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


