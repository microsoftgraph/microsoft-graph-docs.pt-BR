---
title: Excluir unifiedRoleDefinition
description: Excluir um objeto unifiedRoleDefinition.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3950c02a7ef55c0c2f24878aa0c419cfe98d9f24
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48978868"
---
# <a name="delete-unifiedroledefinition"></a><span data-ttu-id="96c72-103">Excluir unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="96c72-103">Delete unifiedRoleDefinition</span></span>

<span data-ttu-id="96c72-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96c72-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96c72-105">Excluir um objeto [unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="96c72-105">Delete a [unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="96c72-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="96c72-106">Permissions</span></span>

<span data-ttu-id="96c72-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96c72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="96c72-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="96c72-109">Permission type</span></span>                        | <span data-ttu-id="96c72-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="96c72-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="96c72-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="96c72-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="96c72-112">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="96c72-112">RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="96c72-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="96c72-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96c72-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96c72-114">Not supported.</span></span> |
| <span data-ttu-id="96c72-115">Application</span><span class="sxs-lookup"><span data-stu-id="96c72-115">Application</span></span>                            | <span data-ttu-id="96c72-116">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="96c72-116">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="96c72-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="96c72-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /roleManagement/directory/roleDefinitions/{id}

```

## <a name="request-headers"></a><span data-ttu-id="96c72-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="96c72-118">Request headers</span></span>

| <span data-ttu-id="96c72-119">Nome</span><span class="sxs-lookup"><span data-stu-id="96c72-119">Name</span></span>          | <span data-ttu-id="96c72-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="96c72-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="96c72-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="96c72-121">Authorization</span></span> | <span data-ttu-id="96c72-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="96c72-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="96c72-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="96c72-123">Request body</span></span>

<span data-ttu-id="96c72-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="96c72-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96c72-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="96c72-125">Response</span></span>

<span data-ttu-id="96c72-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="96c72-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96c72-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="96c72-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="96c72-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96c72-129">Request</span></span>

<span data-ttu-id="96c72-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="96c72-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="96c72-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="96c72-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroledefinition"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/f189965f-f560-4c59-9101-933d4c87a91a
```
# <a name="c"></a>[<span data-ttu-id="96c72-132">C#</span><span class="sxs-lookup"><span data-stu-id="96c72-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="96c72-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="96c72-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="96c72-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="96c72-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="96c72-135">Java</span><span class="sxs-lookup"><span data-stu-id="96c72-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="96c72-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="96c72-136">Response</span></span>

<span data-ttu-id="96c72-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="96c72-137">The following is an example of the response.</span></span>

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
  "description": "Delete unifiedRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


