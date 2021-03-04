---
title: Remover membro da função de diretório
description: Remove um membro de um directoryRole.
author: abhijeetsinha
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 2e5082488dbed8452abeecae904751ae3dff6dde
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436838"
---
# <a name="remove-directory-role-member"></a><span data-ttu-id="e5ce1-103">Remover membro da função de diretório</span><span class="sxs-lookup"><span data-stu-id="e5ce1-103">Remove directory role member</span></span>

<span data-ttu-id="e5ce1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5ce1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5ce1-105">Remove um membro de um directoryRole.</span><span class="sxs-lookup"><span data-stu-id="e5ce1-105">Remove a member from a directoryRole.</span></span>

## <a name="permissions"></a><span data-ttu-id="e5ce1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e5ce1-106">Permissions</span></span>

<span data-ttu-id="e5ce1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5ce1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e5ce1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e5ce1-109">Permission type</span></span>      | <span data-ttu-id="e5ce1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e5ce1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5ce1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e5ce1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e5ce1-112">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e5ce1-112">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e5ce1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e5ce1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5ce1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5ce1-114">Not supported.</span></span>    |
|<span data-ttu-id="e5ce1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5ce1-115">Application</span></span> | <span data-ttu-id="e5ce1-116">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="e5ce1-116">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="e5ce1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e5ce1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directoryRoles/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="e5ce1-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e5ce1-118">Request headers</span></span>

| <span data-ttu-id="e5ce1-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e5ce1-119">Name</span></span>       | <span data-ttu-id="e5ce1-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="e5ce1-120">Type</span></span> | <span data-ttu-id="e5ce1-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5ce1-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e5ce1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e5ce1-122">Authorization</span></span>  | <span data-ttu-id="e5ce1-123">string</span><span class="sxs-lookup"><span data-stu-id="e5ce1-123">string</span></span>  | <span data-ttu-id="e5ce1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e5ce1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e5ce1-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e5ce1-126">Request body</span></span>

<span data-ttu-id="e5ce1-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e5ce1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5ce1-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5ce1-128">Response</span></span>

<span data-ttu-id="e5ce1-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e5ce1-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5ce1-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e5ce1-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e5ce1-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e5ce1-132">Request</span></span>

<span data-ttu-id="e5ce1-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e5ce1-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e5ce1-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="e5ce1-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole"
}-->

```http
DELETE https://graph.microsoft.com/beta/directoryRoles/{id}/members/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="e5ce1-135">C#</span><span class="sxs-lookup"><span data-stu-id="e5ce1-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-from-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e5ce1-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e5ce1-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-from-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e5ce1-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e5ce1-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-from-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e5ce1-138">Java</span><span class="sxs-lookup"><span data-stu-id="e5ce1-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directoryobject-from-directoryrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e5ce1-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5ce1-139">Response</span></span>

<span data-ttu-id="e5ce1-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e5ce1-140">Here is an example of the response.</span></span> 
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
  "description": "Delete a member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


