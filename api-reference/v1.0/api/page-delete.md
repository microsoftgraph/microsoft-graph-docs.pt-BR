---
title: Excluir página
description: Excluir uma página do OneNote.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 696513aab1be4ed8089ed4280b6e55f3798382d1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48087065"
---
# <a name="delete-page"></a><span data-ttu-id="b0a2d-103">Excluir página</span><span class="sxs-lookup"><span data-stu-id="b0a2d-103">Delete page</span></span>

<span data-ttu-id="b0a2d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0a2d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b0a2d-105">Excluir uma página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="b0a2d-105">Delete a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="b0a2d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b0a2d-106">Permissions</span></span>
<span data-ttu-id="b0a2d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0a2d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0a2d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b0a2d-109">Permission type</span></span>      | <span data-ttu-id="b0a2d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b0a2d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b0a2d-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b0a2d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b0a2d-112">Notes. ReadWrite, Notes. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b0a2d-112">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="b0a2d-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b0a2d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0a2d-114">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b0a2d-114">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="b0a2d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b0a2d-115">Application</span></span> | <span data-ttu-id="b0a2d-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0a2d-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b0a2d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b0a2d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/onenote/pages/{id}
DELETE /users/{id | userPrincipalName}/onenote/pages/{id}
DELETE /groups/{id}/onenote/pages/{id}
DELETE /sites/{id}/onenote/pages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b0a2d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b0a2d-118">Request headers</span></span>
| <span data-ttu-id="b0a2d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b0a2d-119">Name</span></span>       | <span data-ttu-id="b0a2d-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0a2d-120">Type</span></span> | <span data-ttu-id="b0a2d-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0a2d-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b0a2d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b0a2d-122">Authorization</span></span>  | <span data-ttu-id="b0a2d-123">string</span><span class="sxs-lookup"><span data-stu-id="b0a2d-123">string</span></span>  | <span data-ttu-id="b0a2d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b0a2d-p102">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="b0a2d-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0a2d-126">Response</span></span>

<span data-ttu-id="b0a2d-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b0a2d-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0a2d-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b0a2d-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b0a2d-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b0a2d-130">Request</span></span>
<span data-ttu-id="b0a2d-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b0a2d-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b0a2d-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="b0a2d-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_page"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/onenote/pages/{id}
```
# <a name="c"></a>[<span data-ttu-id="b0a2d-133">C#</span><span class="sxs-lookup"><span data-stu-id="b0a2d-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-page-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b0a2d-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b0a2d-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-page-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b0a2d-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b0a2d-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-page-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b0a2d-136">Java</span><span class="sxs-lookup"><span data-stu-id="b0a2d-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-page-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b0a2d-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0a2d-137">Response</span></span>
<span data-ttu-id="b0a2d-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b0a2d-138">Here is an example of the response.</span></span>
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

