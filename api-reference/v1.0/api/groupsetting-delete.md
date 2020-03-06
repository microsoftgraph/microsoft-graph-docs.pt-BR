---
title: Excluir uma configuração de grupo
description: Excluir uma configuração de grupo.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 20a6bded37bb2b881b0f9f85d313d0c25fd20560
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516840"
---
# <a name="delete-a-group-setting"></a><span data-ttu-id="12c87-103">Excluir uma configuração de grupo</span><span class="sxs-lookup"><span data-stu-id="12c87-103">Delete a group setting</span></span>

<span data-ttu-id="12c87-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12c87-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="12c87-105">Excluir uma configuração de grupo.</span><span class="sxs-lookup"><span data-stu-id="12c87-105">Delete a group setting.</span></span>

## <a name="permissions"></a><span data-ttu-id="12c87-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="12c87-106">Permissions</span></span>

<span data-ttu-id="12c87-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12c87-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="12c87-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="12c87-109">Permission type</span></span>      | <span data-ttu-id="12c87-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="12c87-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="12c87-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="12c87-111">Delegated (work or school account)</span></span> | <span data-ttu-id="12c87-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="12c87-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="12c87-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="12c87-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12c87-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="12c87-114">Not supported.</span></span>    |
|<span data-ttu-id="12c87-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="12c87-115">Application</span></span> | <span data-ttu-id="12c87-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12c87-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="12c87-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="12c87-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupSettings/{id}
DELETE /groups/{id}/settings/{id}

```

## <a name="request-headers"></a><span data-ttu-id="12c87-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="12c87-118">Request headers</span></span>

| <span data-ttu-id="12c87-119">Nome</span><span class="sxs-lookup"><span data-stu-id="12c87-119">Name</span></span> | <span data-ttu-id="12c87-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="12c87-120">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="12c87-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="12c87-121">Authorization</span></span>  | <span data-ttu-id="12c87-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="12c87-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="12c87-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="12c87-124">Content-Type</span></span>  | <span data-ttu-id="12c87-125">application/json</span><span class="sxs-lookup"><span data-stu-id="12c87-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="12c87-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="12c87-126">Request body</span></span>
<span data-ttu-id="12c87-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="12c87-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12c87-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="12c87-128">Response</span></span>

<span data-ttu-id="12c87-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="12c87-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12c87-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="12c87-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="12c87-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="12c87-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="12c87-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="12c87-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_groupsetting"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groupSettings/{id}
```
# <a name="c"></a>[<span data-ttu-id="12c87-134">C#</span><span class="sxs-lookup"><span data-stu-id="12c87-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-groupsetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="12c87-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="12c87-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-groupsetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="12c87-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="12c87-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-groupsetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="12c87-137">Java</span><span class="sxs-lookup"><span data-stu-id="12c87-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-groupsetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="12c87-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="12c87-138">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
