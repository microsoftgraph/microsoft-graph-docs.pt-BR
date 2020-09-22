---
title: Atualizar página
description: Atualizar o conteúdo de uma página do OneNote.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 4f3b8d219249b578f1876b1b30df7f3c7d2487b7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48004589"
---
# <a name="update-page"></a><span data-ttu-id="e0a55-103">Atualizar página</span><span class="sxs-lookup"><span data-stu-id="e0a55-103">Update page</span></span>

<span data-ttu-id="e0a55-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0a55-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0a55-105">Atualizar o conteúdo de uma página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="e0a55-105">Update the content of a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="e0a55-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e0a55-106">Permissions</span></span>
<span data-ttu-id="e0a55-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0a55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0a55-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e0a55-109">Permission type</span></span>      | <span data-ttu-id="e0a55-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e0a55-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e0a55-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e0a55-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e0a55-112">Notes. ReadWrite, Notes. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e0a55-112">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="e0a55-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e0a55-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0a55-114">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0a55-114">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="e0a55-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e0a55-115">Application</span></span> | <span data-ttu-id="e0a55-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0a55-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0a55-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e0a55-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/onenote/pages/{id}/content
PATCH /users/{id | userPrincipalName}/onenote/pages/{id}/content
PATCH /groups/{id}/onenote/pages/{id}/content
PATCH /sites/{id}/onenote/pages/{id}/content
```
## <a name="request-headers"></a><span data-ttu-id="e0a55-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e0a55-118">Request headers</span></span>
| <span data-ttu-id="e0a55-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e0a55-119">Name</span></span>       | <span data-ttu-id="e0a55-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="e0a55-120">Type</span></span> | <span data-ttu-id="e0a55-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0a55-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e0a55-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e0a55-122">Authorization</span></span>  | <span data-ttu-id="e0a55-123">string</span><span class="sxs-lookup"><span data-stu-id="e0a55-123">string</span></span>  | <span data-ttu-id="e0a55-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e0a55-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e0a55-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e0a55-126">Content-Type</span></span> | <span data-ttu-id="e0a55-127">string</span><span class="sxs-lookup"><span data-stu-id="e0a55-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="e0a55-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e0a55-128">Request body</span></span>
<span data-ttu-id="e0a55-129">No corpo da solicitação, forneça uma matriz de objetos [patchContentCommand](../resources/patchcontentcommand.md) que representam as alterações na página.</span><span class="sxs-lookup"><span data-stu-id="e0a55-129">In the request body, supply an array of [patchContentCommand](../resources/patchcontentcommand.md) objects that represent the changes to the page.</span></span> <span data-ttu-id="e0a55-130">Para obter mais informações e exemplos, consulte [Atualizar conteúdo da página do OneNote](/graph/onenote-update-page).</span><span class="sxs-lookup"><span data-stu-id="e0a55-130">For more information and examples, see [Update OneNote page content](/graph/onenote-update-page).</span></span>

## <a name="response"></a><span data-ttu-id="e0a55-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0a55-131">Response</span></span>

<span data-ttu-id="e0a55-132">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e0a55-132">If successful, this method returns a `204 No Content` response code.</span></span>  <span data-ttu-id="e0a55-133">Nenhum dado JSON é retornado para uma solicitação PATCH.</span><span class="sxs-lookup"><span data-stu-id="e0a55-133">No JSON data is returned for a PATCH request.</span></span>
## <a name="example"></a><span data-ttu-id="e0a55-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e0a55-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e0a55-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e0a55-135">Request</span></span>
<span data-ttu-id="e0a55-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e0a55-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e0a55-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="e0a55-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_page"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/onenote/pages/{id}/content
Content-type: application/json
Content-length: 312

[
   {
    'target':'#para-id',
    'action':'insert',
    'position':'before',
    'content':'<img src="image-url-or-part-name" alt="image-alt-text" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>new-page-content</li>'
  }
]
```
# <a name="c"></a>[<span data-ttu-id="e0a55-138">C#</span><span class="sxs-lookup"><span data-stu-id="e0a55-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-page-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e0a55-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e0a55-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-page-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e0a55-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e0a55-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-page-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e0a55-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0a55-141">Response</span></span>
<span data-ttu-id="e0a55-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e0a55-142">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenotePage"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update page",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


