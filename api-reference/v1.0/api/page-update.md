---
title: Atualizar página
description: Atualizar o conteúdo de uma página do OneNote.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 31678efb9f72ef11648f3352a2802b9471d587c9
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35455270"
---
# <a name="update-page"></a><span data-ttu-id="d2bb2-103">Atualizar página</span><span class="sxs-lookup"><span data-stu-id="d2bb2-103">Update page</span></span>

<span data-ttu-id="d2bb2-104">Atualizar o conteúdo de uma página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="d2bb2-104">Update the content of a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="d2bb2-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d2bb2-105">Permissions</span></span>
<span data-ttu-id="d2bb2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2bb2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2bb2-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d2bb2-108">Permission type</span></span>      | <span data-ttu-id="d2bb2-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d2bb2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2bb2-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d2bb2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d2bb2-111">Notes. ReadWrite, Notes. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d2bb2-111">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="d2bb2-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d2bb2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2bb2-113">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d2bb2-113">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="d2bb2-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d2bb2-114">Application</span></span> | <span data-ttu-id="d2bb2-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2bb2-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d2bb2-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d2bb2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/onenote/pages/{id}/content
PATCH /users/{id | userPrincipalName}/onenote/pages/{id}/content
PATCH /groups/{id}/onenote/pages/{id}/content
PATCH /sites/{id}/onenote/pages/{id}/content
```
## <a name="request-headers"></a><span data-ttu-id="d2bb2-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d2bb2-117">Request headers</span></span>
| <span data-ttu-id="d2bb2-118">Nome</span><span class="sxs-lookup"><span data-stu-id="d2bb2-118">Name</span></span>       | <span data-ttu-id="d2bb2-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="d2bb2-119">Type</span></span> | <span data-ttu-id="d2bb2-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2bb2-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d2bb2-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d2bb2-121">Authorization</span></span>  | <span data-ttu-id="d2bb2-122">string</span><span class="sxs-lookup"><span data-stu-id="d2bb2-122">string</span></span>  | <span data-ttu-id="d2bb2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d2bb2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d2bb2-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d2bb2-125">Content-Type</span></span> | <span data-ttu-id="d2bb2-126">string</span><span class="sxs-lookup"><span data-stu-id="d2bb2-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="d2bb2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d2bb2-127">Request body</span></span>
<span data-ttu-id="d2bb2-128">No corpo da solicitação, forneça uma matriz de objetos [patchContentCommand](../resources/patchcontentcommand.md) que representam as alterações na página.</span><span class="sxs-lookup"><span data-stu-id="d2bb2-128">In the request body, supply an array of [patchContentCommand](../resources/patchcontentcommand.md) objects that represent the changes to the page.</span></span> <span data-ttu-id="d2bb2-129">Para obter mais informações e exemplos, consulte <a href="https://msdn.microsoft.com/office/office365/howto/onenote-update-page">Atualizar páginas do OneNote</a>.</span><span class="sxs-lookup"><span data-stu-id="d2bb2-129">For more information and examples, see <a href="https://msdn.microsoft.com/office/office365/howto/onenote-update-page">Update OneNote pages</a>.</span></span>

## <a name="response"></a><span data-ttu-id="d2bb2-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2bb2-130">Response</span></span>

<span data-ttu-id="d2bb2-131">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d2bb2-131">If successful, this method returns a `204 No Content` response code.</span></span>  <span data-ttu-id="d2bb2-132">Nenhum dado JSON é retornado para uma solicitação PATCH.</span><span class="sxs-lookup"><span data-stu-id="d2bb2-132">No JSON data is returned for a PATCH request.</span></span>
## <a name="example"></a><span data-ttu-id="d2bb2-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d2bb2-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d2bb2-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d2bb2-134">Request</span></span>
<span data-ttu-id="d2bb2-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d2bb2-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d2bb2-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="d2bb2-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_page"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/onenote/pages/{id}/content
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="d2bb2-137">C#</span><span class="sxs-lookup"><span data-stu-id="d2bb2-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-page-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d2bb2-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="d2bb2-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-page-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d2bb2-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d2bb2-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-page-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d2bb2-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2bb2-140">Response</span></span>
<span data-ttu-id="d2bb2-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d2bb2-141">Here is an example of the response.</span></span> 
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
<!-- {
  "type": "#page.annotation",
  "description": "Update page",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
