---
title: Excluir unifiedRoleAssignment
description: Exclua um objeto unifiedRoleAssignment.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 865d18f0278084ecf884ead909374eeccaaace54
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444880"
---
# <a name="delete-unifiedroleassignment"></a><span data-ttu-id="464ec-103">Excluir unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="464ec-103">Delete unifiedRoleAssignment</span></span>

<span data-ttu-id="464ec-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="464ec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="464ec-105">[Exclua um objeto unifiedRoleAssignment.](../resources/unifiedRoleAssignment.md)</span><span class="sxs-lookup"><span data-stu-id="464ec-105">Delete a [unifiedRoleAssignment](../resources/unifiedRoleAssignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="464ec-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="464ec-106">Permissions</span></span>

<span data-ttu-id="464ec-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="464ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="464ec-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="464ec-109">Permission type</span></span>                        | <span data-ttu-id="464ec-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="464ec-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="464ec-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="464ec-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="464ec-112">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="464ec-112">RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="464ec-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="464ec-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="464ec-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="464ec-114">Not supported.</span></span> |
| <span data-ttu-id="464ec-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="464ec-115">Application</span></span>                            | <span data-ttu-id="464ec-116">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="464ec-116">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="464ec-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="464ec-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /roleManagement/directory/roleAssignments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="464ec-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="464ec-118">Request headers</span></span>

| <span data-ttu-id="464ec-119">Nome</span><span class="sxs-lookup"><span data-stu-id="464ec-119">Name</span></span>          | <span data-ttu-id="464ec-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="464ec-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="464ec-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="464ec-121">Authorization</span></span> | <span data-ttu-id="464ec-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="464ec-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="464ec-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="464ec-123">Request body</span></span>

<span data-ttu-id="464ec-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="464ec-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="464ec-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="464ec-125">Response</span></span>

<span data-ttu-id="464ec-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="464ec-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="464ec-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="464ec-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="464ec-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="464ec-129">Request</span></span>

<span data-ttu-id="464ec-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="464ec-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="464ec-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="464ec-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroleassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="c"></a>[<span data-ttu-id="464ec-132">C#</span><span class="sxs-lookup"><span data-stu-id="464ec-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedroleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="464ec-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="464ec-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedroleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="464ec-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="464ec-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedroleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="464ec-135">Java</span><span class="sxs-lookup"><span data-stu-id="464ec-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-unifiedroleassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="464ec-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="464ec-136">Response</span></span>

<span data-ttu-id="464ec-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="464ec-137">The following is an example of the response.</span></span>

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


