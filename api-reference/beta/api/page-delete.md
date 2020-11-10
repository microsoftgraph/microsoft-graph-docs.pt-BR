---
title: Excluir página
description: Excluir uma página do OneNote.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 8b8855631810cc20b5f1c6e7e82fb908d6bcedf8
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48964401"
---
# <a name="delete-page"></a><span data-ttu-id="cc80c-103">Excluir página</span><span class="sxs-lookup"><span data-stu-id="cc80c-103">Delete page</span></span>

<span data-ttu-id="cc80c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc80c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc80c-105">Excluir uma página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="cc80c-105">Delete a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="cc80c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cc80c-106">Permissions</span></span>
<span data-ttu-id="cc80c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc80c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc80c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cc80c-109">Permission type</span></span>      | <span data-ttu-id="cc80c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cc80c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc80c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cc80c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cc80c-112">Notes. ReadWrite, Notes. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="cc80c-112">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="cc80c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cc80c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc80c-114">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cc80c-114">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="cc80c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cc80c-115">Application</span></span> | <span data-ttu-id="cc80c-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc80c-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cc80c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cc80c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/onenote/pages/{id}
DELETE /users/{id | userPrincipalName}/onenote/pages/{id}
DELETE /groups/{id}/onenote/pages/{id}
DELETE /sites/{id}/onenote/pages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="cc80c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cc80c-118">Request headers</span></span>
| <span data-ttu-id="cc80c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="cc80c-119">Name</span></span>       | <span data-ttu-id="cc80c-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="cc80c-120">Type</span></span> | <span data-ttu-id="cc80c-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc80c-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cc80c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="cc80c-122">Authorization</span></span>  | <span data-ttu-id="cc80c-123">string</span><span class="sxs-lookup"><span data-stu-id="cc80c-123">string</span></span>  | <span data-ttu-id="cc80c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cc80c-p102">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="cc80c-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc80c-126">Response</span></span>

<span data-ttu-id="cc80c-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cc80c-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc80c-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cc80c-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cc80c-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cc80c-130">Request</span></span>
<span data-ttu-id="cc80c-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cc80c-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cc80c-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="cc80c-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_page"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/onenote/pages/{id}
```
# <a name="c"></a>[<span data-ttu-id="cc80c-133">C#</span><span class="sxs-lookup"><span data-stu-id="cc80c-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-page-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cc80c-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cc80c-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-page-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cc80c-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cc80c-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-page-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cc80c-136">Java</span><span class="sxs-lookup"><span data-stu-id="cc80c-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-page-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="cc80c-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc80c-137">Response</span></span>
<span data-ttu-id="cc80c-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cc80c-138">Here is an example of the response.</span></span>
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
  "description": "Delete page",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


