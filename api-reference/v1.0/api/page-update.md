---
title: Atualizar página
description: Atualizar o conteúdo de uma página do OneNote.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 58732f60089320dd4c91ebb1b72401841fa9c5a8
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36309363"
---
# <a name="update-page"></a><span data-ttu-id="9af6f-103">Atualizar página</span><span class="sxs-lookup"><span data-stu-id="9af6f-103">Update page</span></span>

<span data-ttu-id="9af6f-104">Atualizar o conteúdo de uma página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="9af6f-104">Update the content of a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="9af6f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9af6f-105">Permissions</span></span>
<span data-ttu-id="9af6f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9af6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9af6f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9af6f-108">Permission type</span></span>      | <span data-ttu-id="9af6f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9af6f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9af6f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9af6f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9af6f-111">Notes. ReadWrite, Notes. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="9af6f-111">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="9af6f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9af6f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9af6f-113">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9af6f-113">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="9af6f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9af6f-114">Application</span></span> | <span data-ttu-id="9af6f-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9af6f-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9af6f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9af6f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/onenote/pages/{id}/content
PATCH /users/{id | userPrincipalName}/onenote/pages/{id}/content
PATCH /groups/{id}/onenote/pages/{id}/content
PATCH /sites/{id}/onenote/pages/{id}/content
```
## <a name="request-headers"></a><span data-ttu-id="9af6f-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9af6f-117">Request headers</span></span>
| <span data-ttu-id="9af6f-118">Nome</span><span class="sxs-lookup"><span data-stu-id="9af6f-118">Name</span></span>       | <span data-ttu-id="9af6f-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="9af6f-119">Type</span></span> | <span data-ttu-id="9af6f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="9af6f-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9af6f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9af6f-121">Authorization</span></span>  | <span data-ttu-id="9af6f-122">string</span><span class="sxs-lookup"><span data-stu-id="9af6f-122">string</span></span>  | <span data-ttu-id="9af6f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9af6f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9af6f-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9af6f-125">Content-Type</span></span> | <span data-ttu-id="9af6f-126">string</span><span class="sxs-lookup"><span data-stu-id="9af6f-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="9af6f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9af6f-127">Request body</span></span>
<span data-ttu-id="9af6f-128">No corpo da solicitação, forneça uma matriz de objetos [patchContentCommand](../resources/patchcontentcommand.md) que representam as alterações na página.</span><span class="sxs-lookup"><span data-stu-id="9af6f-128">In the request body, supply an array of [patchContentCommand](../resources/patchcontentcommand.md) objects that represent the changes to the page.</span></span> <span data-ttu-id="9af6f-129">Para obter mais informações e exemplos, consulte <a href="https://msdn.microsoft.com/office/office365/howto/onenote-update-page">Atualizar páginas do OneNote</a>.</span><span class="sxs-lookup"><span data-stu-id="9af6f-129">For more information and examples, see <a href="https://msdn.microsoft.com/office/office365/howto/onenote-update-page">Update OneNote pages</a>.</span></span>

## <a name="response"></a><span data-ttu-id="9af6f-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="9af6f-130">Response</span></span>

<span data-ttu-id="9af6f-131">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9af6f-131">If successful, this method returns a `204 No Content` response code.</span></span>  <span data-ttu-id="9af6f-132">Nenhum dado JSON é retornado para uma solicitação PATCH.</span><span class="sxs-lookup"><span data-stu-id="9af6f-132">No JSON data is returned for a PATCH request.</span></span>
## <a name="example"></a><span data-ttu-id="9af6f-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9af6f-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9af6f-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9af6f-134">Request</span></span>
<span data-ttu-id="9af6f-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9af6f-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9af6f-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="9af6f-136">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="9af6f-137">C#</span><span class="sxs-lookup"><span data-stu-id="9af6f-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-page-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9af6f-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9af6f-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-page-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9af6f-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="9af6f-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-page-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9af6f-140">Java</span><span class="sxs-lookup"><span data-stu-id="9af6f-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-page-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9af6f-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="9af6f-141">Response</span></span>
<span data-ttu-id="9af6f-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9af6f-142">Here is an example of the response.</span></span> 
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
