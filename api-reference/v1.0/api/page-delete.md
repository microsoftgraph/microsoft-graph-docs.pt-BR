---
title: Excluir página
description: Excluir uma página do OneNote.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: c835e1335653234cc16d40ce3f3c1be1de3440b6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511093"
---
# <a name="delete-page"></a><span data-ttu-id="f92a7-103">Excluir página</span><span class="sxs-lookup"><span data-stu-id="f92a7-103">Delete page</span></span>

<span data-ttu-id="f92a7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f92a7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f92a7-105">Excluir uma página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="f92a7-105">Delete a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="f92a7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f92a7-106">Permissions</span></span>
<span data-ttu-id="f92a7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f92a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f92a7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f92a7-109">Permission type</span></span>      | <span data-ttu-id="f92a7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f92a7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f92a7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f92a7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f92a7-112">Notes. ReadWrite, Notes. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f92a7-112">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="f92a7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f92a7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f92a7-114">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f92a7-114">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="f92a7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f92a7-115">Application</span></span> | <span data-ttu-id="f92a7-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f92a7-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f92a7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f92a7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/onenote/pages/{id}
DELETE /users/{id | userPrincipalName}/onenote/pages/{id}
DELETE /groups/{id}/onenote/pages/{id}
DELETE /sites/{id}/onenote/pages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="f92a7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f92a7-118">Request headers</span></span>
| <span data-ttu-id="f92a7-119">Nome</span><span class="sxs-lookup"><span data-stu-id="f92a7-119">Name</span></span>       | <span data-ttu-id="f92a7-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="f92a7-120">Type</span></span> | <span data-ttu-id="f92a7-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f92a7-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f92a7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f92a7-122">Authorization</span></span>  | <span data-ttu-id="f92a7-123">string</span><span class="sxs-lookup"><span data-stu-id="f92a7-123">string</span></span>  | <span data-ttu-id="f92a7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f92a7-p102">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="f92a7-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="f92a7-126">Response</span></span>

<span data-ttu-id="f92a7-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f92a7-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f92a7-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f92a7-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f92a7-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f92a7-130">Request</span></span>
<span data-ttu-id="f92a7-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f92a7-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f92a7-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="f92a7-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_page"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/onenote/pages/{id}
```
# <a name="c"></a>[<span data-ttu-id="f92a7-133">C#</span><span class="sxs-lookup"><span data-stu-id="f92a7-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-page-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f92a7-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f92a7-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-page-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f92a7-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f92a7-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-page-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f92a7-136">Java</span><span class="sxs-lookup"><span data-stu-id="f92a7-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-page-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f92a7-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="f92a7-137">Response</span></span>
<span data-ttu-id="f92a7-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f92a7-138">Here is an example of the response.</span></span>
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
  "description": "Delete page",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
