---
title: Excluir groupLifecyclePolicy
description: Exclui um objeto groupLifecyclePolicy.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 9a10ed79bfab49b797d5dd9b45376fd0f0a31a16
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36014666"
---
# <a name="delete-grouplifecyclepolicy"></a><span data-ttu-id="9b5ae-103">Excluir groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="9b5ae-103">Delete groupLifecyclePolicy</span></span>

<span data-ttu-id="9b5ae-104">Exclui um objeto [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9b5ae-104">Deletes a [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9b5ae-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9b5ae-105">Permissions</span></span>

<span data-ttu-id="9b5ae-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b5ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b5ae-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9b5ae-108">Permission type</span></span>      | <span data-ttu-id="9b5ae-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9b5ae-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9b5ae-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9b5ae-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9b5ae-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b5ae-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="9b5ae-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9b5ae-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b5ae-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b5ae-113">Not supported.</span></span>    |
|<span data-ttu-id="9b5ae-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9b5ae-114">Application</span></span> | <span data-ttu-id="9b5ae-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b5ae-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9b5ae-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9b5ae-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupLifecyclePolicies/{id}

```

## <a name="request-headers"></a><span data-ttu-id="9b5ae-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9b5ae-117">Request headers</span></span>

| <span data-ttu-id="9b5ae-118">Nome</span><span class="sxs-lookup"><span data-stu-id="9b5ae-118">Name</span></span> | <span data-ttu-id="9b5ae-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b5ae-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="9b5ae-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="9b5ae-120">Authorization</span></span> | <span data-ttu-id="9b5ae-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9b5ae-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9b5ae-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9b5ae-123">Content-Type</span></span>  | <span data-ttu-id="9b5ae-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9b5ae-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="9b5ae-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9b5ae-125">Request body</span></span>
<span data-ttu-id="9b5ae-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9b5ae-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="9b5ae-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b5ae-127">Response</span></span>

<span data-ttu-id="9b5ae-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9b5ae-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b5ae-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9b5ae-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9b5ae-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9b5ae-131">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="9b5ae-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="9b5ae-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_grouplifecyclepolicy"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9b5ae-133">C#</span><span class="sxs-lookup"><span data-stu-id="9b5ae-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-grouplifecyclepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9b5ae-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="9b5ae-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-grouplifecyclepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9b5ae-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="9b5ae-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-grouplifecyclepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9b5ae-136">Java</span><span class="sxs-lookup"><span data-stu-id="9b5ae-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-grouplifecyclepolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9b5ae-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b5ae-137">Response</span></span>

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
  "description": "Delete groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
