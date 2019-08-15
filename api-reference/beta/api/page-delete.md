---
title: Excluir página
description: Excluir uma página do OneNote.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: eeec6fea8a4d4ca374af4f2503240534b2e378fa
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36413829"
---
# <a name="delete-page"></a><span data-ttu-id="e0c2c-103">Excluir página</span><span class="sxs-lookup"><span data-stu-id="e0c2c-103">Delete page</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0c2c-104">Excluir uma página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="e0c2c-104">Delete a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="e0c2c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e0c2c-105">Permissions</span></span>
<span data-ttu-id="e0c2c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0c2c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0c2c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e0c2c-108">Permission type</span></span>      | <span data-ttu-id="e0c2c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e0c2c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e0c2c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e0c2c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e0c2c-111">Notes. ReadWrite, Notes. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e0c2c-111">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="e0c2c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e0c2c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0c2c-113">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0c2c-113">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="e0c2c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e0c2c-114">Application</span></span> | <span data-ttu-id="e0c2c-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0c2c-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0c2c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e0c2c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/onenote/pages/{id}
DELETE /users/{id | userPrincipalName}/onenote/pages/{id}
DELETE /groups/{id}/onenote/pages/{id}
DELETE /sites/{id}/onenote/pages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="e0c2c-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e0c2c-117">Request headers</span></span>
| <span data-ttu-id="e0c2c-118">Nome</span><span class="sxs-lookup"><span data-stu-id="e0c2c-118">Name</span></span>       | <span data-ttu-id="e0c2c-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="e0c2c-119">Type</span></span> | <span data-ttu-id="e0c2c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0c2c-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e0c2c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e0c2c-121">Authorization</span></span>  | <span data-ttu-id="e0c2c-122">string</span><span class="sxs-lookup"><span data-stu-id="e0c2c-122">string</span></span>  | <span data-ttu-id="e0c2c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e0c2c-p102">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="e0c2c-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0c2c-125">Response</span></span>

<span data-ttu-id="e0c2c-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e0c2c-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0c2c-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e0c2c-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e0c2c-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e0c2c-129">Request</span></span>
<span data-ttu-id="e0c2c-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e0c2c-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e0c2c-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="e0c2c-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_page"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/onenote/pages/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e0c2c-132">C#</span><span class="sxs-lookup"><span data-stu-id="e0c2c-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-page-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e0c2c-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e0c2c-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-page-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e0c2c-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="e0c2c-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-page-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e0c2c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0c2c-135">Response</span></span>
<span data-ttu-id="e0c2c-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e0c2c-136">Here is an example of the response.</span></span>
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
